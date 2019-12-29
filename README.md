# Person Regressor
A person regressor using Posenet and a CNN regressor model

### Broadcasting Camera To Browser
Actually, I don't know how to do it so I just googled it then I found, edited a bit and everything worked fine. (not sure but I guess I found source code from [here](https://www.hackster.io/ruchir1674/video-streaming-on-flask-server-using-rpi-ef3d75))

### Extracting Bodies From Frame
I used Posenet to extract key points of the body, after extracting I needed to draw a rectangle over bodies. To achieve this I made a class named Rectangle to keep data and get some data from it and for the drawing into the canvas.

### Training Regressor
I trained regressor with the function "getImageData" of rectangle class after getting it I needed some data to say regressor "what you aren't likely to" then I made a function called "getGarbages" to get places you are not in it from the frame then I fitted the data to regressor.

### Predicting Phase
Program iterates over all bodies to see which body is much likely to you then draws rectangle over you with prediction.

###### Notes
<sub>1. I'm not the best coder in the world there might be some better codes that can do the same thing <sub>I'm still 15 and I'm really bad at JS.</sub></sub>

<sub>Maybe the readme file wasn't what you were expecting. I'm not good at English<sub>so I tried to keep it short and understandable as I can</sub></sub>
