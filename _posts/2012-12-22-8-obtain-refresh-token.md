---
title: '8. Obtain a refresh token'


layout: nil
---
You now have the SDK installed, but your specific device still needs a *refresh token* in order to enable your client to maintain a connection to the AVS in the cloud.  

The install process created a few shell scripts for you to launch the application that generates the authorization token (startauth.sh) and that starts the sample application (startsample)

{:.steps}

1. Open a terminal window.  Copy and paste the following command into terminal to navitage to the avs-sdk directory and run the **startauth.sh** script:

`cd home/pi/avs-sdk/build/Integration
bash startauth.sh`

2. In the browser, go to http://localhost:3000
3. Log into Amazon to generate the refresh token.
4. Your browser page should show that it succeeded, and the auth server will automatically terminate.  Close the browser window to continue.

{:.verify}
### Checkpoint 8

1. From the File Manager, navigate to **/home/pi/avs-sdk/build/Integration** and open **AlexaClientSDKConfig.json** by right-clicking and selecting **Text Editor**.
2. Verify that you have populated fields for everything in the **"authDelegate"** section, including **"refreshToken"** (it should be a very long string of characters).
