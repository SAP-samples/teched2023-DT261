# Batch Identification 
In this exercise you will schedule a background job which will identify all SAP Notes based on a specific search criterion. You will then set up another job which will implement some of the identified SAP Notes. Finally, you will be viewing the results of the implementation.

## Create a Job to Identify Relevant SAP Notes

This option allows you to search and identify all SAP Notes based on SAP Notes type and its released date. Using this option, you can also either schedule a job immediately or select later dates for scheduled implementation. Please follow the below steps to schedule a job to identify SAP Notes.

1.	Go to transaction SNOTE to launch ‘Note Assistant – Home’ screen.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1612939f-4e89-4a40-8609-acde33a2aa91)


2.	In ‘Note Assistant – Home’ screen, navigate to the menu option ‘Batch Processing -> Batch Identification’.

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/64177b57-8cd9-4aa1-94bd-32037c47315a)


4.	You would have navigated to ‘Schedule SAP Notes Batch Identification’ screen. This is where you would need to provide the search criteria, date selection, and schedule a job for immediate or future run. 
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

 
6.	Well done, you just created your first Batch Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.

  	 ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/33b78ad8-a899-41f8-b956-0f645e7792d8)
 

You can now continue with the next exercise – Implement the identified SAP Notes in a batch job.
 

## Implement the identified SAP Notes in a batch Job

In the previous steps, you have scheduled a job which will identify SAP Notes based on a certain search criterion. Now, we will view the results and take the next steps to set up a batch job for Note implementation.  
1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step.

  	 ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/8f2b2df9-7fe5-4f89-9d76-5a9abd300448)

 
3.	In case the job has not completed yet, wait for the job to be completed. You can use the refresh button at the top to update the job status. Once the job is completed, on the rightmost column, you will find a button ‘Confirm pre-requisites’ against the Run ID. You may have to expand the tree to view the Run ID details. 

  	 ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/826a5192-f9d0-44ff-9c58-fc99a3c7a3c1)
 

5.	You will be navigated to another screen which displays the list of identified SAP Notes along with its pre-requisite SAP Notes in a tree format. 

    Some of the SAP Notes which are not yet downloaded will have the status as ‘Undefined Implementation State’. This is fine and the status will be calculated once the SAP Notes are downloaded.

    Keep the checkboxes against the SAP Notes (of type ‘Input Note’) 3337910 and 3336633 checked and uncheck all other checkboxes all other Input Notes.

    Click on the button ‘Download and Implement’.

  	 ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/681552bf-c1a4-4856-8eb4-b420c469856d)

 

7.	In a pop-up, you will be prompted to provide a transport request. Use the ‘Create Request’ option to create a new transport request.

  	  ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b87b8cc1-3a01-4f23-98f9-5cffb46933d8)


9.	Provide Short Description as ‘Batch_Impl_<your laptop/desk number>’. Click on the save button. This will create a new transport request.

  	  ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1f8f27f7-c5de-476b-93ad-e1cc232d8eb2)


11.	The newly created transport request will be filled now. Choose the ‘Ok’ button to continue.
  
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/39ed545b-e2c1-444d-8792-2b3104df9523)


12.	You have just created a Note Implementation job using the results of the Note Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.

   	  ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/495718dd-1e64-4d29-9bb5-b91497e2d79c)


14.	Once the job is completed (if necessary, use the ‘refresh’ button to update the status in the Batch Dashboard), you can now continue with the next exercise – Displaying the Implementation Results.
 
## Viewing the Implementation Results
In the previous steps, you have scheduled a job which will implement SAP Notes based on the results of note identification. Now, we will view the implementation results.

1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step. Locate the Run for Schedule type ‘Note implementation’. You will find a button ‘Implementation Result’ corresponding to this Run. Click on the button.

  	  ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/9142ba0a-227a-4ee5-8369-3da1b6b8220c)


3.	You would have navigated to the ‘SAP Note Batch Implementation Results’ screen. 

    This screen shows all the SAP Notes processed by the batch job. You will find the implementation statuses of the SAP Notes and information/error messages, if any, against each SAP Note.

    Use the checkbox to select a line for any SAP Note which is completely implemented. 

    Click on the button ‘Note Log’ to view the implementation logs of the SAP Note.

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b81c1cad-37a2-4fe7-8794-b16318eff939)

 

5.	Observe the results. Once done close the pop-up for Note Batch Implementation Logs

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/f3e17cb7-ac3a-490e-85f2-1849a6fe46f5)


7.	Keeping the checkbox for the same SAP Note selected, click on button ‘Object List’. This will show the list of objects processed by the SAP Note along with its simulation results.

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/41e93777-7c3d-4517-99aa-d1f9de8d3d87)


9.	Observe the results. Once done close the pop-up for SAP Note Batch Implementation Results.

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d727ed96-cef7-429b-b354-f0869ae27d9a)


You have now completed the exercise for Batch Identification. 

Please proceed with the next exercise – [Batch Implementation](../ex2/README.md).

