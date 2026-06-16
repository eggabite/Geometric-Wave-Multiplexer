# Geometric-Wave-Multiplexer
An open-source STEM gadget exploring the effects of asymmetric ovoid boundaries on sequential traveling wave phase-convergence

## I. Project Overview & Educational Objective

The Geometric-Wave-Multiplexer (GWM) is an open-source, solid-state educational demonstration kit designed to illustrate principles of thermodynamic metamaterials, acoustic-to-electrical coupling, and geometric wave compression. 

The purpose of this project is to build a highly sensitive, completely passive structural lens capable of harvesting stochastic ambient environmental noise (such as thermal drift, architectural vibrations, and low-frequency stray AC hum) and organizing it into a measurable, low-frequency electrical pulse train. 

This kit serves as a practical, hands-on tool for physics students, makers, and electronics hobbyists to explore how asymmetric boundary conditions and structured matter can alter the behavior of ambient field lines without the use of active microcontrollers or external battery inputs.

---

## II. 3D Printing & Material Specifications

To ensure proper insulation between the internal fields and maximize capacitive coupling, the housing should ideally be printed using a dual-extrusion desktop 3D printer. However, a single-extrusion printer can be used by utilizing the fluid-core layout option described in Section III.

### 1. Material Selection
* Dielectric / Insulating Housing: Premium PETG (Polyethylene Terephthalate Glycol) or ABS. Avoid standard PLA, as its dielectric constant can shift under minor ambient humidity and temperature changes.
* Conductive Traces: Carbon-Nanotube (CNT) or Graphene-doped conductive filament (Volume Resistivity should be less than 15 Ohm-cm). 
* Alternative Shielding Method: Print standard internal hollow channels and inject high-grade liquid copper shielding paint using a syringe.

### 2. Slicer Configuration
* External Shell Geometry: Asymmetric Ovoid/Egg Profile constructed using Golden Ratio (1.618) proportions.
* Exterior Texture Surface: Displacement-mapped with a high-resolution Hilbert Curve or Mandelbrot Coastline texture. This structural modification dramatically increases the surface-area-to-volume ratio, maximizing the physical boundary interaction with ambient thermal and acoustic waves.
* Wall Extrusion Profile: Dielectric PETG divider walls must be precisely two perimeters thick (using a 0.8mm nozzle profile or 0.9mm extrusion width) to maintain an optimal capacitive field coupling threshold while completely preventing pinhole current leakage.
* Infill Density: 100% Solid. Air gaps or internal infill patterns within the structural matrix must be avoided, as they damp internal acoustic and thermal wave propagation.

---

## III. Internal Matrix Structure & Core Assembly

The internal chamber functions as an asymmetric dielectric funnel, featuring nested, alternating conductive and insulating concentric pathways pointing down toward a central focal chamber.

### 1. Core Selection (The Crystal Apex)
The mechanical and electrostatic tension of the compressed environment is focused directly onto a high-purity single-crystal core.
* Option A: A high-grade, single-crystal cluster of Rochelle Salt (Potassium Sodium Tartrate). Rochelle Salt is highly recommended for educational displays due to its exceptionally high sensitivity to minor thermal fluctuations and acoustic vibrations.
* Option B: A raw Alpha-Quartz crystal point.

### 2. The Fluid Core Matrix Upgrade (V2 Optimization)
To optimize particle alignment and minimize internal field scattering, design a central hollow cavity to house a standard 10mL glass vial. 
* Fill the vial with low-viscosity Silicone Oil (350 cSt) mixed thoroughly with 4% Fumed Silica to create a thixotropic gel matrix.
* Add atomized copper or iron powder (-325 mesh) to the suspension. 
* Insert the Rochelle Salt or Quartz crystal core directly into this particulate fluid mixture before sealing the vial into the primary PETG housing. The thixotropic gel ensures the particles can dynamically respond to ambient 60 Hz hum, aligning into low-resistance paths toward the crystal apex without permanently settling due to gravity.

### 3. Electrical Connections
Wrap a bare 24 AWG solid copper wire securely around the base of the crystal (Negative Reference Electrode) and another bare copper wire around the sharp crystal tip (Positive Apex Electrode). Route these leads out through the pre-designed bottom exit channels of the 3D print before completing the assembly.

---

## IV. Schematic & Electrical Rectification Circuit

Because the high-impedance crystal core outputs sharp, micro-scale voltage transients, standard silicon rectifiers must be avoided due to excessive forward voltage drops. The GWM uses a passive, low-loss tank circuit designed to trap and store the gathered charge.

