# Power Distribution Unit — Priority Path & Redundant Output ORing

**Status:** Built and deployed in production (Venti Technologies, autonomous vehicle fleet)

## Overview
<!-- 2-3 sentences: what this PDU does, where it's deployed, why it was needed. -->

## Architecture

<!-- Diagram goes here — recommend a clean block diagram: input sources → Priority Power
     Path Controller → redundant voltage regulators → Power ORing → current-sensed
     MOSFET-switched outputs → loads. -->

![Architecture diagram](assets/architecture-diagram.png)

### Design decisions
- **Priority Power Path Controller (input arbitration):** <!-- why PPPC over a simpler switch; what sources are being arbitrated -->
- **Power ORing (output redundancy):** <!-- why ORing across redundant regulators instead of paralleling/diode-OR; what failure it protects against -->
- **Current-sensed MOSFET switched outputs:** <!-- per-channel current limiting and fault isolation — functionally equivalent to a Latching Current Limiter (LCL) -->

## Why this matters for spacecraft power systems

Current-limited, individually switchable, fault-isolatable outputs are the standard pattern
used across spacecraft power distribution — ESA's PDU designs use dedicated Latching Current
Limiter circuits per subsystem with individual current limits and undervoltage protection;
New Horizons' PDU uses fully redundant solid-state switching with hardware fault protection.
This PDU independently converges on the same functional pattern, built and validated in a
terrestrial safety-critical context.

<!-- Be precise here: this is NOT a claim of building spacecraft hardware. It's evidence of
     understanding the same design problem and arriving at industry-standard patterns. -->

## Specs
<!-- Voltage rails, current ratings, channel count, protection thresholds, etc. -->

## Media
<!-- Photos of the built board, oscilloscope captures of the ORing/switching behavior, etc. -->
