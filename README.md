# Person Regressor
A person regressor using Posenet and a CNN regressor model

### Broadcasting Camera To Browser
Actually I dunno how to do it so I just googled it then I found, edited a bit and everything worked fine. (not sure but I guess I found source code from [here](https://www.hackster.io/ruchir1674/video-streaming-on-flask-server-using-rpi-ef3d75))

### Extracting Bodies From Frame
I used Posenet to extract keypoints of body, after extracting I needed to draw rectangle over bodies to make this I made a class named Rectangle to keep data and get some data from it and for the drawing into canvas.

### Training Regressor
I trained regressor with the function "getImageData" of rectangle class after getting it I needed some data to say regressor "what isn't you are likely to" then I made a function called "getGarbages" to get places you are not in it from frame then I fitted the data to regressor.

### Predicting Phase
Program iterates over all bodies to see which body is much likely to you then draws rectangle over you with prediction.

###### Notes
<sub>1. I'm not the best coder in the world there might be some better codes that can do the same thing <sub>I'm still 15 and there is a lot of way to go.</sub></sub>

<sub>Maybe readme file doesn't what you are expecting for so sorry I'm not good at english <sub>so I tried to keep it short and understandable as I can</sub></sub>
