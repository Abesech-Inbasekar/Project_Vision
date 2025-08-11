# Project Vision – Smart Mobility Aid for Visually Impaired

## Overview
A wearable vision module and tactile gripper system to assist visually impaired individuals in detecting and localizing nearby obstacles in real time.

## Objective
Enhance mobility and safety for visually impaired users by combining stereo vision depth mapping with a tactile feedback gripper.

## Methodology
- **Vision Module**
  - Stereo camera calibration and rectification using OpenCV.
  - Depth map generation via triangulation and disparity calculation.
  - MaxPooling-inspired FPS optimization.
  - Denoising and object localization without heavy deep learning reliance.
- **Gripper Module**
  - 3x3 grid of spring-loaded pins mapped to depth map pools.
  - Cylinder–ramp lock–release mechanism for selective pin actuation.
  - Bluetooth communication between vision module (Jetson Nano) and gripper (Arduino).

## Tools & Tech
- Jetson Nano, Arduino
- OpenCV, Python
- CAD design for gripper components

## Results
- Real-time depth localization without GPU-heavy object detection.
- Intuitive tactile feedback mapping objects to user’s palm.

## References
- [YOLO Object Detection](https://pjreddie.com/darknet/yolo/)
- [Stuff Made Here – Tactile Feedback Inspiration](https://youtu.be/8Au47gnXs0w)
