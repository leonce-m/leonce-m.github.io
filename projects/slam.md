---
layout: single
title: "Graph-Based SLAM for Formula Student Autonomous Racing"
permalink: /projects/slam/
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/slam/skidpad-planing-onboard.png
  overlay_filter: "0.25"
---

A modular online SLAM system for cone-based autonomous racing, implemented in ROS 2 and C++.

## Overview

This project develops an online, landmark-based graph SLAM system tailored to Formula Student Driverless. It combines high-rate odometry integration with keyframe-based graph optimization and cone landmark mapping.

{% include figure image_path="/assets/images/slam/trackdrive-planning-3d.png" alt="Foxglove 3D view of a Formula Student Driverless SLAM map with keyframes, cones, trajectories, and loop closure state" caption="3D debugging view of the SLAM graph, mapped cones, vehicle trajectory, and runtime diagnostics." %}

## Highlights

- online landmark-based graph SLAM
- continuous pose output between graph updates
- GTSAM backend with iSAM2 and fixed-lag smoothing variants
- uncertainty-aware cone data association
- keyframe-based smoothing, mapping, and loop closure

## Runtime Visualization

The system is designed to be inspected while running, with ROS 2 topics visualized in Foxglove for perception, mapping, localization, and planner behavior. This makes it possible to compare the onboard camera view, cone detections, planned path, graph state, and timing diagnostics in the same debugging workflow.

<div class="video-embed">
  <iframe
    src="https://www.youtube-nocookie.com/embed/kAgbhLv-lVg"
    title="Graph-Based SLAM runtime visualization"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen>
  </iframe>
</div>

{% include figure image_path="/assets/images/slam/skidpad-planing-onboard.png" alt="Onboard Formula Student view with cone detections and a planned skidpad trajectory overlaid" caption="Onboard debugging view with detected cones and a planned skidpad trajectory overlaid on camera data." %}

## Implementation Focus

The SLAM stack emphasizes a practical online formulation for Formula Student courses: maintaining a consistent cone map, smoothing vehicle poses over keyframes, and keeping a usable pose output available between graph updates for downstream planning and control.

## Technologies

C++, ROS 2, GTSAM, Eigen, factor graphs, SE(2), Docker.

## Status

Bachelor's thesis / active development.
