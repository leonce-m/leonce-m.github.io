---
layout: page
title: Graph-Based SLAM
permalink: /projects/slam/
---

# Graph-Based SLAM for Formula Student Autonomous Racing

A modular online SLAM system for cone-based autonomous racing, implemented in ROS 2 and C++.

## Overview

The system combines high-rate odometry integration with keyframe-based graph optimization and landmark mapping. It is designed around the constraints of Formula Student Driverless, where the vehicle estimates its pose and builds a map from sparse cone detections.

## Highlights

- online landmark-based graph SLAM
- continuous pose output between graph updates
- GTSAM backend with iSAM2 and fixed-lag smoothing variants
- uncertainty-aware cone data association
- keyframe-based graph construction and loop closure

## Technologies

C++, ROS 2, GTSAM, Eigen, factor graphs, SE(2), Docker

## Status

Bachelor's thesis / active development
