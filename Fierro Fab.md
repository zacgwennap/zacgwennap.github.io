---
layout: default
title: Lead Mechanical Engineer - Fierro Fab
parent: Work Experience
nav_order: 1
---

# Lead Mechanical Engineer
**Fierro Fab**  
**Long Beach, CA** | *Mar 2025 – Present*

---

## Overview

Fierro Fab specializes in resto-mod builds — classic cars restored and upgraded with modern engineering. As Lead Mechanical Engineer, I manage projects from initial concept through fabrication and delivery, spanning mechanical design, structural analysis, electronics, and vendor coordination. The primary build is a **1965 Lincoln Continental Convertible** targeting over 1,000 horsepower.

---

## Fixture Table and Chassis Setup

Accurate chassis positioning is foundational to all downstream work on the Lincoln. I designed a fixture table in **Autodesk Fusion** using a combination of square tubing and laser-cut steel plates, then coordinated all component procurement, designed squaring tooling to ensure the table remained true during assembly, and assisted with fabrication.

{% include image-pair.html left="assets/chassis_on_table.PNG" alt_left="Chassis Scan Aligned to Fixture Table CAD" right="assets/fixture_table.jpg" alt_right="Completed Fixture Table" %}

Custom mounting fixtures were developed from 3D scans of the chassis, locking the body to the table at a known location in global coordinates. A scanner tracking field — a saved network of reference targets in the scanning software — allows individual sections of the car to be scanned independently and automatically registered to the existing coordinate system. This eliminates the need to rescan the entire chassis for each work session, significantly improving workflow efficiency.

---

## Chassis Straightening Fixtures

The Lincoln's chassis sustained warping from prior welding, leaving several sections out of position by significant margins. Correcting this required a dedicated set of clamping fixtures to induce the necessary deflection back into specification.

The required correction forces were estimated by modeling the chassis as a cantilever beam, providing a conservative bound on the loads involved. A subsequent bolt slip analysis confirmed that the fasteners would remain engaged under the shear forces generated during straightening.

{% include image-single.html src="assets/welded_chassis_fixture.jpg" alt="Welded Chassis Straightening Fixture" %}

The fixtures were designed for laser cutting, welding, and powder coating. Post-weld inspection of the first fixtures confirmed perpendicularity of **90° ± 0.1°**, demonstrating that proper fixturing during welding prevented measurable distortion. The completed fixtures are currently awaiting final machining operations before installation on the table.

---

## Custom Door Handles

The Lincoln's original cast door handles are being replaced with a fully custom design that preserves the original aesthetic while incorporating a modern latching mechanism. A flush button triggers a microswitch to release the door electronically, with internal components designed around the precise contour of the door panel.

The assembly consists of four machined components — handle front, handle back, microswitch mount, and button cover — along with custom elastomeric gaskets for weathersealing. All parts are intended for final production in CNC-machined aluminum.

{% include image-pair.html left="assets/handle_back.PNG" alt_left="Handle Back Component" right="assets/3d_printed_handle.jpg" alt_right="Handle Assembly" %}

3D printed prototypes of all components were completed and test-fit on the door to validate fit and clearances. Relative to a prior design concept, the geometry was substantially revised to reduce machining complexity, cutting estimated production cost in half while maintaining the original design intent.

{% include image-pair.html left="assets/handle_full_front.PNG" alt_left="3D Printed Handle Prototype" right="assets/handle_front.png" alt_right="Handle Prototype Fitted on Door" %}

---

## Wheels, Tubs, and Suspension Geometry

Transmitting over 1,000 horsepower to the road demands a substantial increase in contact patch area. Custom wheels are being designed at significantly larger diameters and widths than stock, requiring corresponding modifications to the rear body panels.

To validate fitment before any metal is cut, the existing suspension geometry was reverse-engineered from 3D scans. The resulting model allows full simulation of suspension travel, enabling collision detection between moving components and body panels at all ride heights. The same model serves as a visual reference for customer reviews.

{% include image-pair.html left="assets/suspension_demo.gif" alt_left="Suspension Travel Simulation" right="assets/wheel_old.PNG" alt_right="Updated Wheel Design Render" %}

---

## Concealed Gas Filler

The rear taillight is being redesigned to conceal a fuel-filler compartment behind the lens. When released, the taillight pivots outward to expose the fuel cap — a fully integrated solution with no visible external hardware.

{% include image-single.html src="assets/taillight.jpg" alt="Taillight CAD Model" %}

The actuation system uses a **cam-slider linkage** driven by a gas strut, which rotates a linkage arm to produce the controlled pivot. A button triggers the primary release; a manual override provides secondary access independent of the electronic system. The current prototype combines 3D printed iterative components, sheet metal cam geometry, and a temporary CNC-machined taillight arm. Development is paused pending chassis alignment and body panel positioning, which will define the final mounting envelope.

---

## Side Mirrors

The Lincoln's side mirrors are being redesigned around the existing mirror internals and motorized adjustment hardware. Matching the original silhouette while accommodating modern components requires extensive compound surface work.

{% include image-single.html src="assets/side_mirror.jpg" alt="Side Mirror CAD Model" %}

---

## Engine Bay Layout

The engine bay is being digitally mocked up by scanning and aligning the engine, transmission, and engine mounts within the chassis model. This assembly establishes the spatial constraints for all subsequent component designs — custom exhaust headers, supercharger intake routing, and ancillary structure — and will be finalized once the chassis straightening and body positioning are complete.

---

## Additional Projects

### Custom Grille for a 1968 Camaro

Working from a customer concept and 3D scans of the existing panel cutouts, I developed a full grille design to be mounted on existing brackets positioned at compound angles. Asymmetric panel stamping required the left and right halves to be modeled as separate files. After iterative 3D printing, the final parts were sanded, coated, and installed on the vehicle. The project ran from initial scan to customer delivery in approximately two weeks.

{% include image-pair.html left="assets/grill_small.PNG" alt_left="Grille CAD Model" right="assets/grill_on_car.jpg" alt_right="Installed on Vehicle" %}
