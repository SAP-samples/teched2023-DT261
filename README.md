[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2023-DT261)](https://api.reuse.software/info/github.com/SAP-samples/teched2023-DT261)

# DT261 - Ease SAP Notes Implementation in SAP S/4HANA Cloud and On-Premise Software

## Description

This repository contains the material for the SAP TechEd 2022 session called 'DT261 - Ease SAP Notes Implementation in SAP S/4HANA Cloud and On-Premise Software'.  

## Overview

Note assistant tool is now enhanced with features that enable us to schedule jobs to identify, implement, and view the activity summary of SAP Notes. To support these functionalities, you now have three new enhancements, which are batch identification, batch implementation, and batch dashboard. 

In this exercise, we will be creating batch jobs in SNOTE to identify and implement SAP Notes and view the results. We will also be using the Note Analyzer functionality to analyze a set of SAP Notes from an XML file provided as an attachment to an SAP Note. We will then be setting up a batch job to implement the necessary SAP Notes as per the analyser results.



## System and User Details

System Details:

    Server: nw757.tdc.sap.com

    Instance: 00	

    System ID: TE1

Login details:

    Client : 001

    User: DRYRUN

    Password: dryrun

## Exercises

- [Login to System](exercises/ex0/)
- [Exercise 1: Batch Identification](exercises/ex1/)
    - [Exercise 1.1: Create a Job to Identify Relevant SAP Notes](exercises/ex1#exercise-11-create-a-job-to-identify-relevant-sap-notes)
    - [Exercise 1.2: Implement the identified SAP Notes in a batch Job](exercises/ex1#exercise-12-implement-the-identified-sap-notes-in-a-batch-job)
    - [Exercise 1.3: Viewing the Implementation Results](exercises/ex1#exercise-13-viewing-the-implementation-results)
- [Exercise 2: Batch Implementation](exercises/ex2/)
    - [Exercise 2.1: Adding SAP Notes for pre-requisite Identification and Note implementation in Batch Job](exercises/ex2#exercise-21-adding-sap-notes-for-pre-requisite-identification-and-note-implementation-in-batch-job)
    - [Exercise 2.2: Viewing the Implementation Results](exercises/ex2#exercise-22-viewing-the-implementation-results)
- [Exercise 3: SAP Note Analysis and Batch Implementation using Note Analyzer](exercises/ex3%20/README.md#exercise-3-sap-note-analysis-and-batch-implementation-using-note-analyzer)
    - [Exercise 3.1: Launch Note Analyzer](exercises/ex3%20/README.md#exercise-31-launch-note-analyzer)
    - [Exercise 3.2: Analyze SAP Note](exercises/ex3%20/README.md#exercise-32-analyze-sap-note)
        - [Exercise 3.2.1: Download XML File from Support Launch Pad](exercises/ex3%20/README.md#exercise-321-download-xml-file-from-support-launch-pad)
        - [Exercise 3.2.2: Upload the XML](exercises/ex3%20/README.md#exercise-322-upload-the-xml)
        - [Exercise 3.2.3: Analyze the Uploaded XML](exercises/ex3%20/README.md#exercise-323-analyze-the-uploaded-xml)
    - [Exercise 3.3: Conclusion](exercises/ex3%20/README.md#exercise-33-conclusion)       


Start the exercises [here](exercises/ex0/).


**IMPORTANT**

Your repo must contain the .reuse and LICENSES folder and the License section below. DO NOT REMOVE the section or folders/files. Also, remove all unused template assets(images, folders, etc) from the exercises folder. 

## Contributing
Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) to understand the contribution guidelines.

## Code of Conduct
Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
