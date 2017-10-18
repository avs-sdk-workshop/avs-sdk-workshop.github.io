---
title: '8. Launch the Client'

layout: nil
---

{:.steps}

The sample application is in the folder `SampleApp/src` in the `build` directory. There is a shell script to start it with the correct options called `startsample.sh`. To see how it is being started, simply `cat startsample.sh` in the build directory. You can see that it is starting with the highest debug level, `DEBUG9`. If you want to reduce output, simply change that to a lower number or remove it altogether. For starters though leave it at the highest level so you can see what is going on behind the scenes.

In the terminal window, simply run `./startsample.sh` to start the sample running. You should see the following, if you don't, please ask for help:

<TODO: insert a sucessful start screen>

{:.verify}

### Checkpoint 8

1. Say "Alexa". Wait for the **tone**, then say "tell me a joke." If Alexa responds, you have a working prototype.