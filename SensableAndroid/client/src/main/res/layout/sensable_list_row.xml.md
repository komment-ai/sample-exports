## Description

The `sensable_list_row.xml` file is a layout file for an Android application, specifically designed to represent a single row in a list of sensable devices. It defines the visual structure and layout of the row, including the type of sensable, its name, ID, and sample value with unit.


## Usage instructions


* **Step 1: Inflate the layout** Inflate the `sensable_list_row.xml` layout in your Android application to create a View object that represents a single row in the list.
* **Step 2: Set the sensable data** Set the data for the sensable device, including its type, name, ID, and sample value with unit, using the corresponding TextViews and ImageView in the layout.
* **Step 3: Add the row to the list** Add the inflated and populated View object to a ListView or RecyclerView in your Android application to display the sensable device in the list.


## Implementation details

The `sensable_list_row.xml` layout consists of a LinearLayout with a horizontal orientation, containing several child views:

* An ImageView to display the type of sensable device
* A TextView to display the name of the sensable device
* A TextView to display the ID of the sensable device
* A RelativeLayout to display the sample value and unit of the sensable device
* A FontFitTextView to display the sample value with a bold font style
* A TextView to display the unit of the sample value

The layout uses various attributes and styles to customize the appearance of the views, including margins, padding, and text appearance.



