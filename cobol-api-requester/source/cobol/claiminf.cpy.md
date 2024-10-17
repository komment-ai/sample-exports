## Description

The `claiminf.cpy` file is a COBOL copybook that defines a set of constants and variables used in the CICS application. Specifically, it contains definitions for API-related information, such as API names, paths, and methods.


## Usage instructions


**Step 1: Include the copybook in your COBOL program**

To use the definitions in this copybook, include it in your COBOL program using the `COPY` statement.

**Step 2: Use the defined variables and constants**

Once the copybook is included, you can use the defined variables and constants in your program. For example, you can use the `BAQ-APINAME` variable to access the API name.

**Step 3: Modify the copybook as needed**

If you need to change the API-related information, you can modify the copybook accordingly. However, be sure to update all programs that use the copybook to reflect the changes.


## Implementation details


The copybook defines the following variables and constants:

* `BAQ-APINAME`: The API name.
* `BAQ-APINAME-LEN`: The length of the API name.
* `BAQ-APIPATH`: The API path.
* `BAQ-APIPATH-LEN`: The length of the API path.
* `BAQ-APIMETHOD`: The API method.
* `BAQ-APIMETHOD-LEN`: The length of the API method.

These definitions are used to provide a standardized way of accessing API-related information throughout the application.



