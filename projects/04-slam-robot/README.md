# Differential-Drive SLAM Robot — ROS2, IMU/LiDAR/Camera Fusion

**Status:** Personal project, built and operational

## Overview
<!-- What the platform is, what it's used for/demonstrates. -->

## Architecture

![Architecture diagram](assets/architecture-diagram.png)

<!-- Diagram: sensor stack (IMU, LiDAR, camera) → ROS2 nodes → SLAM stack → drive controller,
     plus the SBUS receiver path for manual override. -->

### Design decisions
- **Sensor fusion / SLAM approach:** <!-- LiDAR-based, visual, or fused — which SLAM package/approach used -->
- **Auto/manual switching via SBUS:** <!-- same control-authority pattern as the drive-by-wire project, at RC/hobbyist scale -->
- **Differential drive kinematics:** <!-- any notable tuning or control loop details -->

## Why this matters for space robotics

IMU/LiDAR/camera sensor fusion and SLAM are the terrestrial analog of proximity-operations and
relative-navigation problems in space robotics — approach and characterization of a target for
docking or capture, or rover terrain-relative navigation. This project is the most direct,
though smallest-scale, connection in this portfolio to that class of problem.

## Specs
<!-- Sensor models, ROS2 version, compute platform, drive specs. -->

## Media
<!-- Video clips of SLAM mapping in action, photos of the platform, RViz screenshots. -->
