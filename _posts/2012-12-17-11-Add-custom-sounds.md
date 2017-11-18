---
title: '11. Add a Customized Sound on State Change'


layout: nil
---

### Modify your UImanager file

Navigate to /home/pi/avs-sdk/avs-device-sdk/SampleApp/src/ and open UIManager.cpp with a text editor.

At the top, add `#include <cstdlib>`

Near the bottom of the file in the `printState()` function, where it says `case DialogUXState::LISTENING:` add the following command:

`system("play /home/pi/CustomSounds/ding.wav")`

Don't forget to save your text file before closing it!

Then, rebuild the sample app:
Open a terminal and navigate to /home/pi/avs-sdk/build/SampleApp/ in a terminal and type `make`

After it successfully rebuilds (you should see SampleApp recompile) then navigate back to the /home/pi/avs-sdk directory and relaunch

Now, every time the wake word is spoken and Alexa's state changes to "listening" you should hear your custom sound.  Your /home/pi/CustomSounds folder has several different .wav files - experiment with different sounds at various states in the UI manager!

Your customers will expect their experience to be consistent across many Alexa-enabled devices.  You can learn best practices for implementing visual and audio cues on your device by visiting our [AVS UX Design overview page](https://developer.amazon.com/docs/alexa-voice-service/ux-design-overview.html).

---
