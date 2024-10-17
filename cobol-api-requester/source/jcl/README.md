## Description

The `./source/jcl/` directory contains Job Control Language (JCL) files, which are used to execute batch jobs on a mainframe computer. The JCL files in this directory are specifically designed to compile and run COBOL programs, define CICS (Customer Information Control System) resources, and manage VSAM (Virtual Storage Access Method) files.


## Contents

The directory contains the following JCL files:

* `compile.jcl`: Used to compile COBOL programs.
* `cicsdefn.jcl`: Defines CICS resources, such as transactions and programs.
* `vsam.jcl`: Manages VSAM files, including creating, updating, and deleting files.


## Usage

These JCL files are used to automate the process of compiling and running COBOL programs, as well as managing CICS resources and VSAM files. They are typically submitted to a mainframe job scheduler, such as JES (Job Entry Subsystem), to execute the batch jobs.


## Dependencies

The JCL files in this directory depend on the COBOL programs and CICS resources defined in other parts of the project.



