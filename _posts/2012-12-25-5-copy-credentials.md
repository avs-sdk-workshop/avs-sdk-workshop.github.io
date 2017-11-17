---
title: '5. Copy Your Credentials'


layout: nil
---

1. On your Raspberry Pi, open the File Explorer by clicking on the folder icon on your toolbar at the top left.  It should come up in the **/home/pi** folder.  Navigate to the **avs-sdk** folder.  Right-click on **config.sh** and select "Text Editor" to open your configuration file.  

![](assets/config_file.png)

It should contain the following fields:

`CLIENT_SECRET=""
DEVICE_SERIAL_NUMBER=""
CLIENT_ID=""
PRODUCT_ID=""
`
2. In your web browswer, Navigate back to the AVS dashboard:  [https://developer.amazon.com/avs/home.html#/avs/home](https://developer.amazon.com/avs/home.html#/avs/home).
3. Click **Manage**. From **Details and management** copy your **Product ID** (no spaces) into the `PRODUCT_ID` field of your **config.sh** file.
4. Select **Security Profile** from the left tab and copy your **Client ID** and **Client Secret**.  
5. Place the **ClientID** and **ClientSecret** into the `CLIENT_ID` and `CLIENT_SECRET` fields.  
6. The **device serial number** is created by device makers and isn't used by AVS - for this workshop, it can be any alpha-numeric value (here it's 123456):

example:

`CLIENT_SECRET="12345678901234567890128901234567890123456789012345678901234"
DEVICE_SERIAL_NUMBER="123456"
CLIENT_ID="amzn1.application-oa2-client.12345678901234567890123456789012"
PRODUCT_ID="TEST_SPEAKER"
`
{:.verify}

### Checkpoint 5

1. Make sure you've saved the config.sh file in your /home/pi folder with your **Device Type ID**, **Device Serial Number**, **Client ID** and **Client Secret**.
