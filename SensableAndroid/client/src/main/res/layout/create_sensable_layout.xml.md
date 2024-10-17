## Description

The `create_sensable_layout.xml` file is a user interface layout file for the Sensable Android application. It defines the layout for a screen that allows users to create a new Sensable, which is a device sensor that can be used to collect data. The layout includes a spinner to select the device sensor, a text field to enter the Sensable ID, and a button to create the Sensable.


## Usage instructions


* **Step 1: Open the Create Sensable screen**\n The user must navigate to the Create Sensable screen in the Sensable Android application.
* **Step 2: Select a device sensor**\n The user must select a device sensor from the spinner dropdown menu. The available options are determined by the device's hardware capabilities.
* **Step 3: Enter the Sensable ID**\n The user must enter a unique ID for the Sensable in the text field.
* **Step 4: Create the Sensable**\n The user must click the "Create Sensable" button to create the new Sensable.


## Implementation details


The layout file defines a vertical `LinearLayout` with several child elements:

* A `TextView` that displays a prompt to select a device sensor.
* A `Spinner` that allows the user to select a device sensor.
* A horizontal `LinearLayout` that contains a `TextView` and an `EditText` for entering the Sensable ID.
* A `Button` that creates the new Sensable when clicked.

The layout file uses Android's XML layout syntax to define the user interface elements and their properties. The `android:layout_width` and `android:layout_height` attributes are used to specify the size of each element, while the `android:layout_gravity` attribute is used to specify the alignment of the elements within their parent layout.



