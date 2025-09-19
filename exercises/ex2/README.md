# Exercise 2 - Create A Mobile Services App in Cockpit

You will get comfortable with Mobile Services Cockpit and create a new Mobile Services app.

## Exercise 2.1 Access Mobile Services

1. Open the Mobile Services Cockpit: [https://mobile-service-cockpit-web.cfapps.eu10.hana.ondemand.com/logincfapi/index.html](https://mobile-service-cockpit-web.cfapps.eu10.hana.ondemand.com/logincfapi/index.html)  
2. Enter the API Endpoint: **`https://api.cf.eu10-004.hana.ondemand.com`** and click **Login**.  
   ![API Endpoint](images/api-endpoint.png)  
3. Enter the origin key: **`tdct3ched1-platform`** and click **Sign in with alternative identity provider**.  
   ![Origin Key](images/origin-key.png)  
4. Log in using the credentials provided by the session speakers.
5. Verify the **Organization** and **Space** details as shown in the image, then click **Open**.  
   ![Organization and Space](images/org-space.png)

## Exercise 2.2 Create Mobile Services Cloud 

1. Create new app
2. Select MDK in Type of Application step of the Wizard and click Next
3. Configure the following details in the Basic Info step of the Wizard and click Next
   | Key    | Details | Comments |
   | --------- | ----------- | ----------- |
   | Service Plan | build-code | |
   | ID | edu.xxx.teched25 | Replace xxx with your studnet number, i.e. the last 3 digits of your login email. |
   | Name | XXX MDK App | Replace xxx with your studnet number, i.e. the last 3 digits of your login email. |
   | Description | <anything you prefer> | Since the mobile service space is shared among all students. It is important that you follow the nomencleature. You can add anything custom in description to make the app identifiable for yourself. |
4. Keep XSUAA Settings selected in the Security Settings step and click Next
5. Don't enable Role Settings and click Next
6. Ensure the following feautures are checked in the Assigned Features step and click Next
7. Review the details you have entered and click Finish.

The creation of the new application can take up to 90 seconds. Until then you can do the optional [exercise 2.3](#exercise-23-j4c-queries-optional). Else you can proceed to [Summary](#summary)

## Exercise 2.3 J4C Queries (Optional)

1. Launch J4C - https://ai166-ftaiywgj.eu10.sapdas.cloud.sap/joule and ask the following queries.

2. XSUAA vs IAS
   Example query:  
   > What is the difference between XSUAA and IAS in Mobile Services?

3. Role Settings
   Example query:  
   > What are role settings in SAP Mobile Services? How are they different from SAML attributes? 


## Summary

You've now experienced the Mobile Services Cockpit and created a new Mobile Services app.

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md) //TODO

