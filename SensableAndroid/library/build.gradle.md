## Description

The `./library/build.gradle` file is a Gradle build script for the Android library module in the SensableAndroid project. It specifies the build configuration, dependencies, and tasks for the library module. This file plays a crucial role in building and packaging the library module, which is then used by the client module.


## Implementation details


The script applies the `android-library` plugin and sets the build tools version and compile SDK version. It also disables the `InvalidPackage` lint check.

The script specifies the following dependencies:

* `com.android.support:support-v4:19.1.0`
* `com.squareup.retrofit:retrofit:1.6.0`
* `com.squareup.okhttp:okhttp-urlconnection:2.0.0`
* `com.squareup.okhttp:okhttp:2.0.0`

These dependencies are used by the library module to provide functionality such as networking and data storage.

The script also defines a `wrapper` task that sets the Gradle version to `2.0`.


## Usage instructions


**Note:** This file is a build script and is not intended to be used directly. Instead, it is used by the Gradle build system to build and package the library module.

However, if you need to modify the build configuration or dependencies, you can do so by editing this file. Here are some general steps:

**Step 1: Modify the build configuration**
Modify the `buildToolsVersion` and `compileSdkVersion` properties to change the build configuration.

**Step 2: Add dependencies**
Add new dependencies by adding lines to the `dependencies` block. For example:
```groovy
compile 'com.example:my-library:1.0.0'
```
**Step 3: Remove dependencies**
Remove dependencies by deleting lines from the `dependencies` block.

**Step 4: Update the Gradle version**
Update the Gradle version by modifying the `gradleVersion` property in the `wrapper` task.



