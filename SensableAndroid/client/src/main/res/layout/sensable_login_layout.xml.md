## Description

The `sensable_login_layout.xml` file is a user interface layout file used in the Sensable Android application. It defines the layout for the login screen, which includes input fields for username and password, as well as a submit button.


## Usage instructions

**Step 1: Access the login screen**
The login screen is accessed when the user attempts to log in to the Sensable application.

**Step 2: Enter username and password**
The user enters their username and password into the corresponding input fields.

**Step 3: Submit login credentials**
The user clicks the "Log in" button to submit their login credentials.

**Step 4: Authenticate and proceed**
If the login credentials are valid, the user is authenticated and proceeds to the main application.


## Implementation details

The layout is defined using a `LinearLayout` with a vertical orientation, containing two inner `LinearLayout`s for the username and password input fields, and a `Button` for submitting the login credentials.

* `LinearLayout`: The outer layout that contains the entire login screen.
* `LinearLayout` (inner): The layouts that contain the username and password input fields.
* `EditText`: The input fields for the username and password.
* `Button`: The submit button that triggers the login authentication process.

Note: The actual authentication process is not handled by this layout file, but rather by the corresponding Java code that interacts with this layout.

