![Alt text](./README.md.svg)

## Description

A directory containing the main Java code for the client application of the SensableAndroid project. This directory holds the logic for the client-side functionality, including user interface, sensor handling, and database interactions.


## Package Structure

The directory is organized into several sub-packages, each containing related classes and functionality:

* `io.sensable.client`: Main package for client application code, including activities, fragments, and adapters.
* `io.sensable.client.component`: Custom UI components, such as the `FontFitTextView`.
* `io.sensable.client.scheduler`: Classes related to scheduling and boot receiver functionality.
* `io.sensable.client.sqlite`: Database-related classes, including content providers and database helpers.
* `io.sensable.client.views`: Custom view classes, including fragments and list adapters.


## Key Classes and Functionality

Some notable classes and their functionality include:

* `MainActivity`: The main entry point for the client application.
* `SensableActivity`: An activity for displaying sensable data.
* `SensorHelper`: A utility class for handling sensor-related tasks.
* `SensableLoginFragment`: A fragment for handling user login functionality.
* `ScheduledSensableService`: A service for handling scheduled sensable tasks.
* `SensableDatabaseHelper`: A helper class for interacting with the sensable database.


## Dependencies

This directory depends on the `library` module, which contains the core sensable functionality and data models.



