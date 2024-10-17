## Description

The `activity_about.xml` file is a layout file used in the SensableAndroid project to display the "About" page of the application. It contains the user interface elements for this page, including an image, a scrollable text view, and a text view for displaying statistics.


## Usage instructions


* **Step 1: Access the About page**\n The About page can be accessed by navigating to the corresponding menu item in the application.
* **Step 2: View the About page content**\n The page displays an image, a scrollable text view with information about the application, and a text view with statistics.
* **Step 3: Customize the About page content**\n The content of the About page can be customized by modifying the `about_text` string resource and the `about_statistics` text view.


## Implementation details


The layout file uses a `LinearLayout` with a vertical orientation to arrange the user interface elements. The elements include:

* An `ImageView` to display the application logo
* A `ScrollView` containing a `TextView` to display the About page text
* A `TextView` to display statistics

The layout file uses various resources, such as `@dimen/activity_horizontal_margin` and `@color/textColor`, to define the appearance of the user interface elements.



