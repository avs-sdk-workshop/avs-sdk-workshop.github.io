---
title: '7. Obtain a refresh token'


layout: nil
---
When you run the sample app for the first time, you'll need to authorize your client for access to AVS.

Initialize the sample app by pasting or typing the following command into your terminal:


```
cd home/pi/
sudo bash startsample.sh
```

Wait for the sample app to display a message like this:

######################################################
#       > > > > > NOT YET AUTHORIZED < < < < <       #
######################################################

############################################################################################
#     To authorize, browse to: 'https://amazon.com/us/code' and enter the code: {XXXX}     #
############################################################################################

 Use a browser to navigate to the URL specified in the message from the sample app.
    Authenticate using your Amazon user credentials.
    Enter the code specified in the message from sample app.
    Select “Allow”.
Wait (it may take as long as 30 seconds) for CBLAuthDelegate to successfully get an access and refresh token from Login With Amazon (LWA). This may take At this point the sample app will print a message like this:

########################################
#       Alexa is currently idle!       #
########################################

You are now ready to use the sample app. The next time you start the sample app, you will not need to go through the authorization process.

