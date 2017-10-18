---
title: '8. Obtain a refresh token'


layout: nil
---

The install process created a few shell scripts for you to launch the application that generates the authorization token (startauth.sh) and that starts the sample application (startsample)

{:.steps}

1. In the terminal window, from the avs-sdk directory, run **./startauth.sh**
2. In the browser, go to http://localhost:3000
3. Log into Amazon to generate the refresh token.
4. Your browser page should show that it succeeded, and the auth server will automatically terminate.

{:.verify}
### Checkpoint 8

1. From the terminal window in the avs-sdk directory, type **cat ./Integration/AlexaClientSDKConfig.json** and make sure the refresh token value is set in the configuration.