### Components List
* D1, D2: UF4007 Ultra-Fast Recovery Diodes (75ns maximum recovery time, 1000V rating). Standard 1N4007 diodes are too slow to catch high-frequency environmental transients and will leak the energy.
* C2 (Storage Reservoir): A parallel bank of High-Voltage Ceramic C0G/NP0 or Polypropylene Film Capacitors (for example, five 2.2uF / 250V capacitors wired in parallel to achieve an approximate 11uF reservoir). Do not use standard electrolytic capacitors, as their high internal leakage currents will stall the voltage build-up.
* Threshold Switch (Neon NE-2 Bulb): Functions as a passive, solid-state cold-cathode switch. The bulb maintains near-infinite resistance until the storage reservoir reaches its native ionization breakdown voltage (approximately 65V to 90V), at which point it flashes and discharges the stored energy cleanly into the output.

### Circuit Topology
Connect the positive and negative leads from the crystal core directly to the inputs of the UF4007 diode bridge. Connect the DC output of the bridge across the low-leakage C2 capacitor bank. Wire the NE-2 Neon Bulb directly in parallel across the capacitor bank, leading out to a small step-down pulse transformer or your measurement multimeter.

---

## V. Mathematical Foundation & Wave Dynamics

To assist student research, the operation of the asymmetric ovoid housing can be modeled using standard, mainstream physics equations governing Transformation Optics, Wave Mechanics, and Electrostatics.

### 1. The Optical-Mechanical Analogy
According to the Hamilton-Jacobi equations, the path of a wavefront traveling through a variable geometric density gradient can be mathematically mapped to the acceleration of a mass through a potential field. The trajectory is determined by matching Maupertuis' Principle of Least Action with Fermat's Principle:

δ ∫ √[2m(E − Φ(r))] ds = 0  ←→  δ ∫ n(r) ds = 0

Taking the phase path gradient via the Eikonal Equation (|∇S|² = n²), the wave experiences a spatial compression vector (a) identical to a potential slope:

a = c² ∇ ln n(r) = −∇Φ

This indicates that the continuously narrowing ovoid shape functions as an engineered wave-funnel, concentrating the phase velocity of chaotic ambient fields toward the central apex coordinates.

### 2. Poynting Flux Volumetric Compression
The directional energy flux of the captured ambient background noise entering the device is governed by the Poynting Vector S:

S = E × H

Assuming the thixotropic fluid matrix minimizes scattering losses, energy conservation within the narrowing ovoid tube dictates that the total power passing through the wide base must equal the power arriving at the sharp apex tip:

∫∫Abase S · dA = ∫∫Atip S · dA

Because cross-sectional area decreases quadratically relative to radius (A = πr²), the localized electric field tension (E) undergoes a geometric concentration:

Etip = Ebase × (Rb/rt)²

For a benchmark 161.8 mm desktop prototype where the base catchment radius (Rb) is 50 mm and the crystal tip radius (rt) is 0.5 mm, the geometric field compression multiplier yields a 10,000-fold increase in localized field density before entering the rectification circuit.

---

## VI. Replications & Demonstration Protocol

This kit is designed to demonstrate that a purely passive, structured object can organize low-level environmental chaos into a visible, rhythmic output without any chemical batteries.

### 1. Testing Environment Setup
Place the fully assembled GWM prototype inside a completely dark, quiet room or inside a grounded wire-mesh Faraday cage. This environment eliminates the variables of visible ambient light and high-frequency smart-meter or Wi-Fi pollution, proving the device relies purely on localized mechanical/thermal room energy.

### 2. Measurement Verification
Connect a high-impedance digital multimeter (minimum 10 MOhm input impedance) across the C2 capacitor bank. 
* The Observation: The voltmeter will show a steady, step-ladder climb in voltage.
* The "Heartbeat" Flash: As the capacitor bank accumulates the compressed ambient charge, it will reach the breakdown voltage of the neon lamp (~75V). The NE-2 bulb will emit a sharp, visible orange flash, discharging the capacitor instantly, resetting the voltmeter to 0V, and immediately beginning the step-ladder climb again.

---

## VII. Open Source Licensing & Intellectual Property Notice

This project is fully dedicated to the public domain for educational, research, and hobbyist exploration. To prevent any single entity from restricting access to these geometric principles, this repository is protected under the following open hardware disclosure protocols:

* Documentation and Blueprints: Licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0). You are completely free to copy, redistribute, print, and modify this material for educational and non-commercial purposes, provided you give appropriate credit and license your modifications under the exact same terms.
* Prior Art Declaration: Publication of these specific geometric dimensions, thixotropic particulate fluid core configurations, and passive neon breakdown circuit typologies constitutes a public, timestamped disclosure. This documentation serves as active prior art in the public domain to prevent the filing of future restrictive or proprietary patent claims on this specific macro-scale desktop architectural arrangement.
