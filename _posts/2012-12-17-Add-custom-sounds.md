---
title: 'Add a Customized Sound on State Change'


layout: nil
---

### Modify your UImanager file

Navigate to SampleApp/src/ and open UIManager.cpp with a text editor.

At the top, add `#include <cstdlib>`

Lower down on line 207 in the `printState()` function, where it says `case DialogUXState::LISTENING:` add the following command:

`system(play /home/pi/CustomSounds/ding.wav)`

Then, rebuild the sample app by navigating to SampleApp/src in a terminal and typing `make`

Now, every time the wake word is spoken and Alexa's state changes to "listening" you should hear your custom sound.  Experiment with different states and sounds!
---
