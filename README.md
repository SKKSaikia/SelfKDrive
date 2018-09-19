# Self Driving RC | 🚦 🚘 

Self driving radio controlled car by hacking the electronics and using the magic of Neural Networks. The whole project is sub-categorized as - (i) Input Unit, (ii) Processing Unit & (iii) Output Unit.

- <b>Input Unit :</b> Comprises the vision and the input received by the car. Based upon the processed input, the neural networks decides and takes actions accordingly (actions being steer left, right, stop). The Input Unit comprises of Raspberry Pi Camera (For Camera Frames / Vision received by the front part of the car); SR04 Ultrasonic Ranging Module HC to receive distance measures from the car to front objects encountered while driving forward. Both the camera and the Ultrasonic sensor are connected to the Raspberry Pi. The Raspberry Pi is connected to a laptop via Wifi and it sends all the Data received from the the two inputs to the laptop in real time over Wi-Fi. The Raspberry Pi is being powered with a portable battery onboard the rc car. 

<strong>Input Unit: </strong> The Car  + Raspberry pi + Ultrasonic Sensor + Pi-Camera
<strong>Processing Unit: </strong> Computer + OpenCV (py)
<strong>Output Unit: </strong>Arduino + Transmitter Chip

+ For Object detection  - haar cascade classifier
+ Video Update 1 - Car chasis - https://youtu.be/zYgcddXkipc
+ Video Update 2 - Ultrasonic Sensor Test - https://youtu.be/XntSE13zWPA
+ Video Update 3 - Picamera Test - https://youtu.be/fUyVj07Plps

+ Input Unit Tested ++
+ Processing Code Ready 

Next - Hack/Soldering the 4 direction pins of 2.4 Ghz transmitter to GPIO pins of Arduino
Still working on the project.
