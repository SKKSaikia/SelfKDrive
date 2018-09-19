# Self Driving RC | 🚦 🚘 

Self driving radio controlled car by hacking the electronics and using the magic of Neural Networks. The whole project is sub-categorized as - (i) Input Unit, (ii) Processing Unit & (iii) Output Unit.

- <b>Input Unit :</b> Comprises the vision and the input received by the car. Based upon the  input, the neural network decides and takes actions accordingly (actions being steer left, right, stop etc). The Input Unit comprises of Raspberry Pi Camera (For receiving Camera Frames / Vision by the front part of the car); SR04 Ultrasonic Ranging Module HC to receive distance measures from the front part of the car to objects encountered while driving forward. Both the camera and the Ultrasonic sensor are connected to the Raspberry Pi. The Raspberry Pi is connected to a laptop via Wifi and it sends all the data received from the the two inputs to the laptop in real time over Wi-Fi. The Raspberry Pi is being powered by a portable battery onboard the rc car. 

- <b>Processing Unit :</b> The processing section comprises of training and processing the input data with a Neural Network. The Processed input helps give autonomus instructions to the transmitter in real time.

- <b>Output Unit :</b>Arduino is connected to the laptop which picks up the real time direction instructions. The GPIO pins of the arduino is in turn connected to the original transmitter of the RC car. The transmitter is hacked and is soldered to 4 GPIO pins of arduino. Based on the instructions, the rc car moves in real time.

<b>The Overall Flow :</b>


+ For Object detection  - haar cascade classifier
+ Video Update 1 - Car chasis - https://youtu.be/zYgcddXkipc
+ Video Update 2 - Ultrasonic Sensor Test - https://youtu.be/XntSE13zWPA
+ Video Update 3 - Picamera Test - https://youtu.be/fUyVj07Plps

+ Input Unit Tested ++
+ Processing Code Ready 

Next - Hack/Soldering the 4 direction pins of 2.4 Ghz transmitter to GPIO pins of Arduino
Still working on the project.
