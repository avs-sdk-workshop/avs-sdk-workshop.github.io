---
title: '7. Launch the Companion Service'


layout: nil
---

{:.steps}
### Terminal Window 1
1. In the terminal window, from the avs-sdk directory, run `./startauth.sh`
2. In the browser, go to http://localhost:3000
3. Log into AMazon to generate the refresh token.
4. Your browser page should show that it succeeded, and the auth server will automatically terminate.

{:.verify}
### Checkpoint 7

1. From the terminal window in the avs-sdk directory, type `cat ./Integration/AlexaClientSDKConfig.json` and make sure the refresh token value is set.