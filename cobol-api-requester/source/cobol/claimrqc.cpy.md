## Description

The `claimrqc.cpy` file is a COBOL copybook that defines the structure of a request claim container for the CICS Claims Application. It contains a set of predefined fields that make up a claim request, including the claim ID, type, amount, date, description, and provider. This copybook is used to define the layout of the claim request data that is exchanged between different components of the application.


## Usage instructions


**Step 1: Include the copybook in your COBOL program**

To use the `claimrqc.cpy` copybook, you need to include it in your COBOL program using the `COPY` statement. For example:
```
COPY claimrqc.
```
**Step 2: Define the claim request data**

Once you have included the copybook, you can define the claim request data using the predefined fields. For example:
```
MOVE 'CLAIM001' TO REQ-CLAIM-ID
MOVE 'MEDICAL' TO REQ-CLAIM-TYPE
MOVE 100.00 TO REQ-CLAIM-AMOUNT
```
**Step 3: Use the claim request data in your program**

You can then use the claim request data in your program as needed. For example, you can use it to send a request to a CICS server or to store it in a database.


## Implementation details


The `claimrqc.cpy` copybook defines a single record layout, `REQ-CLAIM-CONTAINER`, which contains two main fields: `REQ-CLAIM-RECORD` and `REQ-CLAIM-ACTION`. The `REQ-CLAIM-RECORD` field contains several subfields that define the details of the claim request, including the claim ID, type, amount, date, description, and provider. The `REQ-CLAIM-ACTION` field contains a single character that indicates the action to be taken on the claim request.

- `REQ-CLAIM-ID`: A field that contains the claim ID, which is an 8-character alphanumeric value.
- `REQ-CLAIM-TYPE`: A field that contains the claim type, which is an 8-character alphanumeric value.
- `REQ-CLAIM-AMOUNT`: A field that contains the claim amount, which is a 2-byte signed integer.
- `REQ-CLAIM-DATE`: A field that contains the claim date, which is a 10-character date value in the format `YYYY-MM-DD`.
- `REQ-CLAIM-DESC`: A field that contains the claim description, which is a 21-character alphanumeric value.
- `REQ-CLAIM-PROVIDER`: A field that contains the claim provider, which is a 21-character alphanumeric value.
- `REQ-CLAIM-ACTION`: A field that contains the action to be taken on the claim request, which is a single character value.



