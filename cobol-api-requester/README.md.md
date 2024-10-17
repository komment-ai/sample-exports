## Description
The file `./README.md` is a markdown file that provides an overview of the project and instructions for how to run it. It serves as the main entry point for users to understand the project's purpose, prerequisites, installation, configuration, and testing.

## Usage instructions

**Step 1: Clone the repository**

 Clone the repository using the command `git clone git@github.com:zosconnect/zosconnect-sample-cobol-apirequester.git`

**Step 2: Allocate a PDS**

 Allocate a PDS with 30 tracks for the jobs and sample source files.

**Step 3: Upload source and sample JCLs**

 Upload the following source and sample JCLs to your z/OS system and store on the PDS that was allocated:
```
claimci0.cbl
claiminf.cpy
claimreq.cpy
claimrqc.cpy
claimrsc.cpy
claimrsp.cpy
cicsdefn.jcl
compile.jcl
vsam.jcl
```

**Step 4: Customize and submit JCLs**

 Customize the uploaded copy of `compile.jcl`, `vsam.jcl`, and `ciscdefn.jcl` for your environment and submit to compile the sample CICS COBOL program, define the VSAM data set, and define the CICS resources.

**Step 5: Configure z/OS Connect EE**

 Create the necessary directories and configure the z/OS Connect EE server to access the CICS region and call the health insurance claim REST API.

**Step 6: Deploy the sample API**

 Deploy the sample API, service, and API requester archive files to the z/OS Connect EE server.

**Step 7: Test the sample API**

 Test the sample API using the z/OS Connect EE API Editor or `curl` to verify that it is working correctly.

## Implementation details

The `README.md` file provides a detailed explanation of the project's purpose, prerequisites, installation, configuration, and testing. It includes instructions for cloning the repository, allocating a PDS, uploading source and sample JCLs, customizing and submitting JCLs, configuring z/OS Connect EE, deploying the sample API, and testing the sample API.

## Notice

&copy; Copyright IBM Corporation 2020

## License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

DIAGRAM:NO