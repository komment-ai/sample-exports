## Description

The `sensableStyle.xml` file is a resource file that defines the visual style and layout of the Sensable Android application. It contains styles, themes, and layouts that are used throughout the app to maintain a consistent look and feel.


## Usage instructions


*   **Step 1: Include the style in your layout**\n To use the styles defined in this file, you need to include them in your layout XML files. For example, you can set the `style` attribute of a `TextView` to `@style/SensableTextView`.
*   **Step 2: Customize the style**\n You can customize the styles defined in this file by overriding the values in your own styles.xml file. For example, you can change the `textColor` attribute of the `SensableTextView` style to use a different color.
*   **Step 3: Apply the theme**\n To apply the theme defined in this file to your entire app, you need to set the `android:theme` attribute in your AndroidManifest.xml file to `@style/SensableStyle`.


## Implementation details


The file defines several styles and themes that are used in the Sensable Android application. These include:

*   `SensableStyle`: The main theme of the app, which defines the overall look and feel.
*   `SensableActionBar`: A style for the action bar, which defines its background color and other attributes.
*   `SensableDialogTheme`: A theme for dialogs, which defines the text color and other attributes.
*   `SensableTextView`: A style for text views, which defines the text color and other attributes.

The styles and themes defined in this file use various attributes and resources, such as colors and drawables, which are defined in other files in the project. For example, the `SensableStyle` theme uses the `mainBackground` color, which is defined in the `colors.xml` file.



