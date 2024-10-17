## Description


The `./gradlew` file is a Gradle wrapper script that allows users to run Gradle tasks without having to install Gradle on their system. It is a Bash script that sets up the environment and runs the Gradle wrapper main class.


## Usage instructions


**Step 1: Navigate to the project directory**
Navigate to the directory where the `./gradlew` file is located.

**Step 2: Run the Gradle wrapper**
Run the `./gradlew` command followed by the desired Gradle task, such as `./gradlew build` or `./gradlew clean`.

**Step 3: Configure the Gradle wrapper (optional)**
If needed, configure the Gradle wrapper by setting environment variables such as `JAVA_HOME` or `GRADLE_OPTS`.


## Implementation details


The `./gradlew` script performs the following tasks:

* Sets up the environment by determining the Java command to use and setting the classpath.
* Increases the maximum file descriptors if possible.
* Converts paths to Windows format if running on Cygwin.
* Runs the Gradle wrapper main class with the specified task and options.

The script uses the following functions and variables:

* `DEFAULT_JVM_OPTS`: a variable that sets default JVM options.
* `warn` and `die`: functions that print warning and error messages, respectively.
* `splitJvmOpts`: a function that splits JVM options into an array.
* `JAVACMD`: a variable that determines the Java command to use.
* `CLASSPATH`: a variable that sets the classpath.



