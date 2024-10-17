![Alt text](./README.md.svg)

## Description

The `./client/` directory contains the source code for the Android client application of the SensableAndroid project. It includes the user interface, business logic, and data storage components of the client-side functionality.


## Structure

The directory is organized into the following subdirectories:
* `src/main/java/`: Java source code for the client application, including activities, fragments, adapters, and database helpers.
* `src/main/res/`: Resources for the client application, including layouts, drawables, menus, and values.
* `src/main/assets/`: Assets for the client application, including images and other files.


## Functionality

The client application provides the following functionality:
* User login and registration
* Sensable creation and management
* Sensable data visualization and analysis
* Data storage and retrieval using a SQLite database
* Scheduling and notification functionality


## Key Components

* `MainActivity.java`: The main entry point of the client application.
* `SensableActivity.java`: Handles sensable creation and management.
* `SensorHelper.java`: Provides utility functions for sensor-related tasks.
* `SensableDatabaseHelper.java`: Manages the SQLite database for storing sensable data.
* `ScheduledSensableService.java`: Handles scheduling and notification functionality.


## Dependencies

The client application depends on the `library/` module, which provides the core functionality for sensable data processing and communication.



