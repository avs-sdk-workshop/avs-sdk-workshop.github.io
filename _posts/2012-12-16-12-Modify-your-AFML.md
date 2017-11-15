---
title: '12. Modify your AFML behavior'


layout: nil
---

### Modify your Alexa Focus Manager Library behavior

Suppose you were building a device whose function involved receiving replies from Alexa that you did not want interrupted.  Currently, any time the wake word "Alexa" is invoked, it will interrupt whatever reply was already playing.  This is because the Alexa Focus Manager Library (AFML) gives a higher priority to Speech Recognition than Speech Synthesizer.
\
-only works for "alexa sing me a song" - playing on audioplayer!

For the purpose of this exercise, we're going to switch those priorities and make Alexa the higher priority.

Navigate to FocusManager/src/FocusManager.cpp and edit line 126 so that `channelToAcquire>*foregroundChannel` is changed to `*foregroundChannel>*channelToAcquire` and save the file.

In a terminal, navigate to your SDK's SampleApp/src folder and type `make` to recompile with your new behavior.

Now restart the SampleApp, initiate an interaction, and try to interrupt Alexa.  What happened?

Try running a Unit test again, following the steps as previously described in your Lab Manual.  What happened?

You'll notice the test failed - it's set up to make sure the AFML has the correct priorities.  Any time you make a modification to the SDK, you'll want to run Unit and Integration tests to verify that you haven't broken any critical behavior that might negatively impact the user experience.  

---
