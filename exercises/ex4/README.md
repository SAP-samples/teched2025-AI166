# Exercise 4 - Using Your App on your Phone

In this exercise, you will explore different features of the mobile app you built.

*Estimated Time: 🕓 10 minutes*

## Exercise 4.1 User Onboarding

1. Launch the **Mobile Svcs** app on your iOS/Android device.  

2. Tap **Agree** on the End User License Agreement and Privacy Statement.  

3. Tap **Use QR Code Scan** / **Scan** to start the device camera for scanning the onboarding QR code.  
   > Allow the app to access the camera on your device to scan the onboarding QR code.

4. Scan the QR code shown at the end of Exercise 3 in SAP Business Application Studio.  

5. Once the scan succeeds, tap **Continue**.  

6. Log in using the credentials provided by the session speakers.  
   > If prompted, select **`tdct3ched1.accounts.ondemand.com`** on the Identity Provider selection page.  

7. Create a passcode (minimum 8 characters) to unlock the app, and then tap **Next**.  

8. Confirm the passcode and tap **Done**.  

9. (Optional) Enable **Biometric Authentication** to unlock the app and decrypt data.  
   > You can also create a multi-user MDK app, i.e., one app shared among different workers based on shift timings.  
   > If this option is enabled, users do not get the option to use biometric authentication.

10. Tap **Now** to accept the deployed metadata definitions.  
    > If prompted, tap **Allow** to let the app send you notifications.  

| iOS | Android |
|-----|---------|
| <img src="images/ios-onboarding.gif" alt="iOS Onboarding" height="750" /> | <img src="images/android-onboarding.gif" alt="Android Onboarding" height="750" /> |

## Exercise 4.2 Scan to Search

1. Tap **Products** to open the products list.  

2. Using any online tool, create a QR code and a barcode for some text from the product list.  
   Example:  

   | QR Code | Barcode |
   |---------|---------|
   | `Camcorders` | `Ink Jet Printers` |

3. Tap the **magnifying glass** icon.  

4. Tap the **scanner icon** in the search bar.  

5. Scan the codes you generated.  
   Example:  

   | QR Code | Barcode |
   |---------|---------|
   | <img src="images/qr-code.gif" alt="QR Code" /> | <img src="images/bar-code.png" alt="Barcode" /> |  

| iOS | Android |
|-----|---------|
| <img src="images/ios-scanning.gif" alt="iOS Scanning" height="750" /> | <img src="images/android-scanning.gif" alt="Android Scanning" height="750" /> |

## Exercise 4.3 Offline Actions

1. Turn on **Airplane mode** on your device (no cellular or Wi-Fi).  

2. Tap **Customers** to open the Customers list.  

3. Make a couple of modifications, for example:  
   - Edit the name of an existing customer to your name.  
   - Delete a customer record.  

4. Return to the main page and, in the popover menu, tap **Sync Changes**.  
   > Since you are offline, you will see an error.  

5. Turn off Airplane mode on your device, then sync changes again once the device is back online.  

6. Verify your changes on the backend.  
   
   To access the backend, replace **<YOUR APP ID HERE>** in the URL below with the App ID you created in [Exercise 2.2](/exercises/ex2/README.md#exercise-22-create-a-mobile-services-app).  

   > Note: Your App ID is of the format `edu.xxx.teched25`. When inserting it into the URL, replace each `.` with `-`. For example, `edu.xxx.teched25` &rarr; `edu-xxx-teched25`.

   ```url
   https://ai166-ftaiywgj-ai166<YOUR APP ID HERE>.cfapps.eu10-004.hana.ondemand.com/com.sap.edm.sampleservice.v4/Customers?auth=uaa
   ```

   | iOS | Android |
   |-----|---------|
   | <img src="images/ios-offline.gif" alt="iOS Offline" height="750" /> | <img src="images/android-offline.gif" alt="Android Offline" height="750" /> |


## Summary

You've experienced how you can build a native application with cutting-edge features such as scanning and offline support on both platforms while maintaining a single code line.

## Navigation
| Previous| Next |
|---|---|
| [Exercise 3](../ex3/README.md) | [Exercise 5](../ex5/README.md) |