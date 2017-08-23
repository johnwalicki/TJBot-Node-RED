# TJBot Node-RED Examples
These TJBot Node-RED flows are an easy way to get started with bringing TJBot to Life.
Node-RED is a great way to teach developers about programming without dropping them down into Node.js code.

These TJBot Node-RED recipes showcase:
* Twitter Tone Analysis (blinks the LED colors and waves his arm on joyful tweets).
* Speech to Text to control the LED color and waves his arm
* Weather report
* TJBot LED Party is a simple flow that randomly generates colors / blinks the TJBot NeoPixel
* Watson Visual Recognition Image Classification and Text Extraction using a Pi Camera 

There are screenshots posted so you can see the Node-RED flows in the Pictures directory.

If you're interested in trying these recipes on your TJBot / Raspberry Pi, find them here:
https://github.com/johnwalicki/TJBot-Node-RED/flows

## Node-RED flows in this repository:
This flow receives a Twitter feed and calls Tone Analyzer
![TJBot Twitter Tone Analysis flow](/pictures/TJBotTweetToneAnalysisBlinkLEDWave.png?raw=true "TJBot Twitter Analyzer flow")
This flow records speech from the browser microphone and controls the LED color and waves his arm.
![TJBot Speech to Text Control the LED color and Wave flow](/pictures/TJBotSetColorWaveviaSpeechCommand.png?raw=true "TJBot Speech to Text flow")
This flow announces the current Weather Conditions using Text to Speech.
![TJBot Announce the Weather conditions using Text to Speech flow](/pictures/TJBotWeatherForecastTTSAnnouncements.png?raw=true "TJBot Speech to Text flow")
TJBot loves to party so I created a simple flow that randomly generates colors and blinks the TJBot NeoPixel.
![TJBot LED Party flow](/pictures/TJBotLEDParty.png?raw=true "TJBot LED Party flow")
I've taught TJBot to read and identify images by using Watson Visual Recognition and Text Extraction.
![TJBot Visual Recognition Image Classification Text Extraction flow](/pictures/TJBot-CameraFlow.png?raw=true "TJBot Watson Vision flow")
A browser screenshot of the "TJBot Cam" Node-RED Dashboard that shows Image Classification.
![TJBot Visual Recognition Image Classification Node-RED Dashboard](/pictures/TJBot-CameraResults-racecar.png?raw=true "TJBot Node-RED Dashboard Racecar")
A browser screenshot of the "TJBot Cam" Node-RED Dashboard that shows Text Extraction.
![TJBot Visual Recognition Image Classification Node-RED Dashboard](/pictures/TJBot-CameraResults-Party.png?raw=true "TJBot Node-RED Dashboard Party Text Extraction")

## Node-RED Dependencies and Install Instructions
These flows use a variety of Node-RED nodes that you might need to install on your Raspberry Pi.
* node-red-node-watson
* node-red-dashboard
* node-red-contrib-camerapi
* node-red-contrib-micropi
* node-red-contrib-speakerpi
* node-red-node-base64
* node-red-contrib-play-audio
* node-red-node-pi-neopixel
* node-red-node-weather-underground

Here is a one liner that will install all of these node-red nodes onto your Raspberry Pi.  Remember to restart the Node-RED service or reboot the Raspberry Pi after the installs complete.
     `$ sudo npm -g install node-red-node-watson node-red-dashboard node-red-contrib-camerapi node-red-node-base64 node-red-contrib-play-audio node-red-contrib-micropi node-red-node-pi-neopixel node-red-node-weather-underground node-red-contrib-speakerpi`

