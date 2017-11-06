---
title: '6. Run the Install Script'


layout: nil
---


### Run the Install Script

You are now ready to run the install script. This will install all dependencies, including the  wake word engine from Sensory.

{:.steps}

To run the script,  open a **terminal** by clicking on the console window in the Pi's toolbar at the upper left of the screen. There should be two scripts in your */home/pi/avs-sdk* directory: **config.sh** that you just populated, and **setup.sh** which uses the data from your config file to run the install script. Copy and paste the following command into your terminal window, and hit return to run the following:

`cd /home/pi/avs-sdk
bash setup.sh config.sh
`

Note if you have made an error in filling out the **config.sh** file with your account-specific information, the script will error out and inform you which field needs to be fixed.  In this event, return to your **security profile** on your Developer page and double-check your copy and paste into **config.sh** was correct.

Once the script is running, you'll be prompted to accept the Sensory agreement during installation.  Hit the return key to scroll through the terms and conditions until prompted for a yes/no.  Type "y" and hit return to continue. Otherwise all steps are covered in the script execution for setup.

If your build was successful, you'll receive a printout of your configuration details (such as Client ID and Client Secret) plus a message informing you that Configuration/Build was successful.

![build success](/assets/build_successful.png)

**Note** for the purposes of this workshop, portions of the script have been pre-built to get your client up and running faster.  If you use this script for an install on a clean OS image, expect it to take around 20 minutes to build.  You can use the text editor to view the contents of the **setup.sh** file. It's a relatively simple script designed to run on a clean install of the Raspbian **stretch** OS.

{:.verify}
### Checkpoint 6

1. Build completed without error output.
