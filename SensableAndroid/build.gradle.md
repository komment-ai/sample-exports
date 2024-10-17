## Description

The `./build.gradle` file is a build configuration file for the SensableAndroid project. It is used by the Gradle build system to manage the project's dependencies, build settings, and compilation process. This file plays a crucial role in defining how the project is built, tested, and deployed.


## Usage instructions


* **Step 1: Configuring the build**\n The user needs to configure the build settings in the `build.gradle` file, such as the Android SDK version, build tools version, and dependencies.
* **Step 2: Specifying dependencies**\n The user needs to specify the project's dependencies, such as libraries and modules, in the `dependencies` block of the `build.gradle` file.
* **Step 3: Customizing the build process**\n The user can customize the build process by adding custom tasks, modifying the build configuration, and configuring the build variants.


## Implementation details


The `build.gradle` file is written in Groovy and uses the Gradle Domain Specific Language (DSL) to define the build configuration. The file is divided into several sections, including:

* `android`: This section defines the Android-specific build settings, such as the SDK version and build tools version.
* `dependencies`: This section specifies the project's dependencies, such as libraries and modules.
* `buildTypes`: This section defines the build variants, such as debug and release.
* `productFlavors`: This section defines the product flavors, such as different versions of the app for different markets.

Some notable functions and classes in the `build.gradle` file include:

* `android.defaultConfig`: This block defines the default build settings for the Android app.
* `dependencies.compile`: This block specifies the dependencies that are compiled into the app.
* `buildTypes.release`: This block defines the build settings for the release variant of the app.



