![Alt text](./README.md.svg)

## Description

The `./client/src/main/java/io/sensable/client/sqlite/` directory contains SQLite database management classes for the Sensable Android client application. This directory is responsible for handling data storage and retrieval, providing a structured way to interact with the local database.


## Database Structure

The directory contains classes that define the database schema and provide functionality for creating, updating, and querying the database tables. The main database tables are:

* `SavedSensablesTable`: stores information about saved sensables
* `ScheduledSensablesTable`: stores information about scheduled sensables


## Content Provider

The `SensableContentProvider` class provides a content provider interface for accessing the database tables. This allows other parts of the application to interact with the database in a standardized way.


## Database Helper

The `SensableDatabaseHelper` class provides a helper class for creating and upgrading the database schema.


## Usage

The classes in this directory are used throughout the Sensable Android client application to store and retrieve data. For example, the `LocalSensablesFragment` uses the `SensableContentProvider` to retrieve a list of saved sensables.


## Dependencies

The classes in this directory depend on the Android SQLite API and the Sensable Android client application's data models.



