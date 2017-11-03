---
title: '8. Launch the Client'

layout: nil
---

{:.steps}

The sample application is in the folder */home/pi/avs-sdk/build/SampleApp/src*. In order to start it, we'll use a shell script called **startsample.sh**. To see how it is being started, you can use File Manager to navigate to */home/pi/avs-sdk* and use your text editor to view the contents :

![debug](../assets/startsample_debug9.png)

You can see that it is starting with the highest debug level, **DEBUG9**.  This will display status messages in the console as you communicate with Alexa.  If you want to reduce output, simply change that to a lower number or remove it altogether. For starters, try it at the highest level so you can see what is going on behind the scenes.

## Terminal Window

1. From a terminal window, run **startsample.sh** to launch the Sample App.

`cd /home/pi/avs-sdk
bash startsample.sh`

2. You should see the following screen:

![app launched](../assets/app_launched.png)

{:.verify}
### Checkpoint 9

1. Say "Alexa". You should see the console status change to **Listening**, then say "tell me a joke." If Alexa responds, you have a working prototype.  You should see a series of status changes annotated by your level of DEBUG set in the above

![app running](../assets/app_running.png)
