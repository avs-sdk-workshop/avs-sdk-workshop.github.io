---
title: '9. Launch the Wake Word Engine'


layout: nil
---

{:.steps}
### Terminal Window 3

This project supports two third-party wake word engines: Sensory's TrulyHandsFree and KITT.AI's Snowboy. The **-e** option is used to select the agent and supports two values for engine: **kitt_ai** and **sensory**.

Open a new terminal window and use the following commands to bring up a wake word engine from Sensory or KITT.AI. The wake word engine will allow you to initiate interactions using the phrase "Alexa".

To use the **Sensory** wake word engine, type -

	cd ~/Desktop/alexa-avs-sample-app/samples
	cd wakeWordAgent/src && ./wakeWordAgent -e sensory

or type this to use **KITT.AI**'s wake word engine -

	cd ~/Desktop/alexa-avs-sample-app/samples
	cd wakeWordAgent/src && ./wakeWordAgent -e kitt_ai

![](assets/avs-pi-7.png)

Now you have a working hands-free AVS prototype!

{:.verify}
### Checkpoint 9

1. Say "Alexa". Wait for the **tone**, then say "tell me a joke." If Alexa responds, you have a working prototype. 
