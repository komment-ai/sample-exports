## Description

A directory containing configuration files for the Gradle wrapper, which is used to manage the Gradle build tool.


## Contents

The directory contains two files:

* `gradle-wrapper.jar`: a JAR file that contains the Gradle wrapper implementation
* `gradle-wrapper.properties`: a properties file that configures the Gradle wrapper, specifying the Gradle version and distribution URL


## Purpose

The Gradle wrapper is used to ensure that the project is built with a consistent version of Gradle, regardless of the version installed on the developer's machine. The wrapper downloads and installs the specified version of Gradle if it is not already present.


## Configuration

The `gradle-wrapper.properties` file can be edited to change the Gradle version or distribution URL. However, this is not recommended unless you have a specific reason to do so, as it can affect the build process.



