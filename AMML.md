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
As an undergraduate researcher, I focused on advancing **multimaterial Digital Light Processing (DLP) 3D printing** and the development of **piezoelectric actuators**. My work involved designing 3D printers and their software, manufacturing small scale piezoelectric actuators, and optimizing printing parameters of novel printing techniques.

---

## Key Contributions  

### Multimaterial DLP Printing
I designed and fabricated a DLP printer that incorporated a new cleaning method between resin swaps. I also configured the software for material swapping and cleaning through **Arduino** and **LabVIEW**. Produced successful multimaterial prints with minimized resin cross-contamination.

**Example Prints:**
{% include image-pair.html left="assets/multicolor_lattice.jpg" alt_left="Dual Color Lattice" right="assets/multicolor_lattice_2.jpg" alt_right="Dual Color on same Layer" %}

**In-situ Electroless Plating:** Contributed to a project incorporating automated electroless plating techniques, though it was not completed before my graduation. The printer I designed incorporated a 3D printed rotary stage for cycling between vats.

**SolidWorks Model of the Rotary 3D Printer**
{% include image-single.html src="assets/rotary_printer.jpg" alt="Render of Rotary Printer" %}

---

### P$\mu$SL Lattices
I enhanced the performance of our [Projection micro-stereolithography](https://pubs.aip.org/aip/rsi/article-abstract/83/12/125001/357459/Design-and-optimization-of-a-light-emitting-diode?redirectedFrom=fulltext) (P$/mu$SL) 3D printer, which prints microlattices with a resolution of 1.3 $\mu$m/pixel. Oxygen inhibition of photopolymerization was a substantial issue in printing performance. I was tasked with mapping the oxygen levels across the print area, and optimizing to reduce the $O_2$ gradient across it. The new vat design decreased the variation of oxygen concentration by 2x by improving the flow of $N_2$, allowing for repeatable printing conditions. An oxygen sensor was also implemented in LabVIEW for in-situ monitoring.

{% include image-single.html src="assets/oxygen_vats.jpg" alt="Image showing the new vats" %}

I developed a **MATLAB** script to detect and adjust slicing outliers, ensuring consistent strut thickness of ~35$\mu$m in printed microlattices.

{% include image-single.html src="assets/mesh_fix.jpg" alt="Image showing the change of slices to optimize strut thickness" %}

I was later added as an author on a published paper in the Additive Manufacturing Journal. The paper can be accessed [here](https://www.sciencedirect.com/science/article/abs/pii/S2214860425000818).

---

### Piezoelectric Actuator
I also designed piezoelectric bimorphs for actuating. The final model was a 2-axis bimorph structure that resulted in 100 microns of displacement in a 3x3x1cm package. To increase the amplitude, another stage of amplification was designed and simulated in **Solidworks**, as shown below. I fabricated printed piezoelectric composites in several lattice configurations made for high density actuator systems.

{% include video-single.html src="assets/amplifier.mp4" %}

---

## Skills & Tools  
- **Software Proficiency:** MATLAB, LabVIEW, SolidWorks, Arduino, Python.  
- **Lab Equipment:** Tensile testing machines, centrifuges, 3D printers, ovens, and precision measurement tools.  
- **Materials Expertise:** Worked in both a dry and wet lab. Properly handled chemicals and delicate parts. Used proper PPE and fume hoods. Worked around hazardous materials.
