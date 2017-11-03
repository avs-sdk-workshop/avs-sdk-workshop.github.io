---
title: '7. Obtain a refresh token'


layout: nil
---

You now have the SDK installed, but your specific device still needs a **refresh token** in order to enable your client to maintain a connection to the AVS in the cloud.  If you ship a million Alexa-enabled devices, they could all use the same Client ID, Client Secret, and ProductID - but each *individual* device requires a unique refresh token to authenticate with the AVS through Login With Amazon (LWA).

The install process created a few shell scripts for you to launch the application that generates the authorization token (**startauth.sh**) and that starts the sample application (**startsample.sh**)

{:.steps}

1. Copy and paste the following command into a terminal window to navigate to the *avs-sdk* directory and run the **startauth.sh** script:

`cd home/pi/avs-sdk
bash startauth.sh`

2. In your Web Browser, go to [http://localhost:3000](http://localhost:3000)
3. You'll be prompted to log into Amazon to generate the refresh token.
4. Your browser page should show that it succeeded, and the auth server will automatically terminate.  Close the browser window to continue.

    ![refresh token success](../assets/refresh_token.png)


{:.verify}
### Checkpoint 8

1. From the File Manager, navigate to */home/pi/avs-sdk/build/Integration* and open **AlexaClientSDKConfig.json** by right-clicking on it and selecting **Text Editor**.
2. Verify that you have populated fields for everything in the **authDelegate** section, including **refreshToken** (it should be a very long string of characters).
