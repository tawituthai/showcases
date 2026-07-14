# Hardware & Robotics Portfolio — Tawit Uthaicharoenpong

Controls & electrical engineer, 15+ years building safety-critical hardware for autonomous
vehicle fleets. Currently pursuing a Master's in Space Systems Engineering (Johns Hopkins, in
progress), applying that background to spacecraft power, avionics, and robotics subsystems.

This repo documents four hardware/robotics projects — production and personal — with an eye
toward how each maps to spacecraft subsystem design. Each project is real hardware I built and
deployed, not a paper design, unless noted otherwise.

**Contact:** iamtawit@gmail.com · [LinkedIn](https://www.linkedin.com/in/tawit-u/)

---

## Projects

| # | Project | Domain | Relevance |
|---|---|---|---|
| 01 | [Power Distribution Unit](projects/01-power-distribution-unit/) | Power electronics | Priority power path arbitration, output ORing for regulator redundancy, current-sensed switched outputs — same functional pattern as spacecraft LCL-based power distribution |
| 02 | [CAN-Bus General-Purpose I/O Module](projects/02-can-io-module/) | Distributed avionics | Digital/analog I/O over a shared CAN bus, deployed as 3-4 reused units across multiple vehicle projects — modular, distributed I/O architecture |
| 03 | [Drive-by-Wire Auto/Manual Switch](projects/03-drive-by-wire-switch/) | Control authority & safety | Production automotive control-authority arbitration between autonomy and human control — same problem crewed spacecraft manual-override systems solve |
| 04 | [Differential-Drive SLAM Robot](projects/04-slam-robot/) | Robotics / perception | ROS2, IMU + LiDAR + camera sensor fusion, SLAM/mapping, dual auto/manual control via SBUS — closest of the four to proximity-operations and relative-navigation problems |

---

## How this is organized

Each project folder contains:
- `README.md` — problem, architecture, design decisions, and space-systems relevance
- `assets/` — schematics, diagrams, photos, and video clips

This is a documentation repo, not a build/run repository — it exists to show engineering
reasoning and real hardware, not to be cloned and executed.
