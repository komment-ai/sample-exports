## Description

The `activity_sensable.xml` file is a layout file used in the Sensable Android application to display the details of a single sensable. It defines the user interface for the SensableActivity, which is responsible for showing the sensable's ID, unit, location, and samples. The layout includes buttons for favouriting, unfavouriting, and deleting the sensable, as well as a list view to display the sensable's samples.


## Usage instructions


* **Step 1: Launch the SensableActivity**
 Launch the SensableActivity to view the details of a single sensable. This can be done by clicking on a sensable from the list of sensables in the MainActivity.
* **Step 2: View sensable details**
 The activity will display the sensable's ID, unit, and location. The user can view this information to understand the sensable's characteristics.
* **Step 3: View sensable samples**
 The activity will display a list of samples for the sensable. The user can scroll through the list to view the samples.
* **Step 4: Favourite or unfavourite the sensable**
 The user can click the favourite or unfavourite button to toggle the sensable's favourite status.
* **Step 5: Delete the sensable (optional)**
 If the sensable is local, the user can click the delete button to remove the sensable from the device.


## Implementation details

The layout file defines a linear layout with several components:

* A linear layout containing buttons for favouriting, unfavouriting, and deleting the sensable.
* Text views to display the sensable's ID, unit, and location.
* An ExpandableListView to display the sensable's samples.

The SensableActivity uses this layout to display the sensable's details and handle user interactions such as favouriting and deleting the sensable.



