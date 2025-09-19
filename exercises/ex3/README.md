# Exercise 3 - Exercise 3 Description

In this exercise, you will access the SAP Build Lobby to create a an MDK Project and deploy the first version of your app.

## Exercise 3.1 Access Lobby

1. Open the SAP Build Lobby: https://ai166-ftaiywgj.eu10.build.cloud.sap/lobby

  > If prompted, select "tdct3ched1.accounts.ondemand.com" on the Identity Provider selection page.

2.	Log in using the credentials provided by the session speakers.

![XXX AI to add name](images/xxx-ai-to-add-name.png)  

## Exercise 3.2 Create Mobile Project

1. In the SAP Build Lobby, click **Create** > **Create** to start the creation process.

![XXX AI to add name](images/xxx-ai-to-add-name.png)  

2. Click the **Application** tile and choose **Next**.    

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

3. Select the **Mobile** category and choose **Next**.

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

4. Select the **Mobile Application** to develop your mobile project in SAP Business Application Studio and choose **Next**. 

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

5. Enter the following details and click **Review**
   
   | Key          | Value               | Comments |
   |--------------|---------------------|----------|
   | Name         | `XXXMDKApp`       | Replace `xxx` with your student number (last 3 digits of your login email). |
   | Description  | *Any text you prefer* | Since the Mobile Services space is shared, follow the naming convention. You can customize the description to help identify your app. |
   | Dev Space         | `Mobile`       | SAP Build pre-selects the dev space it deems most suitable, and it will automatically create a new one for you if you don't already have one. If you have pre-existing dev spaces of the Mobile Application type, you can reuse them. For more details, see [Dev Space Manager](https://help.sap.com/docs/build_code/d0d8f5bfc3d640478854e6f4e7c7584a/ad40d52d0bea4d79baaf9626509caf33.html) |
   
    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  
    

6. Review the inputs under the Summary tab. If everything looks correct, click **Create** to proceed with creating your project.

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

    > Your project is being created in the Project table of the lobby. The creation of the project may take up to 120 seconds. In the meantime, you can try the optional [Exercise 3.6](#exercise-36-j4c-queries-optional)

7. After the project has been created successfully, click the project to open it. 

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  
    
8. The project opens in SAP Business Application Studio.

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

    >When you open the SAP Business Application Studio for the first time, a consent window may appear asking for permission to track your usage. Please review and provide your consent accordingly before proceeding.


## Exercise 3.3 Log in to CF

1. Launch Command Pallete Shift+Ctrl+P and type "Login" and select "CF: Login to Cloud Foundry"

2. Select authetication mode as "SSO Passcode" and click "Open a new browser page to generate your SSO Passcode"

3. Sign in with the credentials provided to you during the session.
   
   > In case you don't get an option to select your username, enter the origin key: **`tdct3ched1-platform`** and click **Sign in with alternative identity provider**.

4. Copy the temporary Authentication Code

5. Pase it in the Enter your SSO Passcode input field and click Sign In

6. Verify the **Organization** and **Space** details as shown in the image, then click **Apply**.

You will recieve toas notifications confirming your CF Login has been completed successfully.


![XXX AI to add name](images/xxx-ai-to-add-name.gif)  


## Exercise 3.4 Configure the Runtime & External Resources Using Storyboard


1. Click on **+** button in the **Runtime Resources** column to add a mobile services app to your project. 

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)  

2. Search for `XXX` Choose `edu.xxx.teched25` from the applications list in the **Mobile Application Services** editor.

    ![XXX AI to add name](images/xxx-ai-to-add-name.png) 

    > Replace `xxx` with your student number (last 3 digits of your login email).

3. Select `com.sap.edm.sampleservice.v4` from the destinations list and click **Add App to Project**.

   ![XXX AI to add name](images/xxx-ai-to-add-name.png) 

In the storyboard window, the app and mobile destination will be added under the Runtime Resources column. The mobile destination will also be added under the External Resources with a dotted-line connection to the Runtime Resource.

![XXX AI to add name](images/xxx-ai-to-add-name.png)

## Exercise 3.5 Create Application UI

1. Click the **+** button in the UI application column header to add mobile UI for your project.

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)

2. In the **Basic Information** step, enter the following details and click **Next**:  

   | Key          | Value               | Comments |
   |--------------|---------------------|----------|
   | MDK Template Type | `CRUD`        |          |

   > leave the other options as they are.
   
   ![XXX AI to add name](images/xxx-ai-to-add-name.png)

3. In the **Data Collections** step, provide the below information and click **Finish**.

    | Key | Value |
    |----|----|
    | `Enter a path to service (e.g. /sap/opu/odata/sap/SERVICE_NAME)` | Leave it as it is  |
    | `Select the Service Type` | Keep `OData` |
    | `Enable Offline` | Keep `Yes` |
    | `Select all data collections` | Choose `Yes` |

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)

    > Since you have Enable Offline set to *Yes*, the generated application will be offline enabled in the MDK Mobile client. Therefore, the end-user can keep making fast read/writes with the local DB without letting the network slow them down.

4. After clicking **Finish**, the storyboard is updated displaying the UI component. 

    ![XXX AI to add name](images/xxx-ai-to-add-name.png)

The MDK project is being generated in the project explorer. Once done, it will automatically deploy the first version to the Mobile Services based on the selections made during the UI Creation. The whole process may take up to 60 seconds. In the meantime, you can try the optional [Exercise 3.6](#exercise-36-j4c-queries-optional).


## Exercise 3.6 J4C Queries *(Optional)*

1. Launch J4C: [https://ai166-ftaiywgj.eu10.sapdas.cloud.sap/joule](https://ai166-ftaiywgj.eu10.sapdas.cloud.sap/joule)  

2. Try the following example queries:  

   - **App in Cockpit vs Lobby**  
     > What is the difference between the MDK app I create in Mobile Services Cockpit, vs. the MDK app I create in SAP Build Lobby?  

   - **Runtime vs External resource**  
     > What is the difference between Runtime Resource and External Resource for an MDK app?  

## Summary

You've now used SAP Build Lobby to create your MDK project and deploy the first version. After the deployment You will now see a QR code for onboarding the mobile app. Leave the Onboarding dialog box open for the next step

Continue to - [Exercise 4 - Exercise 4 Description](../ex4/README.md)