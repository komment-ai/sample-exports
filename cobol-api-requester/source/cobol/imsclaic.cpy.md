## Description
The `imsclaic.cpy` file is a COBOL copybook that defines the structure of input and output data for a CICS application. It contains two main data areas: `INPUT-MSG` and `OUTPUT-MSG`, which represent the format of terminal input and output messages, respectively. The copybook is used to define the layout of data exchanged between the application and the terminal.

## Usage instructions

**Step 1: Include the copybook in your COBOL program**

To use the `imsclaic.cpy` copybook, include it in your COBOL program using the `COPY` statement. For example:
```
COPY imsclaic.cpy
```
**Step 2: Define the input and output areas**

Define the `INPUT-MSG` and `OUTPUT-MSG` areas in your COBOL program using the `01` level number. For example:
```
01 INPUT-MSG.
   05  IN-LL               PIC S9(3) COMP.
   05  IN-ZZ               PIC S9(3) COMP.
   ...
01 OUTPUT-MSG.
   05  OUT-LL              PIC S9(3) COMP VALUE +0.
   05  OUT-ZZ              PIC S9(3) COMP VALUE +0.
   ...
```
**Step 3: Use the input and output areas in your program**

Use the `INPUT-MSG` and `OUTPUT-MSG` areas to read and write data to the terminal. For example:
```
READ INPUT-MSG FROM TERMINAL
...
WRITE OUTPUT-MSG TO TERMINAL
```
**Step 4: Validate the input data**

Validate the input data in the `INPUT-MSG` area to ensure it conforms to the expected format. For example:
```
IF IN-LL NOT NUMERIC
   DISPLAY "Invalid input: LL must be numeric"
   STOP RUN
```
## Implementation details

The `imsclaic.cpy` copybook defines two main data areas:

* `INPUT-MSG`: represents the format of terminal input messages
* `OUTPUT-MSG`: represents the format of terminal output messages

Each data area contains several fields, including:

* `IN-LL` and `OUT-LL`: length of the input/output message
* `IN-ZZ` and `OUT-ZZ`: filler fields
* `IN-TRANCODE` and `OUT-CLAIM-TYPE`: transaction code and claim type
* `IN-CLAIM-DATE` and `OUT-CLAIM-STATUS`: claim date and status
* `IN-CLAIM-AMOUNT` and `OUT-CLAIM-AMOUNT`: claim amount
* `IN-CLAIM-DESC` and `OUT-CLAIM-DESC`: claim description
* `OUT-MESSAGE`: output message

DIAGRAM:NO