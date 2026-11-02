---
title: Course Description for EE3601 Transmission Lines, Fields, and Waves
description: A detailed course description for EE3601 Transmission Lines, Fields, and Waves including overview, topics covered and learning objectives in the format of the 2001 Bloom Taxonomy
quality_score: 100
---

# EE3601 — Transmission Lines, Fields, and Waves

**Credits:** 3 (3 lecture hours per week)
**Level:** Undergraduate, junior year
**Prerequisites:** Circuit analysis I and II; vector calculus (multivariable calculus); university physics II (electricity and magnetism)
**Corequisite (recommended):** Differential equations

## Catalog Description

An introduction to electromagnetic fields and waves for electrical engineers, starting with transmission lines and building up to Maxwell's equations and plane waves. Topics include wave propagation on transmission lines, impedance matching and the Smith chart, transients on lines, electrostatics and magnetostatics, Maxwell's equations, uniform plane waves, reflection and transmission at boundaries, and an introduction to waveguides and antennas. Applications cover high-speed digital interconnects, RF and microwave circuits, and wireless and optical systems.

## Course Overview

At high frequencies, or when interconnects are long relative to the signal's wavelength, ordinary circuit theory stops working: voltage and current turn into traveling waves. EE3601 bridges circuit analysis and field theory. It starts with transmission lines, where wave behavior can be studied with familiar circuit quantities, and then develops the field theory underneath it. Students learn to analyze, design and match transmission-line circuits and to predict how electromagnetic waves propagate, reflect and transmit in practical engineering systems.

## Topics

1. **Introduction to waves and phasors.** Traveling waves, wavelength, phase velocity; when circuit theory breaks down; review of phasors and complex numbers.
2. **Transmission-line theory.** Distributed-element model; telegrapher's equations; characteristic impedance; propagation constant; lossless and low-loss lines.
3. **Terminated transmission lines.** Reflection coefficient; standing waves and VSWR; input impedance; short-circuited, open-circuited and quarter-wave lines; power flow.
4. **The Smith chart and impedance matching.** Smith chart construction and use; lumped-element (L-section) matching; single-stub matching; quarter-wave transformers.
5. **Transients on transmission lines.** Step and pulse response; bounce diagrams; reflections in digital interconnects and signal integrity.
6. **Vector analysis review.** Coordinate systems; gradient, divergence and curl; the divergence and Stokes theorems.
7. **Electrostatics.** Coulomb's law; Gauss's law; electric potential; conductors and dielectrics; boundary conditions; capacitance; Laplace's and Poisson's equations.
8. **Magnetostatics.** Biot–Savart law; Ampère's law; magnetic flux and vector potential; magnetic materials; inductance.
9. **Maxwell's equations.** Faraday's law; displacement current; Maxwell's equations in integral and differential (point) form; time-harmonic fields; boundary conditions.
10. **Uniform plane waves.** The wave equation; propagation in lossless and lossy media; skin depth; polarization; the Poynting vector and power density.
11. **Reflection and transmission of plane waves.** Normal and oblique incidence; Snell's law; Fresnel coefficients; total internal reflection; Brewster angle.
12. **Introduction to waveguides and antennas.** Rectangular waveguides, TE and TM modes, and cutoff frequency; radiation from a Hertzian dipole; basic antenna parameters.

## Topics Not Covered

To keep the course focused, the following are left to later electives:

- Antenna arrays, antenna synthesis and detailed antenna design (only the Hertzian dipole and basic antenna parameters are covered)
- Numerical electromagnetics (FDTD, method of moments, finite element method), apart from using a field solver as a tool
- Optical fiber modes and photonics beyond plane-wave reflection and refraction
- Circular and dielectric waveguides, and resonant cavities
- Microwave network theory beyond impedance matching (S-parameter network analysis, couplers, filters, amplifiers)
- Electromagnetic compatibility (EMC) regulation and shielding design
- Relativistic electrodynamics and quantum electrodynamics

## Tools

Students use Python (NumPy and Matplotlib) for computation and plotting, an interactive Smith chart tool, a 2-D field solver, and, where lab equipment is available, a time-domain reflectometer (TDR) and a vector network analyzer (VNA).

## Learning Outcomes

After this course, students will be able to:

### Remember

1. Recall the values and units of the free-space constants ε₀, μ₀, the speed of light c, and the intrinsic impedance of free space η₀ ≈ 377 Ω.
2. State Maxwell's equations in integral and differential form, together with the constitutive relations.
3. Identify the parts of a Smith chart: constant-resistance circles, constant-reactance arcs, and the wavelength scales.
4. Name common transmission-line types (coaxial, two-wire, microstrip, stripline) and their typical characteristic impedances.
5. List the boundary conditions for electric and magnetic fields at an interface between two media.

### Understand

1. Explain why circuit theory fails when an interconnect is long compared with a wavelength or a signal's rise time.
2. Interpret standing-wave patterns in terms of incident and reflected waves.
3. Explain the physical meaning of each of Maxwell's equations, including displacement current.
4. Describe how uniform plane waves propagate in lossless and lossy media, including attenuation, skin depth, polarization and power density.
5. Explain guided-wave propagation in waveguides, including cutoff, and the basic principles of radiation from antennas.

### Apply

1. Calculate the voltage, current, impedance, reflection coefficient, VSWR and power flow on terminated transmission lines.
2. Use the Smith chart to find input impedances and to design lumped-element, single-stub and quarter-wave matching networks.
3. Apply Gauss's, Ampère's and Faraday's laws to find static and time-varying fields and to calculate capacitance and inductance.
4. Calculate the reflection and transmission of plane waves at boundaries between media, for both normal and oblique incidence.
5. Compute the cutoff frequencies of the TE and TM modes of a rectangular waveguide.

### Analyze

1. Analyze transient signals on transmission lines with bounce diagrams and explain how reflections affect signal integrity.
2. Choose a Gaussian surface or Amperian loop by examining a problem's symmetry.
3. Separate the propagation constant of a lossy line or medium into its attenuation and phase contributions, and identify the dominant loss mechanism.
4. Diagnose the location and type of a fault or discontinuity from a time-domain reflectometry (TDR) trace.

### Evaluate

1. Decide when wave effects matter in a circuit and whether an interconnect must be modeled as a transmission line.
2. Compare lumped-element, single-stub and quarter-wave matching for a given frequency and bandwidth, and justify a choice.
3. Evaluate whether a PCB trace needs termination, given its length and the signal's rise time, and select a termination scheme.
4. Judge whether the low-loss or good-conductor approximation is valid for a given line or medium.

### Create

1. Design a matching network for a given load and verify it in simulation or with a vector network analyzer.
2. Design a termination scheme for a high-speed digital bus that meets a specified reflection budget.
3. Build a Python model of a transmission-line circuit that plots standing-wave patterns or bounce-diagram transients.
4. **Capstone project:** design, simulate and measure a microstrip interconnect with a matching network, including a TDR characterization and a short written design justification.

## Assessment (suggested)

| Component | Weight |
|---|---|
| Homework | 20% |
| Quizzes | 10% |
| Computational / lab projects (e.g., Smith chart, TDR measurements, field simulation) | 15% |
| Midterm exams (2) | 30% |
| Final exam | 25% |
