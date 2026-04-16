---
layout: default
title: Undergraduate Researcher - AMML
parent: Work Experience
nav_order: 2
---

# Undergraduate Researcher  
**Additive Manufacturing and Metamaterials Lab (AMML)**  
**UC Berkeley** | *May 2023 – December 2024*

---

## Overview  

As an undergraduate researcher at the AMML, I contributed to two primary research areas: **multimaterial Digital Light Processing (DLP) 3D printing** and **piezoelectric actuator development**. The work spanned hardware design, embedded systems, wet lab fabrication, and computational analysis, and resulted in a co-authorship on a peer-reviewed journal article.

---

## Multimaterial DLP Printing

### Printer Design

DLP 3D printing cures photopolymer resin layer by layer using projected UV light. Producing true multimaterial parts requires swapping resins mid-print without cross-contaminating adjacent vats — a constraint that necessitated a purpose-built hardware platform.

I designed and fabricated a DLP printer centered on a motorized rotary stage that indexes between multiple resin vats. The stage automates vat positioning, material swapping, and inter-vat cleaning sequences without interrupting the print cycle. Machine control was implemented in **Arduino** and **LabVIEW**.

{% include image-pair.html left="assets/rotary_printer.jpg" alt_left="SolidWorks Model of the Rotary Printer" right="assets/rotary_cross_section.jpg" alt_right="Cross Section of Rotary Stage" %}

The system produced successful multimaterial prints with minimized resin cross-contamination between material swaps.

{% include image-pair.html left="assets/multicolor_lattice.jpg" alt_left="Dual-Color Lattice Print" right="assets/multicolor_lattice_2.jpg" alt_right="Multimaterial Print on a Single Layer" %}

### In-Situ Electroless Plating

A concurrent project explored integrating automated electroless metal plating directly into the print cycle, enabling conductive features to be deposited onto printed geometry without removing the part from the printer. I contributed to the hardware integration of this process into the rotary printer platform prior to graduation.

{% include image-single.html src="assets/electroless_plated_microlattice.jpg" alt="Electroless Plated Microlattice" %}

---

## P$\mu$SL Microlattice Printing

[Projection micro-stereolithography](https://pubs.aip.org/aip/rsi/article-abstract/83/12/125001/357459/Design-and-optimization-of-a-light-emitting-diode?redirectedFrom=fulltext) (P$\mu$SL) is a high-resolution DLP process capable of printing microlattice structures at 1.3 $\mu$m/pixel feature size. A persistent challenge in this process is oxygen inhibition of photopolymerization — dissolved oxygen near the resin surface suppresses curing and creates spatial variation in print quality.

I was tasked with characterizing the oxygen concentration distribution across the print area and redesigning the resin vat to reduce the spatial gradient. Improved nitrogen flow geometry in the redesigned vat reduced the variation in oxygen concentration by a factor of 2, establishing more repeatable printing conditions across the build area.

{% include image-pair.html left="assets/vat_pdms.jpg" alt_left="Redesigned PDMS Vat" right="assets/oxygen_vats.jpg" alt_right="Vat Comparison" %}

An oxygen sensor was integrated into the LabVIEW control interface for continuous in-situ monitoring throughout the print cycle. To address slicing inconsistencies that produced strut thickness variation in printed lattices, a **MATLAB** script was developed to detect and correct outlier slice geometries, achieving a target strut thickness of approximately 35 $\mu$m.

{% include image-single.html src="assets/mesh_fix.jpg" alt="MATLAB Slice Correction for Consistent Strut Thickness" %}

This work contributed to a paper published in the *Additive Manufacturing Journal*, accessible [here](https://www.sciencedirect.com/science/article/abs/pii/S2214860425000818).

---

## Piezoelectric Actuator Development

Piezoelectric bimorphs convert electrical signals directly into mechanical displacement, making them well-suited for high-precision, small-scale actuation. I designed and fabricated a 2-axis bimorph structure achieving 100 $\mu$m of displacement within a 3×3×1 cm package.

To increase usable stroke, a mechanical amplification stage was designed and simulated in **SolidWorks**. The compliant mechanism multiplies output displacement at the cost of force — a standard trade-off in precision actuator design — and was validated through simulation before fabrication.

{% include video-single.html src="assets/amplifier.mp4" %}

Printed piezoelectric composites were also fabricated in multiple lattice configurations, exploring geometric strategies for increasing actuator density in array-based systems.

---

## Skills & Tools  
- **Software:** MATLAB, LabVIEW, SolidWorks, Arduino, Python  
- **Lab Equipment:** Tensile testing machines, centrifuges, resin 3D printers, precision ovens, optical measurement tools  
- **Materials Handling:** Wet and dry lab experience; handling of photopolymers, metal precursor solutions, and piezoelectric composites with appropriate PPE and fume hood protocols
