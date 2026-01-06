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
