## Description

The `gradle-wrapper.properties` file is a configuration file for the Gradle wrapper, a tool that allows you to use Gradle without having to install it on your system. This file specifies the version of Gradle to use, the location of the Gradle distribution, and other settings.


## Usage instructions

**Step 1: Configure the Gradle wrapper**
To use the Gradle wrapper, you need to configure it by specifying the version of Gradle to use and the location of the Gradle distribution. This is done in the `gradle-wrapper.properties` file.

**Step 2: Run the Gradle wrapper**
To run the Gradle wrapper, use the `gradlew` command (or `gradlew.bat` on Windows). This will download and install the specified version of Gradle if it is not already installed.

**Step 3: Use Gradle**
Once the Gradle wrapper is set up, you can use Gradle to build and manage your project. You can use the `gradlew` command to run Gradle tasks, such as `gradlew build` or `gradlew clean`.


## Implementation details

The `gradle-wrapper.properties` file contains the following settings:

* `distributionBase`: The base directory for the Gradle distribution.
* `distributionPath`: The directory where the Gradle distribution will be installed.
* `zipStoreBase`: The base directory for the Gradle zip store.
* `zipStorePath`: The directory where the Gradle zip store will be installed.
* `distributionUrl`: The URL of the Gradle distribution to download.

These settings are used by the Gradle wrapper to determine where to download and install the Gradle distribution.



