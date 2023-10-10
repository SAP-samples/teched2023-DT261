# Exercise 2 - Batch Implementation

Batch Implementation option enables you provide an SAP Note or a range of SAP Notes for which you want to either schedule an implementation or download the mentioned SAP Notes along with its pre-requisite SAP Notes. 

In this exercise, you will be implementing multiple SAP Notes in a single batch job and then viewing the results. 


## Exercise 2.1 Adding SAP Notes for pre-requisite Identification and Note implementation in Batch Job

  1. Relaunch transaction SNOTE. To do this, type ‘/NSNOTE’ in the top-left section of the screen. 
 
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/c2fa14f8-1225-4e9b-8042-f7acef21856d)
     


  2. In ‘Note Assistant – Home’ screen, navigate to the menu option ‘Batch Processing -> Batch Implementation’.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/6f9548d9-95f8-4535-9b3b-f827e74edd50)



     

  3.	You would have navigated to ‘Schedule SAP Notes Batch Implementation’ screen. This is where you would need to provide the list of SAP Notes.
      Click on the multiple selection button next to ‘SAP Note Number’.

        ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/592cab02-c05e-4381-8050-b50a948ba817)


     

  4. Provide the below SAP Notes in the pop-up that opens.

         2909538
         3333874

     Click on ‘Copy (F8)’.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/c59b6793-f4aa-4c47-930d-cc6ce385f752)
     


5.	Click on ‘Add SAP Notes’.

      ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/458de81c-df88-444d-ad0a-5602714819be)

   

6.  The Notes should now appear in the bottom section of the screen. A status of green or yellow traffic lights indicate that the SAP Note might be possible to be implemented in a batch job. 

      ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/61577fba-1bd9-4098-a8bc-2e09d7350600)

     

7.	These input SAP Notes may have pre-requisite SAP Notes which also needs to be implemented together with these input SAP Notes. Choose ‘Identify Prerequisites’ to identify all such pre-requisite SAP Notes.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/fa9a7ca1-ad6c-46fb-81ac-043d8bcec62d)

    

8.	You will be navigated to a new screen which shows all the pre-requisite SAP Notes for every input SAP Note.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/9d2cb3d3-dc80-4082-a9a4-7af8a16f9e5c)

   

9.	Now we will schedule a batch job to download and implement all the SAP Notes. Choose ‘Download and Implement’ button for this.
    
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/ff16ad3d-ce78-4eae-a66a-08766e68cf12)

    

10.	A pop-up will open. You will be required to provide a job/schedule description and a transport request. Provide the Job/Schedule Description as ****'Batch_Implementation_<your laptop/desk number>****'. Provide the transport request that you created earlier as well.
    
    >Hint:
    >
    >You can use the small button next to the Transport Request field to find the previous transport request.
    >![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/9140e83a-6796-4489-ae82-7e62d0f33070)
    >
    >In the screen that opens, click on 'Execute (F8)'
    >![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/febb5591-a138-47c0-94e3-c844badc7276)
    >
    >In the screen that opens, select the transport request that you created earlier.
    >![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/327d978c-f965-4e5d-907f-d859178f058b)
    >
    >This transfers the transport request number to the relevant field.



    Click on the Ok button in the pop-up to schedule the job.

   	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/02942442-1dc0-463b-8ecc-df44f5bfa1b4)

    

13.	You have just created a Batch Implementation job!

    A pop-up confirming the action with the job details will be shown. Click on the ‘Go to Batch Dashboard’ button in the pop-up. This will navigate to the batch dashboard where you will find the status and results of the job that you have scheduled.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/67415c3e-1cb9-47e5-8a6b-969f8dc8be05)

    

14.	The job can take a couple of minutes to complete. You can use the ‘refresh’ button to update the status in the Batch Dashboard.

   	Once the job is complete , you can continue with the next exercise: [Viewing the Implementation Results](../ex2/README.md#exercise-22-viewing-the-implementation-results).



## Exercise 2.2 Viewing the Implementation Results

In the previous steps, you have scheduled a job which will implement SAP Notes. Now, we will view the implementation results. You have already viewed the implementation results for Note implementation done during the Batch Identification in the previous exercises and this is very similar.

1.	At the end of the previous step, you would have navigated to the ‘SAP Notes Batch Identification/Implementation Dashboard’. You will find the job details with a description matching what you have provided in the previous step. Locate the Run for Schedule type ‘Note implementation’. You will find a button ‘Implementation Result’ corresponding to this Run. Click on the button.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/e2b42fe5-f402-4292-adb8-b2d0c0cc733a)



2.	You would have navigated to the ‘SAP Note Batch Implementation Results’ screen. 

    This screen shows all the SAP Notes processed by the batch job. You will find the implementation statuses of the SAP Notes and information/error messages, if any, against each SAP Note.

    Use the checkbox to select a line for the SAP Note which is completely implemented and has the message ‘Object generating report..’. 

    >The message against the SAP Note mentions that an object generating report has also been executed. As the name suggests, such reports can generate ABAP objects. These ABAP objects are not supported by a standard SAP Note implementation, and therefore a report execution is necessary to generate them. If any such report is found in an SAP Note, then the Batch implementation will also execute these reports in the same batch job, once the report is created during the SAP Note implementation. Any relevant manual activity in the same SAP Note will also be confirmed automatically, as you will find in the below steps.

     Click on the button ‘Note Log’ to view the implementation logs of the SAP Note.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/4169e821-b657-417a-9661-a3921278c1b6)




3.	Observe the results.
   
   
    >You will find that the job has automatically confirmed a manual activity. This will be the manual activity which guides the user to execute the object generating report. The report has been executed in the same background job, hence the manual activity has also been automatically confirmed. 

    Once done close the pop-up for Note Batch Implementation Logs.
 
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/64aa169c-c81f-4265-a171-879776c8e9f8)




4.	Keeping the checkbox for the same SAP Note selected, click on button ‘Object List’. This will show the list of objects processed by the SAP Note along with its simulation results.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/bc1c16f6-29af-4e1f-9de0-e744798f2cfb)




5.	Observe the results. This will be the object generating report created during the Note implementation.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/45729576-cb04-4d3c-9022-15e8e118b9cb)


     Once done close the pop-up for SAP Note Batch Implementation Results.


6.	To view the application logs for the object generating report execution, choose the button ‘Display Application Log’ next to the relevant SAP Note.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d39b5c9a-25cf-486a-b869-ea2bc406b30c)




7.	The tool navigates to the application logs. Observe the results.
   
     >This will contain all the objects created/modified during the report execution which happened in the same background job. You can notice that the object generating report name is also mentioned in the column ‘Program’.


     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/2113f450-a5d3-4a04-b714-dc2cdb0b647c)

 


## Summary

Awesome! You have now completed the exercise for Batch Implementation. 

Please proceed with the next exercise - [SAP Note Analysis and Batch Implementation using Note Analyzer](../ex3%20#sap-note-analysis-and-batch-implementation-using-note-analyzer)

