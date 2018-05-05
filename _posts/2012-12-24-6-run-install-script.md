---
title: '5. Run the Install Script'


layout: nil
---


### Run the Install Script

You are now ready to run the install script. This will install all dependencies, including the **Wake Word Engine** (WWE) from Sensory.  The WWE compares your captured audio to an onboard model of a wake word (in this case "Alexa") and will initiate the connection to send captured audio to the AVS when triggered.

To run the install script, open a **terminal** by clicking on the console window in the Pi's toolbar at the upper left of the screen. There should be two scripts in your */home/pi/* directory: **config.txt** that you just populated, and **setup.sh** which uses the data from your config file to run the install script. Copy and paste the following command into your terminal window, and hit return:

```
cd /home/pi/
sudo bash setup.sh config.txt
```

Type **AGREE** and return when prompted.

If you have made an error in filling out the **config.txt** file with your account-specific information, the script will error out and inform you which field needs to be fixed.  In this event, return to your **security profile** on your Developer page and double-check your copy and paste into **config.txt** was correct.

If your build was successful, you'll receive a printout of your configuration details (such as Client ID) plus a message informing you that Configuration/Build was successful.

![build success](/assets/build_successful.png)




