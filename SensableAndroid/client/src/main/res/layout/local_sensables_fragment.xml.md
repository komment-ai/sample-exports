## Description

The `local_sensables_fragment.xml` file is a layout file used in the SensableAndroid project to display a list of local sensables. It is a fragment layout, meaning it is a reusable UI component that can be used in multiple activities.


## Usage instructions


* **Step 1: Create a new fragment**\n Create a new fragment in your activity to display the local sensables. You can do this by extending the `Fragment` class and overriding the `onCreateView` method.
* **Step 2: Inflate the layout**\n Inflate the `local_sensables_fragment.xml` layout in the `onCreateView` method using the `LayoutInflater`.
* **Step 3: Initialize the list view**\n Initialize the `ListView` in the layout and set its adapter to display the local sensables.
* **Step 4: Handle item clicks**\n Handle item clicks on the list view to perform actions when a local sensable is selected.


## Implementation details


The layout file defines a `RelativeLayout` with a `TextView` and a `ListView`. The `TextView` is used to display a message when there are no local sensables, and the `ListView` is used to display the list of local sensables.

The `ListView` has a custom style defined in the `SensableTextView` style, which is used to customize its appearance.

The layout file does not contain any complex logic or functions, but it is used in conjunction with the `LocalSensablesFragment` class to display the local sensables.



