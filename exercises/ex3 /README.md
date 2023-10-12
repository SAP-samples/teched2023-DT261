# Exercise 3: SAP Note Analysis and Batch Implementation using Note Analyzer

Note Analyzer is a tool that allows you analyse the SAP Notes provided by SAP in a file format. The tool analyse and suggests possible actions depending on the result. 
By the end of this Exercise, you will know how to launch Note Analyzer, from where to download the input XML files, how to upload the XML file and how to interpret the analysed result and take actions.

## Exercise 3.1: Launch Note Analyzer
1.	Go to transaction /nSNOTE to launch ‘Note Assistant – Home’ screen.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/3ee5ccd9-a515-47de-9308-947ffc289d9b)

2.	In ‘Note Assistant – Home’ screen, navigate to the menu option ‘Goto -> Other Tools -> Launch Note Analyzer’.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1139b328-c14c-49e0-bf7a-6cd1bdd83e5f)

3.	You would have now reached to the Note Analyzer Home Start Screen.
    Here you can have the option to Upload the XML file and rerun the already uploaded XML File.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/0ed6f0d1-6941-4733-851b-7a3166f82f72)



## Exercise 3.2: Analyze SAP Note

### Exercise 3.2.1: Download XML File from Support Launch Pad

1.	First step is to download the XML file. 
    Go to the link [https://me.sap.com/notes/3383921](https://me.sap.com/notes/3383921).

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/10b8adf2-b1d8-413f-90a0-567e08976bf1)

2.	Click on 'Attachments' Tab.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/57e6fcfd-5805-4756-a1a9-1729c08e6440)

3.	Click on file TECHED_HANDS_ON_DEMO.XML

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/26da7ef7-03ce-4943-9c3a-506d9a1e56fc)

    Your files will get downloaded and get saved in the Downloads folder of the system.



### Exercise 3.2.2: Upload the XML

Next step is to upload the XML file.

1.	Go back to Note Analyzer window
   
2.	Click on Upload

  	![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/edbd9217-f27c-4cbc-a7c8-bd871f0672db)

3.	Choose the XML file.	
    Navigate to folder where the file got saved. Here it got saved in Downloads. 
    Choose file “TECHED_HANDS_ON_DEMO.xml”  Click on ‘Open’.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/e3903187-adac-464c-b664-0b5215e7432a)

    Click allow if you get the below pop-up

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/21a345a8-c4e3-4db5-9ec4-18c05b1b2fe1)

    Now the file is loaded to the system.


### Exercise 3.2.3: Analyze the Uploaded XML

1.	Click on “Analyze”

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/deade09e-37b6-44ed-92b7-1ea2fc16c874)

2.	Result is now ready to analyze by following the below steps.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/4e2f6246-a916-4c5f-8267-54b76aa86112)

    >The overall status of the Note Analyzer is in Red with Preparation SAP Note Check Phase, SAP Note Check Phase with status Red and Scope information with Yellow. After taking all the necessary action it become Green.

    Now it’s the time for the deep dive into the details of the tool. We can take the action one by one to finish the Analysis.


#### Action 1: Preparation SAP Note Check Phase

At the beginning of this activity, you will make the SNOTE up to date.

1.	Click on the hyperlink ‘Action Needed’ against the First Phase ‘Preparation SAP Note Check Phase’.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/5fbcddbd-24f9-4403-af5c-eb9619f450c3)

    These are the SAP Notes needed in your system to make the SNOTE up to date. From this screen you can read it as out of 3 SAP Notes, currently 1 SAP Note is required to make your SNOTE up to date. All the action needed SAP Notes will be with status ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/af78a893-d6a4-45ec-9ef0-a5b7b2b4a817).

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/8bcdce14-0748-4eda-9223-ff385c4b5704)

2.	Next step, take the pending action on this SAP Note.
   
    >The column Valid Prerequisite indicates here how many Pre-requisites is needed for this SAP Note to get successfully installed.
    
    Click on the Button against on ‘Action’ Column for the SAP Note 1668882. The action column indicates the Button to Implement.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b171f16c-4ec1-4d8d-bc49-6e359d8fe81c)

    Now the implementation of this SAP Note has started along with its pre-requisites.

