---
title: '4. Run the Install Script'


layout: nil
---

### Update the Install Script with Your Credentials

Before you run the install script, you need to update the script with the credentials that you got in step 3:  

* `ProductID`
* `ClientID`
* `ClientSecret`

<<IMAGE_HERE>>

Type the following into your **terminal**:

	cd ~/Desktop/alexa-avs-sample-app && nano automated_install.sh

![](assets/update-script.png)

Replace the values for **ProductID**, **ClientID** and **ClientSecret** with your credentials from Step 3.

Your updates should look something like this:

* `ProductID="RaspberryPi3"`    
* `ClientID="amzn.xxxxx.xxxxxxxxx"`    
* `ClientSecret="4e8cb14xxxxxxxxxxxxxxxxxxxxxxxxxxxxx6b4f9"`  

Type **ctrl-X** and then **Y**, and then press Enter to save the changes to the file.

### Run the Install Script

You are now ready to run the install script. This will install all dependencies, including the two wake word engines from Sensory and KITT.AI.

**Note:** The install script will install all project files in the folder that the script is run from.

To run the script, open **terminal** and navigate to the folder where the project was cloned. Then run the following command:

	cd ~/Desktop/alexa-avs-sample-app && . automated_install.sh

You'll be prompted to answer a few simple questions. These help to ensure that you've completed all necessary prerequisites before continuing.

For this workshop, please select the following:
