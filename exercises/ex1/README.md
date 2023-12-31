# Exercise 1: Batch Identification 
In this exercise you will schedule a background job which will identify all SAP Notes based on a specific search criterion. You will then set up another job which will implement some of the identified SAP Notes. Finally, you will be viewing the results of the implementation.

## Exercise 1.1: Create a Job to Identify Relevant SAP Notes

This option allows you to search and identify all SAP Notes based on SAP Notes type and its released date. Using this option, you can also either schedule a job immediately or select later dates for scheduled implementation. Please follow the below steps to schedule a job to identify SAP Notes.

1.	Go to transaction SNOTE to launch ‘Note Assistant – Home’ screen.

    ![ex_01_02](images/1.1_1.png)


2.	In ‘Note Assistant – Home’ screen, navigate to the menu option ‘Batch Processing -> Batch Identification’.

  	![ex_01_02](images/1.1_2.png)


3.	You would have navigated to ‘Schedule SAP Notes Batch Identification’ screen. This is where you would need to provide the search criteria, date selection, and schedule a job for immediate or future run. 
    Please provide the below details:
  	
    - Select radio button _‘Custom Search’_.

  	- Search Term: _*_

    - Search Range: _All_

  	- Application component: _BC-UPG-DTM-TLA_

  	- Date Range: Free Date Range: from _25.05.2023_ to _10.09.2023_

  	- Job/Schedule Description: _Batch_Identification_<your laptop/desk number>_

  	- Select radio button _‘Schedule Immediately’_.

    Once all of this is filled, click on the button ‘Confirm Schedule’ to schedule the batch job, which will identify SAP Notes (along with its required pre-requisite SAP Notes) matching this search criteria valid for this SAP system.

  	 ![ex_01_02](images/1.1_3.png)

 
4.	Well done, you just created your first Batch Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.

  	 ![ex_01_02](images/1.1_4.png)
 

You can now continue with the next exercise – [Implement the identified SAP Notes in a batch Job](exercises/ex1#implement-the-identified-sap-notes-in-a-batch-job).
 

## Exercise 1.2: Implement the identified SAP Notes in a batch Job

In the previous steps, you have scheduled a job which will identify SAP Notes based on a certain search criterion. Now, we will view the results and take the next steps to set up a batch job for Note implementation.  
1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step.

  	 ![ex_01_02](images/1.2_1.png)

 
2.	In case the job has not completed yet, wait for the job to be completed, this can take 2-3 minutes. You can use the refresh button at the top to update the job status. Once the job is completed, on the rightmost column, you will find a button ‘Confirm pre-requisites’ against the Run ID. You may have to expand the tree to view the Run ID details. 

  	 ![ex_01_02](images/1.2_2.png)
 

3.	You will be navigated to another screen which displays the list of identified SAP Notes along with its pre-requisite SAP Notes in a tree format. 

    Some of the SAP Notes which are not yet downloaded will have the status as ‘Undefined Implementation State’. This is fine and the status will be calculated once the SAP Notes are downloaded.

    Keep the checkboxes against the SAP Notes (of type ‘Input Note’) 3337910 and 3336633 checked and uncheck all other checkboxes all other Input Notes.

    Click on the button ‘Download and Implement’.

  	 ![ex_01_02](images/1.2_3.png)

 

4.	In a pop-up, you will be prompted to provide a transport request. Use the ‘Create Request’ option to create a new transport request.

  	  ![ex_01_02](images/1.2_4.png)


5.	Provide Short Description as ‘Batch_Impl_<your laptop/desk number>’. Click on the save button. This will create a new transport request.

  	  ![ex_01_02](images/1.2_5.png)


6.	The newly created transport request will be filled now. Choose the ‘Ok’ button to continue.
  
    ![ex_01_02](images/1.2_6.png)


7.	You have just created a Note Implementation job using the results of the Note Identification job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.

   	  ![ex_01_02](images/1.2_7.png)


8.	The job can take 2-3 minutes to complete. You can use the ‘refresh’ button to update the status in the Batch Dashboard. Once the job is complete , you can continue with the next exercise – [Viewing the Implementation Results](exercises/ex1#viewing-the-implementation-results).
 
## Exercise 1.3: Viewing the Implementation Results
In the previous steps, you have scheduled a job which will implement SAP Notes based on the results of note identification. Now, we will view the implementation results.

1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step. Locate the Run for Schedule type ‘Note implementation’. You will find a button ‘Implementation Result’ corresponding to this Run. Click on the button.

  	  ![ex_01_02](images/1.3_1.png)


2.	You would have navigated to the ‘SAP Note Batch Implementation Results’ screen. 

    This screen shows all the SAP Notes processed by the batch job. You will find the implementation statuses of the SAP Notes and information/error messages, if any, against each SAP Note.

    Use the checkbox to select a line for any SAP Note which is completely implemented. 

    Click on the button ‘Note Log’ to view the implementation logs of the SAP Note.

  	![ex_01_02](images/1.3_2.png)

 

3.	Observe the results. Once done close the pop-up for Note Batch Implementation Logs

  	![ex_01_02](images/1.3_3.png)


4.	Keeping the checkbox for the same SAP Note selected, click on button ‘Object List’. This will show the list of objects processed by the SAP Note along with its simulation results.

  	![ex_01_02](images/1.3_4.png)


5.	Observe the results. Once done close the pop-up for SAP Note Batch Implementation Results.

  	![ex_01_02](images/1.3_5.png)


You have now completed the exercise for Batch Identification. 

Please proceed with the next exercise – [Exercise 2: Batch Implementation](../ex2/README.md).

