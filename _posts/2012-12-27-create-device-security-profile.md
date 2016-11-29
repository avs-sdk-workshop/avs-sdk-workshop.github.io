---
title: '3. Create a Device & Security Profile'


layout: nil
---

### Register Your Product and Create a Security Profile

After you've registered for an Amazon developer account, you'll need to create an Alexa device and security profile. Make note of the following parameters **ProductID** (also known as **Device Type ID**), **ClientID**, and **ClientSecret** -- you'll need these while setting up the project.

1. Login to Amazon Developer Portal - [developer.amazon.com](https://developer.amazon.com/login.html)
2. Click on Apps & Services tab -> Alexa -> Alexa Voice Service -> Get Started  
   ![](assets/avs-navigation-new.png)
3. In the Register a Product Type menu, select **Device**.  
	 ![](assets/avs-choose-device.png)
4. Fill in and save the following values:

**Device Type Info**

1. **Device Type ID**: provide a simple identifier for your product.
2. **Display Name**: the display name in the developer portal, as well as the name that will be provided to your users when they register the product with Amazon.
3. Click **Next**  

**Security Profile**

1. Click on the Security Profile drop down and choose **Create a new profile**  
	 ![](assets/avs-create-new-security-profile.png)

2. From the **General Tab** enter the following:    
	 - **Security Profile Name**: Alexa Voice Service Sample App Security Profile
	 - **Security Profile Description**: Alexa Voice Service Sample App Security Profile Description
	 - Click **Next**.  

   **Note:** These are suggested values. You provide custom information for **Security Profile Name** and **Security Profile Description**.

	 Client ID and Client Secret will be generated for you.

3. Now click on the **Web Settings Tab**.
	 - Make sure the security profile you just created is selected in the drop-down menu, then click the **Edit** button.  
	   ![](assets/avs-web-settings.png)
	 - **Allowed Origins**: Click "**Add Another**" and then enter **https://localhost:3000** in the text field that appears.
	 - **Allowed Return URLs**: Click "Add Another" and then enter **https://localhost:3000/authresponse** in the text field that appears.
	 - Click **Next**.  
     ![](assets/avs-web-settings-filled.png)

**Device Details**

1. Image: Save the following test image to your computer (or use your own), then upload it:
   ![](https://developer.amazon.com/public/binaries/content/gallery/developerportalpublic/solutions/alexa/alexa-voice-service/images/reference-implementation-image.png)
2. Category: **Other**
3. Description: **Alexa Voice Service sample app test**
4. What is your expected timeline for commercialization?: **Longer than 4 months / TBD**
5. How many devices are you planning to commercialize?: **0**  
6. Click **Next**.  
   ![](assets/avs-device-details-filled.png)

**Amazon Music**

1. Select **No** and click the **Submit** button.

### Enable Your Security Profile

1. Open a web browser, and visit [https://developer.amazon.com/lwa/sp/overview.html](https://developer.amazon.com/lwa/sp/overview.html).
   ![](assets/avs-lwa-new-security-profile.png)

2. Near the top of the page, select the security profile you created earlier from the drop down menu and click **Confirm**.  
   ![](assets/avs-lwa-choose-security-profile.png)
3. Enter a privacy policy URL beginning with http:// or https://. For this example, you can enter a fake URL such as http://example.com.
4. [Optional] You may upload an image as well. The image will be shown on the Login with Amazon consent page to give your users context.
5. Click Save.

	 ![](assets/avs-privacy-url.png)

6. Next to the Alexa Voice Service Sample App Security Profile, click Show Client ID and Client Secret. This will display your client ID and client secret. Save these values. You’ll need these.
   ![](assets/avs-show-creds.png)  
   ![](assets/avs-view-security-profile-creds.png)