3.	If Asked, Choose the Transport Request TE1K900024 by clicking on the button ‘Own Request’. If you don’t see the below pop up proceed to step 5.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/6e18b991-7f9f-409d-8766-7ba2bdd38055)

4.	Once the Transport Request is selected, click on Continue Button.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/983bd44c-eec4-410f-8525-33d005d92383)

5.	Now you will be seeing the object list. Click on the Next Button to finish the SAP Note Implementation 

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/69580e9d-33a9-4c58-bdbb-8c3280dfe62a)

    Now you can see the needed SAP Note 1668882 in Completely Implemented Status with Green Traffic Light and the ‘Preparation SAP Note Check Phase’ turned to ****Green**** from ****Red****.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/6318be20-d042-4be6-889a-5ff6ca2a6efe)

   You have now successfully completed the Action 1 and made SNOTE up to date.

#### Action 2: Manual Activities Needed
Here you will be performing any Manual activities mentioned by SAP for the completeness of the process.

1.	Double Click on the Main Node to reach Overview Page 

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/0b4a43d3-4be4-4b3f-b531-dbc42504b1ae)

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/3e56389f-f961-4136-843d-fad65f7348b2)

2.	Click on the View Details to get into the details. 
    Scope information will always be in Yellow Traffic as it’s a Manual Activity that has to be performed by the customer if needed in their system.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b76d157c-8e04-48e9-9960-0177edf1a2ee)

   
3.	The message over here is to execute a Report before proceeding.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/e684800e-8495-485b-b229-f026e6ad9038)

4.	Let’s perform this activity.
    Create a new GUI Window: Click on the 3 lines in the extreme left top Corner and then click New GUI Window.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/6bb11e51-4979-49c5-9bec-23b62a54d3cf)

5.  Enter Transaction as /nSE38 and press ‘Enter’.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/3e6f7d70-060c-488c-a40c-b00a53378c36)

6.	Input the Report Name N_PREPARTION_APPL and Click on Execute ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/a1e570b2-66d6-49b6-8666-f573b0257278)
.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/470faa19-015a-4d61-a112-031009cf0756)

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/3e6deefb-77e4-4809-8edc-a75ff4cf7ec5)

7.	Now you have performed the Manual Activity mentioned.
   
    >This is an example of Manual Activity. SAP can provide any type of comments or activities over here.
    
8.	You can move to the Last Action. Go back to the Note Analyzer Screen now.

#### Action 3: SAP Note Check Phase

Here you will get an overview of all the SAP Notes needed for the application and the next action for the same. 

1.	Double Click on the Main Node to reach Overview Page. 

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d007cc44-0a16-48b3-8d22-8f443062e421)

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/f828511e-b031-4b8b-9716-e47e42c008de)

2.	Click on the ‘Action Needed’ hyperlink against SAP Note Check Phase.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/2e7ac080-3859-4b57-810d-396edf63be29)

3.	You now reached to the SAP Note Check Phase.
    Three SAP Notes here needs an action.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/f6cdcaa1-f6ec-47c1-bf31-7c847ee1b7d5)

4.  Click on the SAP Note 3367975.

    >Clicking on this link will give you the full details of this SAP Note.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/a521dd9a-f453-46ad-9f8d-caf8b24a8b70)

    This SAP Note is opened in SNOTE transaction in a new session as the SAP Note is already downloaded in the system.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/bbb1093a-00bc-4bb1-9a74-9e47f0ebcad7)

    You can now close this newly opened window.

5.	 Click on the SAP Note 3369905.

     >Clicking on this link will give you the full details of this SAP Note.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1ec2b158-e40c-4741-8f24-3fe3fd712724)

     Click on ‘Allow’ if you get the below screen.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/5a71e3c2-ae4d-483a-8c3f-2e1bccbccb22)

     This SAP Note will open in [https://me.sap.com](https://me.sap.com).
     Here the SAP Note file is not yet downloaded to the system hence it opened in browser.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/c13d18e0-7270-4780-a287-c04c3d100cc5)

     You can now close this window and go back to Note Analyzer Screen.

