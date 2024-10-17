## Description

A directory containing adapter classes for the Sensable Android client. These adapters are used to bridge the gap between the data models and the user interface, providing a way to bind data to UI components.


## Adapters

The directory contains the following adapters:

* `ExpandableListAdapter`: an adapter for expandable lists, used to display a list of sensables with their corresponding samples.
* `TabsPagerAdapter`: an adapter for a pager that displays different tabs, used to navigate between local and remote sensables.


## Usage

These adapters are used in various activities and fragments throughout the client, such as `MainActivity`, `SensableActivity`, and `SensableListAdapter`. They are responsible for taking data from the data models and binding it to the UI components, making it easier to display and interact with the data.


## Dependencies

The adapters in this directory depend on the data models and UI components defined in other parts of the client. They also rely on the Android framework's adapter classes, such as `BaseExpandableListAdapter` and `PagerAdapter`.



