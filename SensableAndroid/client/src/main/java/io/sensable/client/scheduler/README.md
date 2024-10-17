![Alt text](./README.md.svg)

## Description

A directory containing classes responsible for scheduling and managing scheduled sensables in the Sensable Android client application.


## Contents

The directory contains the following classes:

* `BootReceiver`: A broadcast receiver that listens for the device boot event and starts the scheduled sensable service.
* `ScheduledSensableService`: A service that runs in the background and manages scheduled sensables.
* `ScheduleHelper`: A utility class that provides helper methods for scheduling and managing scheduled sensables.


## Functionality

The classes in this directory work together to enable the scheduling of sensables, allowing users to configure their sensables to run at specific times or intervals. The `BootReceiver` ensures that the scheduled sensable service is started when the device boots, and the `ScheduledSensableService` runs in the background to manage the scheduled sensables. The `ScheduleHelper` provides utility methods for scheduling and managing scheduled sensables.


## Usage

The classes in this directory are used by the Sensable Android client application to provide scheduling functionality for sensables. The application uses the `ScheduleHelper` class to schedule sensables, and the `ScheduledSensableService` runs in the background to manage the scheduled sensables.



