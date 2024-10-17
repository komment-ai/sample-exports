![Alt text](./SensableDatabaseHelper.java.md.svg)

## description


A SQLiteOpenHelper class that provides a singleton connection to a SQLite database for content providers. It creates and manages the database schema and provides a way to access the database through a single instance.

## code_explanation


The SensableDatabaseHelper class is a SQLiteOpenHelper that extends the Android SQLiteOpenHelper class. It provides a singleton connection to a SQLite database for content providers. The class creates and manages the database schema and provides a way to access the database through a single instance.

The class uses a static instance variable `sInstance` to store a reference to a SensableDatabaseHelper object. This variable is used to store a single instance of the helper class, which can be retrieved by calling the `getHelper` function.

The `getHelper` function provides a single instance of SensableDatabaseHelper for a given Context. If the instance is null, it creates a new one using the context's application context.

The class also overrides the `onCreate` and `onUpgrade` methods of the SQLiteOpenHelper class. The `onCreate` method is responsible for creating the SavedSensablesTable and ScheduledSensablesTable in a SQLite database. The `onUpgrade` method updates the SavedSensables and ScheduledSensables tables when upgrading the database version.

## dependencies


### Built-in Libraries

*   `android.content.Context`: The Context class represents the Android application environment, providing access to various components and resources within the app.
*   `android.database.sqlite.SQLiteDatabase`: The SQLiteDatabase class represents a SQLite database, providing methods for performing database operations.
*   `android.database.sqlite.SQLiteOpenHelper`: The SQLiteOpenHelper class is a helper class that simplifies the process of creating, modifying, and upgrading SQLite databases.

### Third-party Libraries

*   `io.sensable.client.settings.Config`: The Config class is used to store configuration settings, including the database name, version, and other settings.

### Custom Libraries

*   `io.sensable.client.sqlite.SavedSensablesTable`: The SavedSensablesTable class is used to create and manage the SavedSensables table in the SQLite database.
*   `io.sensable.client.sqlite.ScheduledSensablesTable`: The ScheduledSensablesTable class is used to create and manage the ScheduledSensables table in the SQLite database.

## security_insights


No security insights are available for this file.

## additional_information


*   The SensableDatabaseHelper class uses a singleton pattern to provide a single instance of the helper class, which can be retrieved by calling the `getHelper` function.
*   The class creates and manages the database schema, including the SavedSensablesTable and ScheduledSensablesTable.
*   The `onUpgrade` method is used to update the database schema when upgrading the database version.
*   The class uses the `Config` class to store configuration settings, including the database name, version, and other settings.
## usage_instructions

**Usage Instructions for SensableDatabaseHelper Class**

### Using the SensableDatabaseHelper Class

**Overview:**
The SensableDatabaseHelper class is a SQLiteOpenHelper that provides a singleton connection to a SQLite database for content providers.

**Step 1: Import the Class**

* Import the SensableDatabaseHelper class into your Android application using the following line of code: `import io.sensable.client.sqlite.SensableDatabaseHelper;`

**Step 2: Get a Singleton Instance of the Helper Class**

* Use the `getHelper` method to get a singleton instance of the SensableDatabaseHelper class, passing in the Android application context: `SensableDatabaseHelper helper = SensableDatabaseHelper.getHelper(context);`

**Step 3: Perform Database Operations**

* Use the `getWritableDatabase` method to get a writable database instance: `SQLiteDatabase db = helper.getWritableDatabase();`
* Perform database operations using the `db` instance, such as inserting, updating, or deleting data.

**Step 4: Handle Database Upgrade**

* Use the `onUpgrade` method to handle database upgrade when the database version changes.

**Step 5: Close the Database**

* Use the `close` method to close the database instance when it is no longer needed.

**Configuration Options:**

* `Config.SENSABLE_STORAGE_DB`: The name of the SQLite database file.
* `Config.SENSABLE_STORAGE_DB_VERSION`: The version of the SQLite database schema.

**Potential Pitfalls:**

* Make sure to close the database instance when it is no longer needed to avoid memory leaks.
* Use the `getWritableDatabase` method to get a writable database instance, but be aware that it may throw an exception if the database is not available.

**Example Usage:**

```java
import android.content.Context;
import io.sensable.client.sqlite.SensableDatabaseHelper;

public class MainActivity extends AppCompatActivity {
    private SensableDatabaseHelper helper;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        helper = SensableDatabaseHelper.getHelper(this);
        SQLiteDatabase db = helper.getWritableDatabase();
        // Perform database operations using the db instance
        db.close();
    }
}
```

By following these steps, you can successfully use the SensableDatabaseHelper class in your Android application.
