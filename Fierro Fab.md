---
layout: default
title: Mechanical Engineer - Fierro Fab
parent: Work Experience
nav_order: 1
---

# Mechanical Engineer
**Fierro Fab**  
**Long Beach, CA** | *Mar 2025 – Present*

---

## Overview

As a Mechanical Engineer at Fierro Fab, I take high-end resto-mod builds — classic cars rebuilt with modern drivetrains, electronics, and hardware — from concept to finished part. My work spans 3D scanning and metrology, fixture and mechanism design, electronics integration, and hands-on fabrication, bridging the engineering side and the shop floor so that what gets designed is what actually gets built. The primary build is a **1965 Lincoln Continental Convertible** targeting around 1,000 horsepower.

## Key Contributions

### Fixture Table

One of the larger projects I have worked on was designing a fixture table for the 1965 Lincoln Continental. The table was designed in Autodesk Fusion using a mix of square tubing and laser-cut steel plates. I orchestrated the orders for all components, designed tooling to keep the table square during assembly, and assisted in its fabrication. Using 3D scans of the chassis, I designed custom mounting fixtures that lock the car body to the table at a precise, known location in global coordinates. A scanner tracking field — a saved network of reference targets in the scanning software — lets us scan individual sections of the car independently and automatically register them to the existing coordinate system, eliminating the need to rescan the whole chassis each work session and keeping file sizes manageable.

{% include image-pair.html left="assets/fierro-fab/chassis-on-fixture-table.webp" alt_left="Chassis scan on the fixture-table CAD" right="assets/fierro-fab/fixture-table.webp" alt_right="Constructed fixture table" %}

After welding, I 3D-scanned the assembled table with the chassis in place and compared it against the CAD to map flatness deviation. Most of the surface came in within 2 mm (1/16 in) across the full 9 × 18 ft span, with the largest error isolated to the bottom-right corner (shown in orange). Leveling is still ongoing — it isn't fully dialed in yet, but it's well within what our current work requires. I also designed dedicated locating fixtures, like the rear chassis fixture below, that bolt to the table's hole grid and constrain the body at known points.

{% include image-pair.html left="assets/fierro-fab/fixture-table-flatness-scan.webp" alt_left="3D-scan flatness deviation map of the fixture table with the chassis mounted" right="assets/fierro-fab/rear-locating-fixture.webp" alt_right="Rear chassis locating fixture bolted to the table grid" %}

### Chassis Straightening Fixtures

The Lincoln's chassis carried warping from prior welding, with several sections out of position by up to half an inch. Correcting it required a dedicated set of clamping fixtures to push the necessary deflection back into specification. I estimated the required correction forces by modeling the chassis as a cantilever beam — a conservative bound on the loads involved — and ran a bolt-slip analysis to confirm the fasteners would stay engaged under the resulting shear. The fixtures were designed for laser cutting, welding, and powder coating; post-weld inspection of the first units confirmed **90° ± 0.1°** perpendicularity, showing that proper fixturing during welding prevented measurable distortion.

{% include image-pair.html left="assets/fierro-fab/chassis-straightening-fixture.webp" alt_left="Welded chassis straightening fixture" right="assets/fierro-fab/chassis-straightening-fixtures-complete.webp" alt_right="Completed and powder-coated straightening fixtures on the table" %}

### Measurement Tower

Accurate bilateral measurement is essential for verifying chassis symmetry throughout the build. A pair of cast magnesium measurement towers mount on either side of the fixture table with a crossbeam spanning between them, enabling repeatable measurements from both sides at once and symmetry checks at any stage. To interface each tower with the table, I designed a custom machined linear-rail slider — an aluminum plate riding on two parallel linear rails — that gives fine positioning beyond the table's fixed 2-inch hole grid. An integrated ruler and pointer read the exact lateral position, a brake locks the slider once set, and each slider is shimmed to its tower for perpendicularity to the table. The tower legs slot directly into the table holes for precise, repeatable location and to prevent tipping in use.

{% include image-pair.html left="assets/fierro-fab/measurement-tower-on-table.webp" alt_left="Measurement tower mounted on the fixture table" right="assets/fierro-fab/measurement-tower-slider.webp" alt_right="Machined linear-rail slider base of the measurement tower" %}

### Custom Door Handle

I redesigned the car's door handle, machining it from billet aluminum and replacing the original mechanical linkage with a digital one: a flush button triggers a microswitch that releases a soft-close latch electronically, rather than physically pulling it. The assembly breaks into four machined components — handle front, handle back, microswitch mount, and button cover — plus custom gaskets for weathersealing, with chrome plating planned for the final parts. To preserve the factory look, I 3D-scanned the door panel's surface and matched the handle's profile to the scan, so the result reads as nearly identical to the original — just with noticeably less slop in the button.

