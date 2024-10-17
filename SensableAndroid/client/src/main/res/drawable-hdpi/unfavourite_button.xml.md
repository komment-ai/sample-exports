## Description

The `unfavourite_button.xml` file is a drawable resource that defines the appearance of an "unfavourite" button in the Sensable Android application. The button's appearance changes depending on its state, such as when it is focused or pressed.


## Usage instructions


* **Step 1: Include the button in a layout**\n Include the `unfavourite_button.xml` drawable in a layout file, such as `favourite_sensables_fragment.xml`, to display the button.
* **Step 2: Set the button's state**\n Use the `android:state_focused` and `android:state_pressed` attributes to set the button's state, which will change its appearance accordingly.
* **Step 3: Use the button in an activity or fragment**\n Use the layout file that includes the `unfavourite_button.xml` drawable in an activity or fragment, such as `FavouriteSensablesFragment`.


## Implementation details


The `unfavourite_button.xml` file uses a `selector` element to define the button's appearance in different states. The `selector` element contains four `item` elements, each specifying a different state and the corresponding drawable to display.

* `<item android:state_focused="true" android:state_pressed="false" android:drawable="@drawable/unfavourite" />`: Displays the `unfavourite` drawable when the button is focused but not pressed.
* `<item android:state_focused="true" android:state_pressed="true" android:drawable="@drawable/unfavourite_pressed" />`: Displays the `unfavourite_pressed` drawable when the button is focused and pressed.
* `<item android:state_focused="false" android:state_pressed="true" android:drawable="@drawable/unfavourite_pressed" />`: Displays the `unfavourite_pressed` drawable when the button is not focused but pressed.
* `<item android:drawable="@drawable/unfavourite" />`: Displays the `unfavourite` drawable when the button is not focused and not pressed.



