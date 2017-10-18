---
title: '5. Copy Your Credentials'


layout: nil
---

1. Navigate back to the AVS dashboard:  [https://developer.amazon.com/avs/home.html#/avs/home](https://developer.amazon.com/avs/home.html#/avs/home).
2. Click **Manage**. From **Details and management** copy your **Product ID**.
3. Select **Security Profile** from the left nav and copy your **Client ID** and **Client Secret**.
4. Place the following into a text file on your pi with your values entered for each field, and save as config.sh in your home folder (/home/pi). The device serial number can be any alpha-numeric value.:

```
CLIENT_SECRET=""
DEVICE_SERIAL_NUMBER=""
CLIENT_ID=""
PRODUCT_ID=""
```

example:

```
CLIENT_SECRET="1234567890123456789012345678901234567890123456789012345678901234" 
DEVICE_SERIAL_NUMBER="DEV12345"
CLIENT_ID="amzn1.application-oa2-client.12345678901234567890123456789012"
PRODUCT_ID="MY_GREAT_SPEAKER"
```

{:.verify}
### Checkpoint 5

1. Make sure you've saved the file with your **Device Type ID**, **device serial number**, **Client ID** and **Client Secret** to a text file on your Pi (make sure it is placed your home folder).