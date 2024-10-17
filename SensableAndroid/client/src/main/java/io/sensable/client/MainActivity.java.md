![Alt text](./MainActivity.java.md.svg)

## description


This is a basic implementation of an Android application using the Android SDK. It provides a framework for managing user interactions with sensors, including login and create sensable functionality. The class implements the ActionBar.TabListener interface to handle tab selection events and initializes tabs using a TabsPagerAdapter.

## code_explanation


The `MainActivity` class extends `FragmentActivity` and implements `ActionBar.TabListener`. It uses a `ViewPager` to display fragments and an `ActionBar` to manage tab selection. The class initializes tabs using a `TabsPagerAdapter` and sets up a callback interface for handling login status updates.

The `onCreate` method sets up the user interface and initializes the `SensableUser` class, which manages the user's login state. It also inflates the menu with options based on the logged-in status of the sensable user.

The `onOptionsItemSelected` method handles menu item selections, such as opening the about screen or login dialog, logging out, and creating a new sensable user.

The `loginDialog` method creates a fragment to display a login dialog and sets up a listener to handle the login confirmation event.

The `createSensable` method creates a fragment to display a scheduled sensable and sets up a listener for when the sensable is confirmed.

## dependencies


### Built-in Libraries

*   `android.app`: Provides classes for building Android applications, including activities, fragments, and services.
*   `android.content`: Provides classes for managing content, including resources, preferences, and intents.
*   `android.os`: Provides classes for managing operating system resources, including threads, processes, and memory.
*   `android.util`: Provides utility classes for working with Android resources, including logging and formatting.

### Third-party Libraries

*   `retrofit`: A library for making HTTP requests in Android, providing a simple and efficient way to interact with web services.
*   `io.sensable`: A custom library for working with sensable data, providing classes for managing user interactions and sensor data.

### Custom Libraries

*   `io.sensable.client.adapter`: A custom library for working with sensable adapters, providing classes for managing tab adapters and fragment managers.
*   `io.sensable.model`: A custom library for working with sensable models, providing classes for managing user login and sensable data.

## security_insights


No security insights are available for this file.

## additional_information


*   The `SensableUser` class can be extended to include more features, such as user authentication and authorization.
*   The `loginDialog` method can be modified to use a different login dialog fragment or to handle login errors in a different way.
*   The `createSensable` method can be modified to use a different fragment for creating sensables or to handle sensable creation errors in a different way.

Endpoints:

*   None

Note: This is a basic implementation of an Android application and does not include any REST API endpoints.
## usage_instructions

**Usage Instructions for MainActivity Class**

### Using the MainActivity Class

**Overview:**
The MainActivity class is the main entry point of the Android application, responsible for handling user interactions and displaying the application's UI.

**Step 1: Import the Class**

* Import the MainActivity class into your Android project using the following line of code: `import io.sensable.client.MainActivity;`

**Step 2: Extend the Class**

* Extend the MainActivity class in your Android activity file, for example: `public class MyActivity extends MainActivity {`

**Step 3: Override Required Methods**

* Override the following methods to implement the necessary functionality:
	+ `onCreate(Bundle savedInstanceState)`: Called when the activity is created. Use this method to initialize the UI and set up the necessary components.
	+ `onOptionsItemSelected(MenuItem item)`: Handles menu item selections, such as logging in, logging out, and creating a new sensable user.
	+ `onTabSelected(ActionBar.Tab tab, FragmentTransaction ft)`: Updates the current item displayed by a `ViewPager` when a tab is selected in an `ActionBar`.

**Step 4: Implement Callback Interface**

* Implement the `CallbackInterface` to handle login status updates, for example:
```java
public class MyActivity extends MainActivity implements CallbackInterface {
    @Override
    public void loginStatusUpdate(Boolean loggedIn) {
        if (loggedIn) {
            Toast.makeText(this, "Logged In", Toast.LENGTH_SHORT).show();
        } else {
            Toast.makeText(this, "Logged Out", Toast.LENGTH_SHORT).show();
        }
    }
}
```
**Step 5: Initialize the UI**

* Initialize the UI components, such as the `ViewPager` and `ActionBar`, in the `onCreate` method:
```java
@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.main_activity);

    // Initialize ViewPager and ActionBar
    ViewPager viewPager = findViewById(R.id.pager);
    viewPager.setAdapter(new TabsPagerAdapter(getSupportFragmentManager()));
    ActionBar actionBar = getActionBar();
    actionBar.setHomeButtonEnabled(false);
    actionBar.setNavigationMode(ActionBar.NAVIGATION_MODE_TABS);
}
```
**Step 6: Handle Menu Item Selections**

* Handle menu item selections in the `onOptionsItemSelected` method:
```java
@Override
public boolean onOptionsItemSelected(MenuItem item) {
    int id = item.getItemId();
    if (id == R.id.action_login) {
        loginDialog();
    } else if (id == R.id.action_logout) {
        sensableUser.deleteSavedUser(new CallbackInterface() {
            @Override
            public void loginStatusUpdate(Boolean loggedIn) {
                if (!loggedIn) {
                    Toast.makeText(MainActivity.this, "Logged out", Toast.LENGTH_SHORT).show();
                } else {
                    Toast.makeText(MainActivity.this, "Logout failed", Toast.LENGTH_SHORT).show();
                }
                invalidateOptionsMenu();
            }
        });
    }
    return super.onOptionsItemSelected(item);
}
```
**Step 7: Display the UI**

* Display the UI by calling the `startActivity` method:
```java
@Override
protected void onStart() {
    super.onStart();
    Intent intent = new Intent(this, MyActivity.class);
    startActivity(intent);
}
```
**Example Usage:**

```java
public class MyActivity extends MainActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.main_activity);

        // Initialize ViewPager and ActionBar
        ViewPager viewPager = findViewById(R.id.pager);
        viewPager.setAdapter(new TabsPagerAdapter(getSupportFragmentManager()));
        ActionBar actionBar = getActionBar();
        actionBar.setHomeButtonEnabled(false);
        actionBar.setNavigationMode(ActionBar.NAVIGATION_MODE_TABS);
    }

    @Override
    public boolean onOptionsItemSelected(MenuItem item) {
        int id = item.getItemId();
        if (id == R.id.action_login) {
            loginDialog();
        } else if (id == R.id.action_logout) {
            sensableUser.deleteSavedUser(new CallbackInterface() {
                @Override
                public void loginStatusUpdate(Boolean loggedIn) {
                    if (!loggedIn) {
                        Toast.makeText(MainActivity.this, "Logged out", Toast.LENGTH_SHORT).show();
                    } else {
                        Toast.makeText(MainActivity.this, "Logout failed", Toast.LENGTH_SHORT).show();
                    }
                    invalidateOptionsMenu();
                }
            });
        }
        return super.onOptionsItemSelected(item);
    }
}
```
By following these steps, you can successfully use the MainActivity class in your Android application.
