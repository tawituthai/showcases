# General-Purpose I/O Module — CAN Bus Controlled

**Status:** Built and deployed — 3-4 units reused across multiple vehicle projects

## Overview
<!-- What it does: DIO + AIO channel counts, CAN interface, what it's used for. -->

## Architecture

![Architecture diagram](assets/architecture-diagram.png)

<!-- Diagram: sensors/actuators → DIO/AIO front end → MCU → CAN transceiver → shared bus →
     host controller. -->

### Design decisions
- **Why CAN:** <!-- multi-drop wiring savings vs point-to-point, bus arbitration, fault tolerance, bus-off recovery if implemented -->
- **I/O specification:** <!-- channel counts, voltage/signal ranges, isolation approach if any -->
- **Reuse across projects:** <!-- which projects, whether hardware stayed identical or needed per-project firmware/config changes -->

## Why this matters for spacecraft avionics

Distributed remote I/O over a shared bus — rather than home-running every sensor/actuator to
a central computer — is the standard modern spacecraft avionics pattern, reducing harness mass
and complexity by placing I/O close to the hardware it serves. This module, built once and
deployed across 3-4 vehicle projects, follows the same "qualify once, reuse many" philosophy
spacecraft component vendors build their product lines around.

## Specs
<!-- Channel counts, voltage ranges, CAN bitrate, message format if custom. -->

## Media
<!-- Photos, wiring diagrams, one project's integration photo. -->
