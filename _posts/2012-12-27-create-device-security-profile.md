---
title: '3. Create a Device & Security Profile'


layout: nil
---

{:.steps}
### Register Your Product and Create a Security Profile

After you've registered for an Amazon developer account, you'll need to create an Alexa device and security profile. Make note of the following parameters **ProductID** (also known as **Device Type ID**), **ClientID**, and **ClientSecret** -- you'll need these while setting up the project.

1. Login to Amazon Developer Portal - [developer.amazon.com](https://developer.amazon.com/login.html)
2. Click on Apps & Services tab -> Alexa -> Alexa Voice Service -> Get Started  
   ![](assets/avs-navigation-new.png)
3. In the Register a Product Type menu, select **Device**.  
	 ![](assets/avs-choose-device.png)

{:.tab}
#### Device Type Info (Left Nav)

1. **Device Type ID**: provide a simple identifier for your product. **No spaces.**
2. **Display Name**: the display name in the developer portal, as well as the name that will be provided to your users when they register the product with Amazon.
3. Click **Next**  

{:.tab}
#### Security Profile (Left Nav)

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

{:.tab}
#### Device Details (Left Nav)

1. Image: Right click on this link to save this test image to your computer (or use your own), then upload it:   
[https://developer.amazon.com/public/binaries/content/gallery/developerportalpublic/solutions/alexa/alexa-voice-service/images/reference-implementation-image.png](https://developer.amazon.com/public/binaries/content/gallery/developerportalpublic/solutions/alexa/alexa-voice-service/images/reference-implementation-image.png)
2. Category: **Other**
3. Description: **Alexa Voice Service sample app test**
4. What is your expected timeline for commercialization?: **Longer than 4 months / TBD**
5. How many devices are you planning to commercialize?: **0**  
6. Click **Next**.  
   ![](assets/avs-device-details-filled.png)

{:.tab}
#### Amazon Music (Left Nav)

1. Select **No** and click the **Submit** button.

{:.verify}
### Checkpoint 3
1. Ensure that your device is now listed in the AVS dashboard [https://developer.amazon.com/edw/home.html#/avs/list](https://developer.amazon.com/edw/home.html#/avs/list)
2. Click the **Edit** button next to your device in the AVS dashboard. Navigate to **Security Profile** > **Web Settings** and ensure that you've set your **Allowed Origins** and **Allowed Return URLs**.