I also extended the handle by 1/4 inch. The door panels have a scooped hand indent that varies from panel to panel; the added length keeps the handle from crossing into that dish, making the fit look intentional across the variance. Relative to an earlier concept, I substantially revised the geometry to cut machining complexity — roughly halving the estimated production cost while keeping the original design intent — and test-fit 3D-printed prototypes of every component on the door to validate fit and clearances.

{% include media-pair.html left="assets/fierro-fab/door-handle-front.webp" alt_left="Machined billet-aluminum custom door handle" right="assets/fierro-fab/door-handle-demo.mp4" alt_right="" %}

### Headlights

The Lincoln's headlights are being fully redesigned — off-the-shelf options were either too modern or carried obtrusive branding, so I'm developing a custom LED module and housing to match the car's era. Each assembly is constrained by a **Kelvin kinematic mount** — a three-point cone, groove, and flat arrangement that fully constrains all six degrees of freedom without overconstraint — and is spring-preloaded against its mount points, with independent adjusters for vertical and horizontal tilt. A 3D-printed mockup validated the packaging and adjustment range. The headlights are planned to integrate into a custom billet grille that replaces the entire front fascia, unifying the lighting and grille into one machined assembly.

{% include image-pair.html left="assets/fierro-fab/headlight-housing-cad.webp" alt_left="Headlight housing CAD" right="assets/fierro-fab/headlight-kinematic-mount.webp" alt_right="Headlight kinematic mount assembly" %}

### Wheels, Tubs, and Suspension Geometry

For a car putting over 1,000 horsepower to the road, the wheels and tires are critical. We're designing our own wheels at significantly larger diameters and widths than stock to grow the contact patch, which in turn requires reworking the rear body panels.

To validate fitment before cutting any metal, I reverse-engineered the existing suspension geometry from 3D scans. The model lets me simulate full suspension travel and catch collisions between moving components and panels at any ride height, and it doubles as a visual reference for customer reviews.

{% include media-pair.html left="assets/fierro-fab/suspension-travel.mp4" alt_left="" right="assets/fierro-fab/wheel-design.webp" alt_right="Render of the updated wheel design" %}

To validate the wheel before committing to machining, I 3D-printed a full-size prototype and mounted it on a **325/35ZR21 Continental SportContact 7**. The design uses a flush whitewall — the white band sits level with the face of the tire, recreating the classic whitewall look while keeping a modern thin-sidewall performance profile. The prototype is currently out for machining.

{% include image-single.html src="assets/fierro-fab/wheel-3dp-prototype.webp" alt="3D-printed wheel prototype with a flush whitewall, mounted on a tire" %}

### Concealed Gas Filler

I am also redesigning the rear taillight to conceal a fuel-filler compartment behind the lens. When released, the taillight pivots outward to expose the fuel cap — a fully integrated solution with no visible external hardware. The motion comes from a cam-slider linkage driven by a gas strut that rotates a linkage arm into the controlled pivot, with a manual override providing access independent of the electronics. The current prototype combines 3D-printed iterative parts, sheet-metal cam geometry, and a temporary CNC-machined taillight arm; the control electronics are mocked up on an Arduino driving the release and status LEDs from a hall-effect sensor and a button. Development is paused pending chassis alignment and final body-panel positioning, which will define the mounting envelope.

{% include image-single.html src="assets/fierro-fab/taillight-cad.webp" alt="CAD model of the redesigned taillight" %}

### Side Mirrors

The Lincoln's side mirrors are being redesigned around the existing mirror internals and motorized adjustment hardware. Matching the original silhouette while packaging modern components calls for extensive compound-surface work.

{% include image-single.html src="assets/fierro-fab/side-mirror-cad.webp" alt="Side mirror CAD model" %}

### Engine Bay Layout

The engine bay is being digitally mocked up by scanning and aligning the engine, transmission, and mounts within the chassis model. This assembly establishes the spatial constraints for everything that follows — custom exhaust headers, supercharger intake routing, and auxiliary structure — and will be finalized once chassis straightening and body positioning are complete.

### Custom Grill (1968 Camaro)

Working from a customer concept and 3D scans of the existing panel cutouts, I designed a full grille to mount on existing brackets set at compound angles. Because the panel stamping is asymmetric, the left and right halves had to be modeled as separate parts. After iterative 3D printing, the final parts were sanded, coated, and installed on the car — the project ran from initial scan to customer delivery in about two weeks.

{% include image-pair.html left="assets/fierro-fab/camaro-grill-cad.webp" alt_left="Custom Camaro grill CAD" right="assets/fierro-fab/camaro-grill-installed.webp" alt_right="Finished custom grill installed on the Camaro" %}

### Reverse Light

A backup (reverse) light that mounts to the rear bumper and illuminates when the car is in reverse. I prototyped the housing and lens fit by 3D-printing the bezel around a clear lens.

{% include image-single.html src="assets/fierro-fab/backup-light-lens-prototype.webp" alt="Prototype backup/reverse light — clear lens in a 3D-printed bezel" %}
