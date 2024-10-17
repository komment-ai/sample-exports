## Description

The `saved_sensables.xml` file is a menu resource file for the Android application. It defines a menu that can be used in the `SavedSensablesActivity` to provide options for the user to interact with the application. The menu includes options to view information about the application, log out, log in, and create a new sensable.


## Usage instructions


* **Step 1: Access the SavedSensablesActivity**\n The user must navigate to the `SavedSensablesActivity` in the application to access the menu defined in this file.
* **Step 2: Open the menu**\n The user can open the menu by clicking on the menu button or by using the menu key on their device.
* **Step 3: Select an option**\n The user can select one of the options from the menu to perform the corresponding action.


## Implementation details

The menu is defined using XML and includes four items:

* `action_about`: Displays information about the application.
* `action_logout`: Logs the user out of the application.
* `action_login`: Logs the user into the application.
* `action_create`: Creates a new sensable.

Each item has a title and an ID, and can be shown as an action in the action bar or as a menu item. The `orderInCategory` attribute is used to determine the order in which the items are displayed in the menu.



