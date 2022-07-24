# Setup
## What you will need
* Embedded Computer: Raspberry Pi 3 B+ or better
* USB sound card
* SD card
* Microphone
* LED
* 150 ohm resistor
* Logic 2 relay module

## Setting up your embedded computer
we will be using Python3, so if you are using Raspberry pi as your embedded computer, the raspberry pi uses python2 on default.
Check python ver. on your embedded computer

on the terminal, run  
``` 
$ python --version 
```

if it doesnt show "python3"

then install it using this,
```
$ sudo update-alternatives--install/usr/bin/python python/usr/bin/python3 10
```


then, install python IDLE
```
$ sudo apt install python 3 idle3
```
this may take few seconds to install.



installing required packages for speech recognition,
```
$ pip install SpeechRecognition
```
installing it may take few minutes

now, its ready to recognize speech and convert it to text, except that python is not recognizing the microphone inputs.

so, install the audio recognition package for python to recognize the microphone
```
$ sudo apt-get install python-pyaudio python3-pyaudio
```

lastly, make sure you have the flac encoder, since we will be using google web speech API.
if you are working on a raspberry pi, you most likely dont.

to install it
```
$ sudo apt-get install flac
```
installation will take some time.
and thats it!

You can copy and run the python code provided, on your embedded computer.
