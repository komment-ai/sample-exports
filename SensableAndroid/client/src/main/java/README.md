![Alt text](./README.md.svg)

## Description

The `./client/src/main/java/` directory contains the Java source code for the client-side application of the SensableAndroid project. This directory holds the core logic, UI components, and data storage mechanisms for the client application.


## Package Structure

The Java source code is organized into several packages, each representing a specific aspect of the application:

* `io.sensable.client`: Contains the main activities, fragments, and UI components of the application.
* `io.sensable.client.adapter`: Holds adapters for displaying data in the application's UI.
* `io.sensable.client.component`: Contains custom UI components used in the application.
* `io.sensable.client.scheduler`: Holds classes responsible for scheduling tasks and handling boot events.
* `io.sensable.client.settings`: Contains classes for managing application settings and configurations.
* `io.sensable.client.sqlite`: Holds classes for interacting with the application's SQLite database.
* `io.sensable.client.views`: Contains fragments and adapters for displaying data in the application's UI.


## Key Classes and Components

Some notable classes and components in this directory include:

* `MainActivity.java`: The main entry point of the application.
* `SensableActivity.java`: An activity for displaying and interacting with sensable data.
* `SensorHelper.java`: A utility class for working with sensor data.
* `SensableListAdapter.java`: An adapter for displaying sensable data in a list.
* `LocalSensablesFragment.java` and `RemoteSensablesFragment.java`: Fragments for displaying local and remote sensable data, respectively.


## Dependencies

This directory depends on the `library` module, which provides the core sensable functionality.



