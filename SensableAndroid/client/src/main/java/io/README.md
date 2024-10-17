![Alt text](./README.md.svg)

## Description

A directory containing Java source files for the client-side application of the SensableAndroid project. This directory is part of the client module and contains the main application logic, including activities, fragments, adapters, and database helpers.


## Package Structure

The directory is organized into several sub-packages, each containing related classes and interfaces. The main packages are:

* `io.sensable.client`: Contains the main application activities, fragments, and helpers.
* `io.sensable.client.adapter`: Contains adapters for displaying data in the application.
* `io.sensable.client.component`: Contains custom UI components.
* `io.sensable.client.scheduler`: Contains classes for scheduling tasks and handling boot events.
* `io.sensable.client.sqlite`: Contains database helpers and providers for storing and retrieving data.
* `io.sensable.client.views`: Contains fragments and adapters for displaying data in the application.


## Key Classes and Interfaces

Some of the key classes and interfaces in this directory include:

* `MainActivity.java`: The main activity of the application.
* `SensableActivity.java`: An activity for displaying sensable data.
* `SensorHelper.java`: A helper class for working with sensors.
* `SensableLoginFragment.java`: A fragment for logging in to the application.
* `CreateSensableFragment.java`: A fragment for creating new sensables.
* `SensableContentProvider.java`: A content provider for accessing sensable data.
* `SensableDatabaseHelper.java`: A helper class for working with the sensable database.


## Dependencies

This directory depends on the `library` module, which contains the SensableService and other shared classes.



