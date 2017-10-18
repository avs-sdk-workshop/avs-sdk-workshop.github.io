---
title: '6. Run the Install Script'


layout: nil
---

{:.steps}
### Run the Install Script

You are now ready to run the install script. This will install all dependencies, including the  wake word engine from Sensory.

To run the script, open **terminal**. There should be two scripts in your home directory, config.sh that you just created, and setup.sh that was already there. Run the following:

```
mkdir avs-sdk
cp *.sh avs-sdk
cd avs-sdk
./setup.sh config.sh
```

*You'll be prompted accept the Sensory agreement during installation. Otherwise all steps are covered in the script execution for setup.*

{:.verify}
### Checkpoint 6

1. Build completed without error output.
2. Verify that there are two script files created, `startauth.sh` and `startsample.sh`




