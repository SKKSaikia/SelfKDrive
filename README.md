# Self Driving RC | 🚦 🚘 

Self driving radio controlled car by hacking the electronics and using the magic of Neural Networks. The whole project is sub-categorized as - (i) Input Unit, (ii) Processing Unit & (iii) Output Unit. | <b>Goal :</b> Self- driving and Front Collision avoidance

- <b>Input Unit :</b> Comprises the vision and the input received by the car. Based upon the  input, the neural network decides and takes actions accordingly (actions being steer left, right, stop etc). The Input Unit comprises of Raspberry Pi Camera (For receiving Camera Frames / Vision by the front part of the car); SR04 Ultrasonic Ranging Module HC to receive distance measures from the front part of the car to objects encountered while driving forward. Both the camera and the Ultrasonic sensor are connected to the Raspberry Pi. The Raspberry Pi is connected to a laptop via Wifi and it sends all the data received from the the two inputs to the laptop in real time over Wi-Fi. The Raspberry Pi is being powered by a portable battery onboard the rc car. 

- <b>Processing Unit :</b> The processing section comprises of training and processing the input data with a Neural Network. The Processed input helps give autonomus instructions to the transmitter in real time.

- <b>Output Unit :</b> Arduino is connected to the laptop which picks up the real time direction instructions. The GPIO pins of the arduino is in turn connected to the original transmitter of the RC car. The transmitter is hacked and is soldered to 4 GPIO pins of arduino. Based on the instructions, the rc car moves in real time.

<b>The Overall Flow :</b> Ultrasonic sensor sends distance data and the Raspberry Pi camera sends frames to the Raspberry Pi. The Raspberry Pi sends those data to a laptop via Wifi. Neural Networks in the laptop processes the input data and decides whether to move left, right, forward or to stop ,i.e decides to steer the car based on input frames. Everything happens in real time. The laptop is connected to an Arduino, which is in turn connected to the original transmitter. The transmitter is hacked ( The controls in the transmitter (original left, right, forward or stop) are soldered to 4 GPIO pins of the arduino). Based on the predictions for steering from the Neural Network in the laptop; the transmitter sends instructions accordingly to the receiver in the rc car. The receiver in the RC car wasn't hacked and it connects to the transmitter over 2.4 Ghz.

<img src="https://github.com/SKKSaikia/SelfKDrive/blob/master/Gallery/rc0.jpg" height=232px><a> </a><img src="https://github.com/SKKSaikia/SelfKDrive/blob/master/Gallery/rc1.jpg" height=232px><a> </a><img src="https://github.com/SKKSaikia/SelfKDrive/blob/master/Gallery/rc2.jpg" height=232px><a> </a>

+ Project Updates - [Car chasis](https://youtu.be/zYgcddXkipc) ; [Ultrasonic Sensor Test](https://youtu.be/XntSE13zWPA) ; [Picamera Test](https://youtu.be/fUyVj07Plps)


