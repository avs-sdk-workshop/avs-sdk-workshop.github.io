---
title: '10. Talk to Alexa'


layout: nil
---

{:.steps}
### Let's Interact with Your Prototype

You can now talk to your Pi by simply saying the wake word "Alexa". Try the following, and watch the output in the terminal window to see the directives and events that flow for each -

* Say "Alexa", then ask "What time is it?"  
* Say "Alexa", then ask "What's the weather in Las Vegas?"  
* Say "Alexa", then say "Set a timer for 5 seconds."
* Say "Alexa", then say "Play BBC news on TuneIn."
* Say "Alexa", then say "Good afternoon."
* Say "Alexa", then say "Tell me a joke."
* Say "Alexa", then ask "What's the meaning of life?"
* Say "Alexa", then say "Sing happy birthday."
* Say "Alexa", then ask "What day of the week does Christmas fall on?"
* Say "Alexa", then ask "Where were you born?"
* Say "Alexa", then ask "Can you rap?"

### Try a Multi-Turn interaction

* Say "Alexa", then ask "Set an alarm for 12:30."  You should receive a response asking you to clarify AM or PM.  If you have DEBUG9 active, scroll up until you see the **Listening...** box - right above that you'll see that the state of the Audio Input Processor has changed from `IDLE` to `EXPECTING_SPEECH` and then `RECOGNIZING` - without requiring a wake word!  In multi-turn interactions, you can continue to speak with Alexa as part of a continuing conversation without starting every phrase with "Alexa".

### Other Multi-Turn interactions to Try

* Say "Alexa, Wikipedia" - you'll have the option of looking up any subject without having to speak the wake word before the subject.


{:.verify}
### Look ma, no more checkpoints!
