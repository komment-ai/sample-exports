## Description

A notification icon image used in the Sensable Android application for devices with extra-high-density screens (xhdpi) running Android 3.0 or higher (v11). The image is a rocket icon used to represent the application in the notification bar.


## Implementation details

The image is a PNG file with a specific size and density to match the requirements of xhdpi devices running Android 3.0 or higher. It is designed to be used as a notification icon, which is displayed in the notification bar when the application is running in the background.


## Usage instructions

This file is not intended to be used directly by the end-user. Instead, it is used by the Android application to display a notification icon in the notification bar. The application will automatically select the correct icon based on the device's screen density and Android version.

However, developers working on the Sensable Android application can use this file by including it in their project's resources and referencing it in their code. For example, they can use the following code to set the notification icon:
```java
NotificationCompat.Builder builder = new NotificationCompat.Builder(context);
builder.setSmallIcon(R.drawable.ic_stat_rocket);
```
In this example, `R.drawable.ic_stat_rocket` refers to the `ic_stat_rocket.png` file in the `drawable-xhdpi-v11` directory.


## Notes

This file is one of several notification icon images used in the Sensable Android application, each with a different size and density to match the requirements of different devices. The application will automatically select the correct icon based on the device's screen density and Android version.



