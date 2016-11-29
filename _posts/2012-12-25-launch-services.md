---
title: '5. Launch Services'


layout: nil
---

### Run Your Node.js Server, Sample App and Wake Word Engine

Now that installation is complete, you'll need to run three commands in **3 separate terminal windows**:

1. **Terminal Window 1**: to run the web service for authorization
2. **Terminal Window 2**: to run the sample app to communicate with AVS
3. **Terminal Window 3**: to run the wake word engine which allows you to start an interaction using the phrase "Alexa".

**Note:** These commands must be run in order.

---

#### Terminal Window 1
Open a new terminal window and type the following commands to bring up the web service which is used to authorize your sample app with AVS:

	cd ~/Desktop/alexa-avs-sample-app/samples/companionService && npm start

The server is now running on port 3000 and you are ready to start the client.		

See [API Overview > Authorization](https://developer.amazon.com/public/solutions/alexa/alexa-voice-service/content/avs-api-overview#authorization) to learn more about authorization.

---

#### Terminal Window 2

Open a new terminal window and type the following commands to run the sample app, which communicates with AVS:

	cd ~/Desktop/alexa-avs-sample-app/samples/javaclient && mvn exec:exec

![](assets/avs-pi-3.png)			 

See [API Overview > Interfaces](https://developer.amazon.com/public/solutions/alexa/alexa-voice-service/content/avs-api-overview#interfaces) to learn more about the messages sent to/from AVS.

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

---

#### Terminal Window 3

This project supports two third-party wake word engines: Sensory's TrulyHandsFree and KITT.AI's Snowboy. The **-e** parameter is used to select the agent and supports two values for engine: **kitt_ai** and **sensory**.

Open a new terminal window and use the following commands to bring up a wake word engine from Sensory or KITT.AI. The wake word engine will allow you to initiate interactions using the phrase "Alexa".

To use the **Sensory** wake word engine, type -

	cd ~/Desktop/alexa-avs-sample-app/samples
	cd wakeWordAgent/src && ./wakeWordAgent -e sensory

or type this to use **KITT.AI**'s wake word engine -

	cd ~/Desktop/alexa-avs-sample-app/samples
	cd wakeWordAgent/src && ./wakeWordAgent -e kitt_ai

![](assets/avs-pi-7.png)

Now you have a working hands-free AVS prototype!

Use the following resources to learn more about available wake word engines:

* [Sensory](https://github.com/Sensory/alexa-rpi)
* [KITT.AI](https://github.com/Kitt-AI/snowboy)
