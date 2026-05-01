# Vision-Based Autonomous Driving with Lane and Object Detection
A Project by Aadil Nuckchady, Danial Syed Muhammad, Hussein Dabbous, and Khundker Reshad

<p align="center">
   <img width="323" height="323" alt="551173914-86f2d73e-03a6-49b3-90c3-1d54ffc6dc1f" src="https://github.com/user-attachments/assets/baa42d09-33fc-4f8b-b099-0dacc4dc7ec5" />
   <b>Nvidia-JetRacer-Pro-AI-kit Robot</b>
</p>

This project focuses on implementing autonomous driving capabilities on the JetRacer Pro AI Kit, developed as part of our Computer Vision course.

We chose to train a robot car seeing as autonomous driving is a hot topic today and it's an opportunity to work with hardware unlike anything we've done before. It was a very rewarding experience to see our hard work come to fruition in our demos.

<p align="center">
   <img width="540" height="301" alt="Robot Car All" src="https://github.com/user-attachments/assets/9bbdaf3f-e2ca-46ee-8992-c0decfc8966f" />
</p>

## Features:
Following training using computer vision and machine learning techniques, the robot car is able to do the following:

#### 1) Lane Following
> The JetRacer autonomously follows a predefined lane it was trained on using a vision-based model.

<p align="center">
   <img width="480" height="268" alt="Robot Car Track" src="https://github.com/user-attachments/assets/4707d5aa-b22b-4bd8-adfa-6c0e0c928ed5" />
</p>

#### 2) Red Stop Sign Detection & Stop
> The robot detects a red sign in its field of view and comes to a complete stop for 3 seconds and then continues driving along it's predefined lane.

<p align="center">
   <img width="480" height="268" alt="Robot Car Stop" src="https://github.com/user-attachments/assets/7c7e2c62-2772-47c9-ad31-994163b3e2da" />
</p>

#### 3) Car Avoidance
> When another car is placed on the lane, the JetRacer detects it and performs an avoidance maneuver to continue driving safely. 

<p align="center">
   <img width="480" height="268" alt="Robot Car vs Car" src="https://github.com/user-attachments/assets/34f07cda-d50b-4567-a634-077710ccf4db" />
</p>

## Methodology:
The basic motion, teleoperation, and road following codes were already provided by the [JetRacer Wiki](https://www.waveshare.com/wiki/JetRacer_Pro_AI_Kit).

### Data Collection
In order to collect the data necessary to train the bot to drive autonomously along the track, we had to drive the bot manually, move a small position, stop and take a picture of the track using the _interactive-regression.ipynb_ file and the bot's camera. 

For object detection, we collected images of blocked instances, with the stop sign or the car on the track, as well as images of free instances.

We did around 25-30 laps for every data collection process, i.e road following and obstacle and stop sign detection and avoidance. 

### Lane Following
A regressive model for training for road following with parameter tuning to ensure best performance and responsive autonomous driving, including car throttle for the bot's speed, steering gain to avoid the bot swaying too much or missing turns, and steering bias to align the bot correctly when it's driving straight. Training was performed on the bot's GPU using PyTorch with interactive Jupyter notebooks to save and load model checkpoints easily.

<p align="center">
   <img width="1754" height="937" alt="image" src="https://github.com/user-attachments/assets/40f2bf12-5646-4858-8dfd-ca101f9b4b59" />
</p>

### Object Detection
We created 2 models, one for for automatically stopping with stop sign detection and another for automatically navigating around with obstacle detection. 

<p align="center">
   <img width="2508" height="729" alt="image" src="https://github.com/user-attachments/assets/808d1a0c-3863-4e36-a5b6-a1f1aa2245c6" />
</p>

## Lessons Learned
If we were to do this project again, we would do many things differently with the experience that we now have because of this project. 

Firstly, we would've spent more time on training. Though the truth is the majority of the time spent on this project was allotted for collecting images, the robot car's driving and obstacle detection and avoidance could definitely be improved further.

Following up on the previous point, we would also train in different environments. One issue we ran into was the bot driving strangely in different lighting situations. More data collected would once again improve its performance.

Finally, from a team environment perspective, as we are now more familiar with how to approach a project like this, we would divide tasks more efficiently and trust the process more, especially in new and unfamiliar projects and environments. 

So, we take our experience with us and hope to continue to be able to apply our knowledge in future projects with greater confidence and efficiency.
