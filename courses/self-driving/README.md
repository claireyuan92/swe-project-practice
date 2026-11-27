# Course 2 — Self-Driving Car Project

Build a self-driving stack in simulation: perceive the road, detect objects,
and plan motion. You start with classical computer vision (lane detection in
OpenCV), then move to learned perception and reinforcement learning for
motion planning.

## Tech stack

Python · OpenCV · TensorFlow · CARLA simulator · Apollo

## What you build

A CARLA-based autonomous-driving pipeline: real-time lane detection, object
detection (cars, pedestrians, bikes), traffic-light recognition, and adaptive
speed control — plus a DeepTraffic motion-planning experiment.

## Videos

1. **Autonomous Self Driving Car Part 3 | Carla simulator** (~53 min, en)
https://www.youtube.com/watch?v=m1vctOrYrTY
TensorFlow object detection (cars, pedestrians, bikes) and OpenCV lane detection inside the CARLA simulator, including TF Object Detection API setup.
2. **MIT 6.S094: Deep Reinforcement Learning** (~55 min, en, Lex Fridman)
https://www.youtube.com/watch?v=MQ6pP65o7OM
MIT lecture 3 of Deep Learning for Self-Driving Cars — the AI pipeline from sensors to action, RL, deep RL, AlphaGo, and the DeepTraffic motion-planning simulator.
3. **MIT 6.S094: Deep Reinforcement Learning for Motion Planning** (~1 hr, en, Lex Fridman)
https://www.youtube.com/watch?v=QDzM8r3WgBw
ML, Q-learning, and deep RL applied to motion planning, using the DeepTraffic simulation.
4. **Lane Detection for Self Driving Cars (Real-Time Lane Detection using OpenCV)** (en, Analytics Vidhya)
https://www.youtube.com/watch?v=sYhZbhT-Smw
Hands-on OpenCV/Python lane detection — frame masking, thresholding, Hough line transform on driving video, no deep learning needed.
5. **OpenCV Lane Detection Tutorial using Python – Intro to Self Driving Cars** (en)
https://www.youtube.com/watch?v=CvJN_jSVm30
Beginner walkthrough of lane detection with pure OpenCV (Canny edges, region of interest, Hough lines), code explained line by line.

## Docs, articles & repos

- **CARLA Simulator — Official Documentation** (en)
https://carla-ue5.readthedocs.io/en/latest/
Official CARLA docs (Unreal Engine, Python/C++ APIs, sensors, maps) — quick start, first-steps tutorial, Python API and sensor references.
- **PreritSM/Carla_Autonomous_Driving** (GitHub, en)
https://github.com/PreritSM/Carla_Autonomous_Driving
Complete CARLA 0.9.15 autonomous-driving system — YOLO11n object detection, UFLD lane detection, traffic-light recognition, adaptive speed control, with training notebooks and demo videos.
- **Self-Driving Car Fundamentals: Featuring Apollo** (Udacity × Baidu, free course, en)
https://www.classcentral.com/course/udacity-self-driving-car-fundamentals-featuring-apollo-11639
Free course by Sebastian Thrun covering the full Apollo stack — HD maps, localization, perception, prediction, planning, control.
- **2024年B站最好的自动驾驶系列知识课程** (Bilibili series, zh)
https://www.bilibili.com/video/BV1Mv421C7QN/
12-lesson Chinese course from beginner to advanced — perception practice, visual localization, HD maps, prediction, path planning, control theory, RL-based driving.
- **自动驾驶资料合集：视频、书籍与开源项目** (Tencent Cloud Developer Community, zh)
https://cloud.tencent.com/developer/article/2249254?policyId=1004
Curated Chinese roundup of self-driving courses (Apollo/Udacity, Coursera Toronto, 深蓝学院 SLAM), books, and open-source projects (Apollo, Autoware).
