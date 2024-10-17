## Description

The `favourite_button.xml` file is a selector drawable that defines the appearance of a favourite button in different states. It is used in the Sensable Android application to provide visual feedback when a user interacts with a favourite button.


## Usage instructions

**Step 1: Add the favourite button to a layout**
Add the favourite button to a layout XML file using the `@drawable/favourite_button` attribute.

**Step 2: Define the favourite and favourite_pressed drawables**
Create the `favourite.png` and `favourite_pressed.png` drawables in the `res/drawable-hdpi` directory. These drawables will be used to display the favourite button in its normal and pressed states.

**Step 3: Use the favourite button in an activity or fragment**
In an activity or fragment, use the favourite button to toggle the favourite state of an item. The button will automatically display the correct drawable based on its state.


## Implementation details

The `favourite_button.xml` file uses a selector to define the appearance of the favourite button in different states. The selector contains four items:

* `android:state_focused="true" android:state_pressed="false"`: Displays the favourite drawable when the button is focused but not pressed.
* `android:state_focused="true" android:state_pressed="true"`: Displays the favourite_pressed drawable when the button is focused and pressed.
* `android:state_focused="false" android:state_pressed="true"`: Displays the favourite_pressed drawable when the button is not focused but pressed.
* Default: Displays the favourite drawable when the button is not focused and not pressed.

The favourite button uses the `@drawable/favourite` and `@drawable/favourite_pressed` attributes to reference the favourite and favourite_pressed drawables.