6.   Observe the icon Changes in Action Column. Hover over each icon to get the Tool Tip.
     First two SAP Notes are with Action Implement ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b56b76aa-6232-4647-9cce-86b564012d9a)
  as these are already downloaded to the System.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/ac5ecd31-b9cd-44e9-b3e3-4b472fa83752)

     Third SAP Note is with Action Download ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/58212ef6-659c-4896-a378-fee188341aba)
 . This action will change to implement Action once the SAP Note is downloaded to the system.

7.	 Click on the Hyperlink ‘Details’ against any one SAP Note.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/1d40fefe-d252-4b02-9c9b-e393fd9accbf)


     This will give the information of what type of Correction Instruction this SAP Note has like whether the SAP Note contain Automatic Correction Instruction or Manual Correction Instruction etc.
     Click OK to close the same.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/46762bde-aeb2-4e9c-84ec-a48aae5469ac)

8.	 Click on hyperlink against the SAP Note 3367975 in Valid Prerequisite column.
    
     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/5cea4c91-760d-4821-8357-3bd0214fde16)

     This will display the valid prerequisite for this SAP Note in the current system.
  	 
     >This list may have few invalid prerequisites SAP Note as well. This detail is available even if the SAP Note is not downloaded to the system. 

     Click OK to Close the window.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/504c9bcf-6af7-4e88-a1cc-cb3f23bdba31)

 9.	 Click on the ‘More info’ column button against the SAP Note 3367975.   

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/10ab8c8e-3ad3-47d0-a051-04a84ec349dc)

     This shows the validity of the SAP Note. Click ‘Ok’ to close the same.

     ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/b3b9f86e-a857-4a09-91bc-3933d78c807e)

10.	 Implement the needed SAP Notes.

      >We can either implement the needed SAP Notes one by one in foreground by clicking on the ‘Action’ Button against the individual SAP Note, or we can implement multiple SAP Notes in background.

      In this exercise, we will use the background process to implement all SAP Notes from the Note Analyzer in one go.

      Click on the ‘Batch Implementation’.

      ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d6a23c55-a092-4d0c-9874-f6543450a0a2)

      >We can Implement selected SAP Notes in Background or we can implement all valid SAP Notes from the list in background.

      We will go ahead with all valid SAP Notes. Click on ‘All Valid Notes’.

      ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/39d83507-3e11-410e-899f-99119299bbd3)

11.	Enter the Transport Request as TE1K900024 then click ‘Ok’.
         
    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/d9d7b32c-1756-4986-9073-050e9650260f)

12.	Your Job to implement all the Valid SAP Notes has been scheduled. Click on ‘Go to Batch Dashboard’ to view the background job details.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/8b57d554-0cc5-4782-88f0-f92b93721e8c)

    This is the same dashboard you have already seen in your prior exercises. The display will be filtered with the Schedule IDs for the Current XML. The description of the Schedule/Run ID is “SNOTE_NA_(Name of the XML).

    If the Schedule Status in In Progress, click on ‘Refresh’ button to get the Latest status. The Job can take 1 – 2 minutes to complete.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/326d91ff-6044-41e2-ac84-29bf3c76a436)

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/c1fbdb61-aefa-45be-a4a4-a6df61c890d1)

    You have now successfully scheduled and implemented the Job from Note Analyzer tool.

## Exercise 3.3: Conclusion    

You have now completed all the actions required for the input XML. 

1.	Click on Back Button to Navigate back to the Note Analyzer.

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/ddbb4b5b-8f59-477d-852c-64b36a8a15c2)

2.	You are now back to the Note Analyzer Screen.    

    ![image](https://github.com/SAP-samples/teched2023-DT261/assets/144778626/80e4b1f7-b08f-488d-aecb-1f238716fa82)

    You can find that the phases are now turned to **Green** along with Main Node. That means you have successfully implemented all the needed SAP Notes from this XML to make the application up to date.   


**Congratulations! You have now completed all the steps for today’s session!**
