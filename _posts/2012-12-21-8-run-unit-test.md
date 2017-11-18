---
title: '9. Run unit test'


layout: nil
---
This assumes the build is in the directory created by the script (avs-sdk).

{:.steps}

#### Unit Tests

1. For this workshop, tests have been pre-built to save time.  Go to the terminal window, and run the following steps to execute the series of Unit tests on your prototype.  If you have your earbuds or speakers in, you'll hear Alexa run through a series of audio tests as well as functional tests.

`cd /home/pi/avs-sdk/build
make all test
`

Your test should show success, with the exception of a few Sensory WWE fails.  As a developer, any time you modify the client's on-device software you should run Unit Test to ensure nothing was unintentionally broken.  Now you're ready to launch your client!
 
<add picture of success>
