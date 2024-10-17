## Description

The file `./library/src/main/res/drawable-hdpi-v11/ic_stat_rocket.png` is a high-density image file used in the project to represent a rocket icon. It is part of the SensableAndroid library and is used to display a notification icon on Android devices with high-density displays (hdpi). The image is a variant of the rocket icon, specifically designed for Android 3.0 (API level 11) and later versions.


## Implementation details

This image file is a PNG (Portable Network Graphics) file, which is a raster graphics file format that supports lossless data compression. The file is stored in the `res/drawable-hdpi-v11` directory, which indicates that it is intended for use on high-density devices with Android 3.0 or later.

The image is used in conjunction with other variants of the rocket icon, which are stored in different directories (e.g., `drawable-xhdpi-v11`, `drawable-xxhdpi-v11`, etc.) to provide support for different screen densities and Android versions. The use of these variant images allows the app to display the correct icon size and resolution on different devices.


## Usage instructions

This file is not intended to be used directly by developers. Instead, it is used by the Android system to display a notification icon when the app is running in the background. To use this icon in an Android app, developers should follow these steps:

*   **Step 1: Add the image file to the project**
    Add the `ic_stat_rocket.png` file to the `res/drawable-hdpi-v11` directory in the project.
*   **Step 2: Configure the notification icon**
    In the app's `AndroidManifest.xml` file, specify the `ic_stat_rocket.png` file as the notification icon using the `android:icon` attribute.
*   **Step 3: Test the notification icon**
    Run the app on a high-density device with Android 3.0 or later to verify that the notification icon is displayed correctly.



