---
title: '8. Launch the Client'

layout: nil
---

{:.steps}
### Terminal Window 2

Open a new terminal window and type the following commands to run the sample app, which communicates with AVS:

	cd ~/Desktop/alexa-avs-sample-app/samples/javaclient && mvn exec:exec

![](assets/avs-pi-3.png)			 

Let's walk through the next few steps relevant to Window 2.

1. When you run the client, a window should pop up with a message that says -

	 *Please register your device by visiting the following URL in a web browser and following the instructions: https://localhost:3000/provision/d340f629bd685deeff28a917. Would you like to open the URL automatically in your default browser?*

	 ![](assets/avs-pi-5.png)

	 Click on **"Yes"** to open the URL in your default browser.

2. If you're running Raspbian Jessie with Pixel desktop (and with Chromium browser), you may get a warning from the browser. You can get around it by clicking on **Advanced -> Proceed to localhost(unsafe)**.

	![](assets/safety-1.png)
	![](assets/safety-2.png)

3. You'll be taken to a Login with Amazon web page. Enter your Amazon credentials.

4. You'll be taken to a Dev Authorization page, confirming that you’d like your device to access the Security Profile created earlier.

	 Click **Okay**.

5. You will now be redirected to a URL beginning with `https://localhost:3000/authresponse` followed by a query string. The body of the web page will say device tokens ready.

	![](assets/avs-device-tokens-ready.png)

6. Return to the Java application and click the OK button. The client is now ready to accept Alexa requests.

	![](assets/avs-click-ok.png)

{:.verify}
### Checkpoint 8

1. Ensure that the client displays a **Bearer Token** 
2. Use the **Listen** button to test push-to-talk functionality. **After the tone**, ask Alexa, "What's the weather in Las Vegas?" If Alexa responds you're ready to move on to the next step.
