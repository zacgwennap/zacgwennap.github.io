---
layout: default
title: Thrust Vector Controlled Rocket
parent: Projects
nav_order: 2
---

# Thrust Vector Controlled (TVC) Model Rocket
*May 2020 – Aug 2021*

Thrust vector control (TVC) steers a rocket by redirecting the thrust vector of its motor rather than relying on aerodynamic surfaces. The technique is used extensively in modern launch vehicles, most visibly by SpaceX.

This project was undertaken while I was still in community college, without formal training in fluid dynamics, control theory, embedded programming, or PCB design. Despite that, the attempt to integrate all of these disciplines simultaneously accelerated my development significantly and established the technical foundation I carried into my engineering degree.

---

## Mechanical Design

The TVC mount was designed to fit within a 74mm airframe and provides two degrees of freedom with ±5° of actuation, driven by high-torque servos. Designing for the confined envelope required several iterations to achieve a layout that was both functional and manufacturable within the airframe constraints.

{% include image-single.html src="assets/tvc.jpg" alt="TVC Mount Assembly" %}

A parachute ejection system was developed in parallel. A spring provides the ejection impulse, triggered by a servo that releases upon detecting descent via the onboard pressure sensor.

{% include image-single.html src="assets/piston_mechanism.jpg" alt="Spring-Loaded Parachute Ejection Mechanism" %}

---

## Electronics

A custom PCB was designed around a Teensy microcontroller to handle onboard sensing and control. The board incorporated a voltage regulator, MOSFETs for motor ignition, a BMP280 barometric pressure sensor for altitude and ejection triggering, and a BNO-055 IMU for acceleration and orientation data. Outputs were provided for three servos, status LEDs, and an SD card for flight data logging.

{% include image-single.html src="assets/flight_board.jpg" alt="Custom Flight Computer PCB" %}

All sensors were successfully interfaced, servos and MOSFETs were tested under load, and data logging to the SD card was validated — establishing a complete data acquisition and actuation chain.

---

## Simulation

A 2D flight simulation was developed in **Python** to model the rocket's trajectory. Using the Estes F15 motor thrust curve and a specified launch angle, the simulation computed position, velocity, and acceleration over the flight profile. Full details and source code are available in the [GitHub repository](https://github.com/ZacCac/Model-Rocket-Flight-Simulation/tree/main).

{% include image-single.html src="assets/rocket_sim.jpg" alt="Simulation Output Plots" %}

---

## What I Learned

The TVC mount functioned mechanically but exhibited significant backlash, which would have compromised any closed-loop control algorithm. Correcting this would require either tighter hardware tolerances or a controller robust enough to compensate for the slop. The project ultimately stalled at the software stage — the control algorithm was never completed.

The more lasting outcome was the confidence to engage with unfamiliar, technically demanding problems. The combination of mechanical design, PCB layout, embedded programming, and simulation was ambitious given my background at the time, and navigating it set the tone for how I approach complex projects today.

---

## Skills Applied

- CAD: originally **Fusion 360**, redesigned in **SolidWorks**
- PCB schematic design in **Autodesk Eagle**; firmware in **C / Arduino**
- Flight simulation in **Python**
- Fabrication: **FDM 3D printing** and **soldering**
