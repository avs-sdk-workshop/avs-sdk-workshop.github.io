---
title: '6. Run the Install Script'


layout: nil
---

{:.steps}
### Update the Install Script with Your Credentials

We are now ready to run the install script, but before we do that we need to make some adjustments to the script.

First, from the Desktop open the **alexa-avs-sample-app** folder. Then right-click on **automated_install.sh** and select **Text Editor**. In your text editor, select **Options** from the top nav and enable **Line Numbers**.

Now that you've got the script open in text editor, we need to enter your credentials. Paste the values for **ProductID**, **ClientID** and **ClientSecret** with your credentials that you copied in the previous step.

![](assets/nano_creds.png)

Your updates should look something like this:

* `ProductID="RaspberryPi3"`    
* `ClientID="amzn.xxxxx.xxxxxxxxx"`    
* `ClientSecret="4e8cb14xxxxxxxxxxxxxxxxxxxxxxxxxxxxx6b4f9"`  

Last, you'll need to comment out lines 403 through 409. Your file should look exactly like this:

```
# Install dependencies
# echo "========== Update Aptitude ==========="
# sudo apt-get update
# sudo apt-get upgrade -y

# echo "========== Installing Git ============"
# sudo apt-get install -y git
```

{:.steps}
### Run the Install Script

You are now ready to run the install script. This will install all dependencies, including the two wake word engines from Sensory and KITT.AI.

To run the script, open **terminal** and navigate to the folder where the project was cloned. Then run the following command:

	cd ~/Desktop/alexa-avs-sample-app && . automated_install.sh

{:.verify}
### Checkpoint 6
You'll be prompted to answer a few simple questions. These help to ensure that you've completed all necessary prerequisites before continuing.

For this workshop, you'll need to:

1. Agree to AVS Terms and Conditions
2. Confirm you have an Amazon developer account
3. Validate that your Product ID, Client ID, and Client Secret are accurate
4. Type **Y** when asked for audio output, to choose 3.5mm audio jack
5. Type **Y** when asked to enable Alexa wake word detection
