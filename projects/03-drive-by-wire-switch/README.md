# Drive-by-Wire Auto/Manual Control Authority Switch

**Status:** Built and deployed in production — core safety system across multiple autonomous vehicle programs

## Overview
<!-- What it does, why it's described as "the heart" of the vehicle — what fails without it. -->

## Architecture

![Architecture diagram](assets/architecture-diagram.png)

### Design decisions
- **Switching mechanism:** <!-- hard relay/contactor cutout vs. arbitration logic — which one, and why -->
- **Transition handling:** <!-- how bumpless transfer / fail-safe defaults are handled during handover -->
- **Trigger conditions:** <!-- operator-commanded only, or fault-triggered automatic handback -->

## Why this matters for crewed spacecraft systems

Crewed spacecraft — Orion, Dragon, Starliner — all require the same core capability: switching
control authority between autonomous/computer control and manual crew control, with a hard
guarantee the switch is safe and unambiguous. This is the same control-authority arbitration
problem, solved for a production automotive safety-critical system.

## Specs
<!-- Response time, fail-safe behavior, interfaces to the rest of the vehicle stack. -->

## Media
<!-- Circuit photos, timing diagrams/scope captures of a transition event if available. -->
