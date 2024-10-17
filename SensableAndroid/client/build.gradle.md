## Description


The `./client/build.gradle` file is a Gradle build script for the Android client module of the SensableAndroid project. It defines the dependencies, build configuration, and other settings required to build the client module.


## Usage instructions


**Step 1: Configure the build environment**
 Ensure that you have the Android SDK and Gradle installed on your machine.

**Step 2: Update the build configuration (optional)**
 If necessary, update the `buildToolsVersion` and `compileSdkVersion` variables in the `android` block to match your desired Android SDK version.

**Step 3: Add dependencies**
 Add any additional dependencies required by your project to the `dependencies` block.

**Step 4: Build the project**
 Run the command `gradle build` in the terminal to build the client module.

**Step 5: Run the application**
 Run the command `gradle installDebug` to install the application on a connected device or emulator.


## Implementation details


The script applies the `android` plugin and configures the build settings for the client module. It also defines the dependencies for the module, including the `library` module and the Android support library.

* `buildscript`: Defines the repositories and dependencies for the build script itself.
* `android`: Configures the build settings for the client module, including the build tools version and compile SDK version.
* `dependencies`: Defines the dependencies for the client module, including the `library` module and the Android support library.
* `wrapper`: Configures the Gradle wrapper to use version 2.0.



