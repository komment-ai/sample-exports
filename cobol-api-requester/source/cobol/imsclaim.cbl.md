![Alt text](./imsclaim.cbl.md.svg)

## Description
The `imsclaim.cbl` file is a COBOL program that serves as an IMS (Information Management System) application. It is designed to call an external REST API to evaluate claims based on business rules. The program uses the z/OS Connect EE API Requester function to make the API call. It processes input messages from a queue, calls the API, and then returns the output message to the queue.

## Usage instructions

**Step 1: Configure the IMS environment**

Configure the IMS environment to include the necessary resources, such as the queue and the API endpoint.

**Step 2: Compile and link the program**

Compile and link the `imsclaim.cbl` program using the COBOL compiler and linker.

**Step 3: Run the program**

Run the program as an IMS application, passing the necessary parameters, such as the queue name and the API endpoint.

**Step 4: Process input messages**

The program will process input messages from the queue, calling the API for each message.

**Step 5: Return output messages**

The program will return the output messages to the queue, including the result of the API call.

## Implementation details

The program uses the following functions and variables:

* `CALL-API`: A routine that calls the API using the z/OS Connect EE API Requester function.
* `GET-INPUT-MESSAGE`: A routine that gets the input message from the queue.
* `SET-OUTPUT-MESSAGE`: A routine that sets the output message to the queue.
* `LOG-MESSAGE`: A routine that logs messages to STDOUT.
* `BAQ-REQUEST-PTR` and `BAQ-RESPONSE-PTR`: Pointers to the request and response data structures.
* `BAQ-REQUEST-LEN` and `BAQ-RESPONSE-LEN`: The lengths of the request and response data structures.

The program uses the following copybooks:

* `BAQRINFO`: A copybook that defines the z/OS Connect EE API Requester function.
* `CLAIMREQ` and `CLAIMRSP`: Copybooks that define the request and response data structures.
* `CLAIMINF`: A copybook that defines the API info data structure.
* `IMSCLAIC`: A copybook that defines the IMS claim data structure.

DIAGRAM:YES