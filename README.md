# ABB IRB 120 Automated Drilling Simulation — RobotStudio

An industrial robot drilling simulation built in ABB RobotStudio, programming an IRB 120 robot arm to perform automated hole drilling across a workpiece with defined waypoints, tool paths, and drilling sequences.

## Overview

This project simulates an automated drilling operation using an **ABB IRB 120** industrial robot in **RobotStudio**. The robot follows a programmed path of waypoints across a workpiece mounted on a worktable, performing precision drilling at each target location.

The simulation covers the full workflow: station setup, tool definition, workobject calibration, waypoint teaching, path programming, and cycle execution.

## System Setup

```
    ┌─────────────────────────────────┐
    │         Worktable               │
    │  ┌───────────────────────────┐  │
    │  │      Workpiece            │  │
    │  │   ×  ×  ×  ×  ×  ×  ×    │  │  × = Drill points
    │  │   ×  ×  ×  ×  ×  ×  ×    │  │    (programmed waypoints)
    │  └───────────────────────────┘  │
    └─────────────┬───────────────────┘
                  │
         ┌────────▼────────┐
         │   ABB IRB 120   │
         │   + Drill Tool  │
         │   (6-axis arm)  │
         └─────────────────┘
```

## Robot Specifications

| Parameter | Value |
|-----------|-------|
| Robot Model | ABB IRB 120 |
| Axes | 6 |
| Payload | 3 kg |
| Reach | 580 mm |
| Repeatability | ±0.01 mm |
| Software | ABB RobotStudio |
| Programming Language | RAPID |

## What I Did

- **Station design** — set up the complete robot cell including worktable, workpiece, and tool
- **Tool definition** — created and calibrated the drill tool with correct TCP (Tool Centre Point)
- **Workobject calibration** — defined the workpiece coordinate frame for accurate positioning
- **Waypoint teaching** — programmed drill locations across the workpiece surface
- **Path programming** — created RAPID motion paths with MoveL and MoveJ instructions for approach, drill, retract, and traverse sequences
- **Simulation and validation** — ran the full drilling cycle, checked for collisions, singularities, and reachability

## Simulation Demo

Watch the drilling simulation video in media

## Context

Developed as a solo project at RMIT University as part of the Robotics and Mechatronics Engineering program.

## Skills Demonstrated

- Industrial robot programming (ABB RobotStudio, RAPID)
- Robot cell design and layout
- Tool and workobject calibration
- Path planning and waypoint programming
- Collision detection and simulation validation
- Understanding of 6-axis robot kinematics

