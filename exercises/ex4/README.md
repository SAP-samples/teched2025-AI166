# Exercise 4 - Exercise 4 Description

In this exercise, you will use different features of the app you built on your phone.


## Exercise 4.1 User Onboarding

1. Launch **`Mobile Svcs`** app on your iOS/Android device. 

2. Tap **Agree** on `End User License Agreement and Privacy Statement`.

3. Tap **Use QR Code Scan**/**Scan** to start the device camera for scanning the onboarding QR code. 
   
   > Allow the app to access the camera on your device to scan the onboarding QR code.

4. Scan the QR Code shown at the end of exercise 3 in SAP Business Application Studio.

5. Once scan is succeeded, tap **Continue**.

6. Log in using the credentials provided by the session speakers.  
   
   > If prompted, select **`tdct3ched1.accounts.ondemand.com`** on the Identity Provider selection page.  

7. Create a passcode that is at least 8 characters long to unlock the app, and then tap **Next**.

8. Confirm the passcode and tap **Done**.

9.  You have the option to enable Biometric Authentication for unlock the app and unencryp the data. Tap **Enable** if you wish to use this feature.
  
  > You can create a multi-user app in MDK, i.e. one app shared among different workers based on shift timings. If this option is enabled, users do not get the option to use biometric.

9.  Tap **Now** to accept the deployed metadata definitions.

  > If prompted, tap **Allow** to let the app send you notifications.

| iOS | Android |
|-----|---------|
| ![iOS Onboarding](images/ios-onboarding.gif)) | ![Android Onboarding](images/android-onboarding.gif) |


## Exercise 4.2 Scan to Search

1.	Tap on products to open the products list

2.	Using online tools, create a QR Code and a Barcode for some text that you see in the product list.
    For example:
    | QR Code | Barcode |
    | --- | --- |
    | `Camcorders` | `Ink Jet Printers` | 

3. Tap on the magnifying glass

4. Tap on the scanner icon in the search bar

5. Scan the codes you generated
   For example:
    | QR Code | Barcode |
    | --- | --- |
    | ![QR Code](images/qr-code.gif) | ![Bar Code](images/bar-code.gif) | 
   

| iOS | Android |
|-----|---------|
| ![iOS Scanning](images/TODO)) | ![Android Onboarding](images/TODO) |


## Exercise 4.3 Offline Actions

1. Turn on the airplane mode on your device, i.e. no cellular or wifi.
2. Tap on Customers to open the Customers List
3. Make a couple of modifications.
   E.g. Edit the name of an exisiting customer to your name. And Delete a customer record.
4. Come back to the Main page and in the pop-over menu tap on Sync Changes.
   
   > Since you have no network, you will see an error.

5. Turn off airplane mode on your device, and try to sync changes after the device gets internet connection.

6. Verify your changes on the back-end.
   To access the back-end, replace **<YOUR CHANGE HERE>** in the following URL with the ID you defined in [Exercise 2.2](/exercises/ex2/README.md#exercise-22-create-a-mobile-services-app)
   
   `https://ai166-ftaiywgj-**<YOUR CHANGE HERE>**.cfapps.eu10-004.hana.ondemand.com/com.sap.edm.sampleservice.v4/Customers?auth=uaa`

   > If prompted, Log in using the credentials provided by the session speakers.


| iOS | Android |
|-----|---------|
| ![iOS Offline](images/ios-offline.gif)) | ![Android Offline](images/TODO) |

## Summary

You've now ...

Continue to - [Exercise 5 - Exercise 5 Description](../ex5/README.md)