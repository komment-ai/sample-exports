## Description

The `./client/src/main/java/io/sensable/` directory contains Java source code for the client-side application of the SensableAndroid project. This directory is a part of the larger `client` module, which is responsible for providing a user interface and functionality for interacting with Sensable services.


## Package Structure

The directory is organized into several sub-packages, each containing related classes:

* `io.sensable.client`: Contains main application activities, such as `AboutActivity`, `MainActivity`, and `SensableActivity`.
* `io.sensable.client.adapter`: Holds adapter classes for displaying data in the user interface, including `ExpandableListAdapter` and `TabsPagerAdapter`.
* `io.sensable.client.component`: Contains custom UI components, such as `FontFitTextView`.
* `io.sensable.client.scheduler`: Includes classes for scheduling and managing Sensable services, including `BootReceiver`, `ScheduledSensableService`, and `ScheduleHelper`.
* `io.sensable.client.settings`: Holds configuration classes, such as `Config`.
* `io.sensable.client.sqlite`: Contains database-related classes, including `SensableContentProvider`, `SavedSensablesTable`, `ScheduledSensableContentProvider`, `SensableDatabaseHelper`, and `ScheduledSensablesTable`.
* `io.sensable.client.views`: Holds fragment classes for displaying different types of Sensable data, including `LocalSensablesFragment`, `RemoteSensablesFragment`, `SensableListAdapter`, and `FavouriteSensablesFragment`.


## Functionality

The classes in this directory work together to provide the following functionality:

* User interface and user experience for interacting with Sensable services
* Scheduling and management of Sensable services
* Data storage and retrieval using a SQLite database
* Display of Sensable data in various formats, including lists and fragments



