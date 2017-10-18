---
title: '9. Launch the Client'

layout: nil
---

{:.steps}

The sample application is in the folder **SampleApp/src** in the **build** directory. There is a shell script to start it with the correct options called **startsample.sh**. To see how it is being started, simply from the build directory:
`
cat startsample.sh
`
You can see that it is starting with the highest debug level, **DEBUG9**. If you want to reduce output, simply change that to a lower number or remove it altogether. For starters though leave it at the highest level so you can see what is going on behind the scenes.

## Terminal Window

1. run **./startsample.sh**
2. You should see the following, if you don't, please ask for help:

<TODO: insert a sucessful start screen>

{:.verify}

### Checkpoint 9

1. Say "Alexa". Wait for the **tone**, then say "tell me a joke." If Alexa responds, you have a working prototype.