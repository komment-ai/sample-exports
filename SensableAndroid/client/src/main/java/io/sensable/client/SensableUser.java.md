![Alt text](./SensableUser.java.md.svg)

## description


A Java class responsible for handling user authentication and settings retrieval in an Android application. It provides functions to login, logout, retrieve user settings, save the user's information to preferences, and delete the saved user information.

## code_explanation


The SensableUser class is designed to interact with the Sensable API to authenticate users and retrieve their settings. It uses the Retrofit library to make HTTP requests to the API and stores user data in shared preferences. The class has methods for logging in, logging out, retrieving user settings, saving user data to preferences, and deleting saved user information.

## dependencies


### Built-in Libraries

*   `java.lang`: Provides basic classes and interfaces for the Java programming language, such as `String`, `Integer`, and `Exception`.
*   `java.net`: Provides classes for working with network protocols, such as `CookieManager` and `CookiePolicy`.
*   `android.content`: Provides classes for working with Android content, such as `Context` and `SharedPreferences`.

### Third-party Libraries

*   `retrofit`: A type-safe HTTP client for Android and Java.
*   `io.sensable`: A library for interacting with the Sensable API.

### Custom Libraries

*   `io.sensable.model.User`: A class representing a user, with properties for username, email, and access token.
*   `io.sensable.model.UserLogin`: A class representing user login credentials, with properties for username and email.
*   `MainActivity.CallbackInterface`: An interface for callback methods, with a single method for updating the login status of the user.

## security_insights


The SensableUser class stores user credentials in shared preferences, which may be a security risk if the device is compromised. Additionally, the class uses a `CookieManager` to store cookies from the API, which may also be a security risk if not properly managed.

## additional_information


*   The SensableUser class uses a `RestAdapter` to make HTTP requests to the API, which can be configured to use different authentication methods or API endpoints.
*   The class uses a `CallbackInterface` to notify the caller of the login status, which can be used to update the UI or perform other actions based on the login status.
*   The `saveUserToPreferences` method stores user data in shared preferences, which can be used to persist user data between app sessions.
*   The `deleteSavedUser` method removes saved user information from shared preferences, which can be used to log out the user and clear their data.

Endpoint 1: http://sensable.io/login
    Description: API endpoint for user login
    Method: POST
    Request Parameters:
        - username: The username of the user attempting to log in
        - email: The email address of the user attempting to log in
    Response: A `User` object representing the authenticated user

Endpoint 2: http://sensable.io/settings
    Description: API endpoint for user settings
    Method: GET
    Request Parameters:
        - username: The username of the user attempting to retrieve their settings
    Response: A `User` object representing the user's settings
## usage_instructions

**Usage Instructions for SensableUser Class**

### Using the SensableUser Class

**Overview:**
The SensableUser class is a utility class responsible for handling user authentication and settings retrieval in an Android application. It provides functions to login, logout, retrieve user settings, and save the user's information to preferences.

**Step 1: Import the Class**

* Import the SensableUser class into your Android project using the following line of code: `import io.sensable.client.SensibleUser;`

**Step 2: Initialize the Class**

* Initialize the SensableUser class by passing the SharedPreferences and Context objects to its constructor: `SensibleUser sensableUser = new SensableUser(sharedPreferences, context);`

**Step 3: Login to Sensable**

* Call the login method to authenticate the user with Sensable, passing the UserLogin object and a CallbackInterface object as inputs: `sensableUser.login(userLogin, callbackInterface);`

* The login method will call the Sensable API to authenticate the user and update the user's data and preferences upon success.

**Step 4: Retrieve User Settings**

* Call the userSettings method to retrieve the user's settings from the Sensable API: `sensableUser.userSettings();`

* The userSettings method will call the Sensable API to retrieve the user's settings and update the user's data and preferences upon success.

**Step 5: Save User Information to Preferences**

* Call the saveUserToPreferences method to save the user's information to preferences: `sensableUser.saveUserToPreferences();`

* The saveUserToPreferences method will save the user's username, email, and access token to preferences.

**Step 6: Logout and Delete Saved User Information**

* Call the deleteSavedUser method to remove the saved user information from preferences and update the login status, access token, and user data to empty values: `sensableUser.deleteSavedUser(callbackInterface);`

* The deleteSavedUser method will remove the saved user information from preferences and update the login status, access token, and user data to empty values.

**Example Usage:**

```java
import android.content.Context;
import android.content.SharedPreferences;
import io.sensable.client.SensibleUser;

public class MainActivity extends AppCompatActivity {

    private SharedPreferences sharedPreferences;
    private Context context;
    private SensibleUser sensableUser;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        sharedPreferences = getSharedPreferences("sensable_user", MODE_PRIVATE);
        context = this;
        sensableUser = new SensibleUser(sharedPreferences, context);

        // Login to Sensable
        UserLogin userLogin = new UserLogin("username", "email");
        sensableUser.login(userLogin, new CallbackInterface() {
            @Override
            public void loginStatusUpdate(boolean loggedIn) {
                if (loggedIn) {
                    // User is logged in
                } else {
                    // User is not logged in
                }
            }

            @Override
            public void failure(RetrofitError retrofitError) {
                // Login failed
            }
        });
    }

    private class CallbackInterface implements SensibleUser.CallbackInterface {
        @Override
        public void loginStatusUpdate(boolean loggedIn) {
            // Update the login status
        }

        @Override
        public void failure(RetrofitError retrofitError) {
            // Handle the failure
        }
    }
}
```

By following these steps, you can successfully use the SensableUser class in your Android application.
