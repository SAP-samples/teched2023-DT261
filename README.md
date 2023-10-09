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

- [Getting Started](exercises/ex0/)
- [Exercise 1 - First Exercise Description](exercises/ex1/)
    - [Exercise 1.1 - Exercise 1 Sub Exercise 1 Description](exercises/ex1#exercise-11-sub-exercise-1-description)
    - [Exercise 1.2 - Exercise 1 Sub Exercise 2 Description](exercises/ex1#exercise-12-sub-exercise-2-description)
- [Exercise 2 - Second Exercise Description](exercises/ex2/)
    - [Exercise 2.1 - Exercise 2 Sub Exercise 1 Description](exercises/ex2#exercise-21-sub-exercise-1-description)
    - [Exercise 2.2 - Exercise 2 Sub Exercise 2 Description](exercises/ex2#exercise-22-sub-exercise-2-description)

  
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

### Batch Identification 
#### Create a Job to Identify Relevant SAP Notes

This option allows you to search and identify all SAP Notes based on SAP Notes type and its released date. Using this option, you can also either schedule a job immediately or select later dates for scheduled implementation. Please follow the below steps to schedule a job to identify SAP Notes.

1.	Go to transaction SNOTE to launch ‘Note Assistant – Home’ screen.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1612939f-4e89-4a40-8609-acde33a2aa91)


2.	In ‘Note Assistant – Home’ screen, navigate to the menu option ‘Batch Processing -> Batch Identification’.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/64177b57-8cd9-4aa1-94bd-32037c47315a)


3.	You would have navigated to ‘Schedule SAP Notes Batch Identification’ screen. This is where you would need to provide the search criteria, date selection, and schedule a job for immediate or future run. 
    Please provide the below details:
    Select radio button ‘Custom Search’.
    Search Term: *
    Search Range: All
    Application component: BC-UPG-DTM-TLA
    Date Range: Free Date Range: from 25.05.2023to 10.09.2023
    Job/Schedule Description: Batch_Identification_<your laptop/desk number>
    Select radio button ‘Schedule Immediately’.

    Once all of this is filled, click on the button ‘Confirm Schedule’ to schedule the batch job, which will identify SAP Notes (along with its required pre-requisite SAP Notes) matching this search criteria valid for this SAP system.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/80a651e5-8142-4f07-970e-d7784dbc2937)

 
4.	Well done, you just created your first Batch Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/33b78ad8-a899-41f8-b956-0f645e7792d8)
 

You can now continue with the next exercise – Implement the identified SAP Notes in a batch job.
 

#### Implement the identified SAP Notes in a batch Job

In the previous steps, you have scheduled a job which will identify SAP Notes based on a certain search criterion. Now, we will view the results and take the next steps to set up a batch job for Note implementation.  
1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/8f2b2df9-7fe5-4f89-9d76-5a9abd300448)

 

2.	In case the job has not completed yet, wait for the job to be completed. You can use the refresh button at the top to update the job status. Once the job is completed, on the rightmost column, you will find a button ‘Confirm pre-requisites’ against the Run ID. You may have to expand the tree to view the Run ID details. 
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/826a5192-f9d0-44ff-9c58-fc99a3c7a3c1)
 

3.	You will be navigated to another screen which displays the list of identified SAP Notes along with its pre-requisite SAP Notes in a tree format. 

    Some of the SAP Notes which are not yet downloaded will have the status as ‘Undefined Implementation State’. This is fine and the status will be calculated once the SAP Notes are downloaded.

    Keep the checkboxes against the SAP Notes (of type ‘Input Note’) 3337910 and 3336633 checked and uncheck all other checkboxes all other Input Notes.

    Click on the button ‘Download and Implement’.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/681552bf-c1a4-4856-8eb4-b420c469856d)

 



4.	In a pop-up, you will be prompted to provide a transport request. Use the ‘Create Request’ option to create a new transport request.
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b87b8cc1-3a01-4f23-98f9-5cffb46933d8)


5.	Provide Short Description as ‘Batch_Impl_<your laptop/desk number>’. Click on the save button. This will create a new transport request.
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1f8f27f7-c5de-476b-93ad-e1cc232d8eb2)


6.	The newly created transport request will be filled now. Choose the ‘Ok’ button to continue.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/39ed545b-e2c1-444d-8792-2b3104df9523)


7.	You have just created a Note Implementation job using the results of the Note Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/495718dd-1e64-4d29-9bb5-b91497e2d79c)


8.	Once the job is completed (if necessary, use the ‘refresh’ button to update the status in the Batch Dashboard), you can now continue with the next exercise – Displaying the Implementation Results.
 
#### Viewing the Implementation Results
In the previous steps, you have scheduled a job which will implement SAP Notes based on the results of note identification. Now, we will view the implementation results.

1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step. Locate the Run for Schedule type ‘Note implementation’. You will find a button ‘Implementation Result’ corresponding to this Run. Click on the button.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/9142ba0a-227a-4ee5-8369-3da1b6b8220c)


2.	You would have navigated to the ‘SAP Note Batch Implementation Results’ screen. 

    This screen shows all the SAP Notes processed by the batch job. You will find the implementation statuses of the SAP Notes and information/error messages, if any, against each SAP Note.

    Use the checkbox to select a line for any SAP Note which is completely implemented. 

    Click on the button ‘Note Log’ to view the implementation logs of the SAP Note.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b81c1cad-37a2-4fe7-8794-b16318eff939)

 

3.	Observe the results. Once done close the pop-up for Note Batch Implementation Logs
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/f3e17cb7-ac3a-490e-85f2-1849a6fe46f5)


4.	Keeping the checkbox for the same SAP Note selected, click on button ‘Object List’. This will show the list of objects processed by the SAP Note along with its simulation results.
   ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/41e93777-7c3d-4517-99aa-d1f9de8d3d87)


5.	Observe the results. Once done close the pop-up for SAP Note Batch Implementation Results.
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d727ed96-cef7-429b-b354-f0869ae27d9a)


You have now completed the exercise for Batch Identification. 

Please proceed with the next exercise – Batch Implementation.



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
