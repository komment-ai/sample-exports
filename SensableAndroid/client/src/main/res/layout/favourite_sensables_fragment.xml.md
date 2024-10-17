## Description

This XML file defines the layout for the FavouriteSensablesFragment in the SensableAndroid application. It is used to display a list of favourite sensables to the user. The layout consists of a RelativeLayout containing a TextView and a ListView. The TextView is used to display a message when there are no favourite sensables, and the ListView is used to display the list of favourite sensables.


## Usage instructions


* **Step 1: Inflate the layout**\n Inflate the layout in the FavouriteSensablesFragment's onCreateView method.
* **Step 2: Populate the ListView**\n Populate the ListView with the list of favourite sensables. This can be done by creating a custom adapter and setting it to the ListView.
* **Step 3: Handle empty list**\n Handle the case where there are no favourite sensables. This can be done by setting the visibility of the TextView to visible and displaying a message to the user.
* **Step 4: Customize the layout**\n Customize the layout as needed. This can include changing the background color, text color, and font size.


## Implementation details


The layout consists of the following elements:

* A RelativeLayout with a background color of #fa6a6a
* A TextView with the id "text_no_favourite" that is used to display a message when there are no favourite sensables
* A ListView with the id "saved_sensable_list" that is used to display the list of favourite sensables

The layout uses the following styles:

* The style "@style/SensableTextView" is used for the ListView

The layout uses the following strings:

* The string "@string/no_favourites" is used to display a message when there are no favourite sensables



