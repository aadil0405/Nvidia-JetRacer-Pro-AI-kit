# Nvidia-JetRacer-Pro-AI-kit

This project focuses on implementing autonomous driving capabilities on the JetRacer Pro AI Kit.
The robot is trained to follow a specific lane, detect and stop at a red sign, and avoid another vehicle placed in its path using computer vision and machine learning techniques.

The project was developed as part of our Computer Vision course.

Features:

1) Lane Following
The JetRacer autonomously follows a predefined lane it was trained on using a vision-based model.

2) Red Sign Detection & Stop
The robot detects a red sign in its field of view and comes to a complete stop for 3 seconds and then continues driving along it's predefined lane.

3) Car Avoidance
When another car is placed on the lane, the JetRacer detects it and performs an avoidance maneuver to continue driving safely. 

4) Manual Driving & Data Collection
Manual control mode used to collect training data for the lane-following model, stop sign detection and obstacle avoidance.

The basic motion, teleoperation and road following codes were already provided to us by JetRacer Wiki (https://www.waveshare.com/wiki/JetRacer_Pro_AI_Kit?srsltid=AfmBOoqF7iE91rC4y-dcaFzcc81nGKchYrRWgNz4CNZ2A2izwW4enjkZ#Road-following).

In order for the bot to drive autonomously along the track, we had to drive the bot manually, move a small position, stop and take a picture of the track using the interactive-regression.ipynb file and the bot's camera. We did around 25-30 laps for every data collection process, i.e road following, stop sign detection and obstacle avoidance. 


