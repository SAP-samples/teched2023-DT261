[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2023-DT261)](https://api.reuse.software/info/github.com/SAP-samples/teched2023-DT261)

# DT261 - Ease SAP Notes Implementation in SAP S/4HANA Cloud and On-Premise Software

## Description

This repository contains the material for the SAP TechEd 2022 session called 'DT261 - Ease SAP Notes Implementation in SAP S/4HANA Cloud and On-Premise Software'.  

## Overview

Note assistant tool is now enhanced with features that enable us to schedule jobs to identify, implement, and view the activity summary of SAP Notes. To support these functionalities, you now have three new enhancements, which are batch identification, batch implementation, and batch dashboard. 

In this exercise, we will be creating batch jobs in SNOTE to identify and implement SAP Notes and view the results. We will also be using the Note Analyzer functionality to analyze a set of SAP Notes from an XML file provided as an attachment to an SAP Note. We will then be setting up a batch job to implement the necessary SAP Notes as per the analyser results.


## Requirements

The requirements to follow the exercises in this repository are...

## System and User Details

Server: nw757.tdc.sap.com

Instance: 00	

System ID: TE1

Login details:

Client : 001

User: DRYRUN

Password: dryrun

## Exercises

Provide the exercise content here directly in README.md using [markdown](https://guides.github.com/features/mastering-markdown/) and linking to the specific exercise pages, below is an example.

- [Login to System](exercises/ex0/)
- [Batch Identification](exercises/ex1/)
    - [Create a Job to Identify Relevant SAP Notes](exercises/ex1#create-a-job-to-identify-relevant-sap-notes)
    - [Implement the identified SAP Notes in a batch Job](exercises/ex1#implement-the-identified-sap-notes-in-a-batch-job)
    - [Viewing the Implementation Results](exercises/ex1##viewing-the-implementation-results)
- [Batch Implementation](exercises/ex2/)
    - [Adding SAP Notes for pre-requisite Identification and Note implementation in Batch Job](exercises/ex2#exercise-21-sub-exercise-1-description)
    - [Viewing the Implementation Results](exercises/ex2#exercise-22-sub-exercise-2-description)

  
**OR** Link to the Tutorial Navigator for example...

Start the exercises [here](https://developers.sap.com/tutorials/abap-environment-trial-onboarding.html).



### Login to System
1.	Open SAP Logon application from the laptop windows menu.
   
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/662f0c07-8f4e-4e71-a41e-799dfabd4c36)


2.	Use the ‘New -> Connection’ button to create a system:
   
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/e3d84316-1af5-47d2-8ebf-4d0b91ee1da5)
               

3.	Keeping the cursor on ‘User Specified System’, click on next:
   
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/e330763d-ee8c-443e-a479-7af5e068afbf)

 

4.	Fill the details as provided in the ‘System and User’ section of this document:
    Server: nw757.tdc.sap.com
    Instance: 00	
    System ID: TE1

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/46cbfa28-2786-4947-b266-5d24cac298f3)

 

5.	The added system will now appear in the list of systems:
   
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/5cece1d1-7b7b-43e5-8992-9cf7867cb966)

 

6.	Select the system and click on ‘Log On’. The login screen should appear. Provide the client and user details as provided in ‘System and User’ section of this document.
    Client : 001
    User: DRYRUN
    Password: dryrun

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/3a6381fc-8874-419c-9a9b-a98717571af5)

 
7.	You will be logged into the system now.



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
