---
title: '5. Copy Your Credentials'


layout: nil
---

1. From the file explorer on your Pi desktop, navigate to /home/pi/avs-sdk.  Right-click on **config.sh** and select "Text Editor" to open your configuration file.  It should contain the following fields:
`
CLIENT_SECRET=""
DEVICE_SERIAL_NUMBER=""
CLIENT_ID=""
PRODUCT_ID=""
`
2. Navigate back to the AVS dashboard:  [https://developer.amazon.com/avs/home.html#/avs/home](https://developer.amazon.com/avs/home.html#/avs/home).
2. Click **Manage**. From **Details and management** copy your **Product ID** (no spaces) into the `PRODUCT_ID` field .
3. Select **Security Profile** from the left tab and copy your **Client ID** and **Client Secret**.  
4. Place the **ClientID** and **ClientSecret** into the `CLIENT_ID` and `CLIENT_SECRET` fields.  The device serial number can be any alpha-numeric value (here it's 123456):

example:
`
CLIENT_SECRET="1234567890123456789012345678901234567890123456789012345678901234"
DEVICE_SERIAL_NUMBER="DEV12345"
CLIENT_ID="amzn1.application-oa2-client.12345678901234567890123456789012"
PRODUCT_ID="MY_GREAT_SPEAKER"
`
{:.verify}
### Checkpoint 5

1. Make sure you've saved the 'config.sh' file with your **Device Type ID**, **Device Serial Number**, **Client ID** and **Client Secret** to a text file on your Pi (make sure it is placed your home/pi folder).
