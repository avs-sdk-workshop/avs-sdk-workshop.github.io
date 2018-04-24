---
title: '4. Input Your Credentials'


layout: nil
---

1. On your Raspberry Pi, open the File Explorer by clicking on the folder icon on your toolbar at the top left.  It should come up in the */home/pi* folder.  Right-click on **config.txt** and select "Text Editor" to open your configuration file.  

![](assets/config_file.png)

It should contain the following fields:

```
DEVICE_SERIAL_NUMBER=""
CLIENT_ID=""
PRODUCT_ID=""
```

2. In your web browser, Navigate back to the AVS dashboard:  [https://developer.amazon.com/avs/home.html#/avs/home](https://developer.amazon.com/avs/home.html#/avs/home).
3. Click **Manage**. From **Details and management** copy your **Product ID** (no spaces) into the `PRODUCT_ID` field of your **config.sh** file.
4. Select **Security Profile** from the left tab, navigate to **Other Devices and Platforms** and copy your **Client ID**.  
5. Place the **ClientID** (make sure it's from **Other Devices and Platforms** section) into the `CLIENT_ID` field.  
6. The **device serial number** is created by device makers and isn't used by AVS - for this workshop, it can be any alpha-numeric value (here it's 123456):

Your completed config.txt fields will look something like this:

```
DEVICE_SERIAL_NUMBER="123456"
CLIENT_ID="amzn1.application-oa2-client.12345678901234567890123456789012"
PRODUCT_ID="TEST_SPEAKER" (your custom name)
```

