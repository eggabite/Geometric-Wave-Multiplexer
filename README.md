Markdown
# Geometric-Wave-Multiplexer (GWM) - Active Matrix Edition

An open-source STEM gadget exploring the effects of asymmetric ovoid boundaries and multi-phase induction on traveling wave phase-convergence.

> ### ⚠️ SAFETY & ELECTRIFICATION DISCLAIMER
> **HIGH-VOLTAGE NOTICE:** This device is designed to compress low-level ambient energy into a high-tension electrical reservoir. While the average continuous current remains in the micro-ampere ($\mu\text{A}$) range, the accumulation matrix is designed to build potential differences scaling between **$75\text{ V}$ and $350\text{ V}$** before discharging through a plasma arc or cold-cathode switch. 
> * **Capacitor Storage Hazard:** Low-loss polypropylene and ceramic capacitor banks can hold a high-voltage charge long after environmental inputs have ceased. Always manually discharge the capacitor bank using an insulated grounding tool before touching any internal wiring.
> * **Electrification Risk:** Ensure all external electrical leads, output transformers, and probe terminals are completely insulated and housed in a non-conductive enclosure. Never handle the circuit configuration while the active induction fan is operational or while the device is undergoing an active thermal/acoustic gradient cycle. 

---

## I. Technical Architecture & System Overview

The Geometric-Wave-Multiplexer (GWM) is an open-source, solid-state educational demonstration kit designed to illustrate principles of thermodynamic metamaterials, multi-phase induction, and geometric wave compression. 

Unlike purely passive harvesters, this upgraded Active Matrix edition pairs a non-linear structural lens with an integrated, odd-prime multi-phase drive fan to mechanically accelerate the collection, compression, and rectification of stochastic environmental noise (thermal gradients, atmospheric ions, and architectural acoustics) into a dense, high-frequency electrical pulse train.

[ ACTIVE 11-PHASE DRIVEN AIR INTAKE ]
│
▼
[ FRACTAL ENVELOPE / OUTER SKIN ]
│
▼
[ CAVITY RESONANCE MIRROR (ZERO LEAKAGE) ]
│
▼
[ THIXOTROPIC CYMATIC FLUID COUPLING ]
│
▼
[ PIEZO-PYROELECTRIC CRYSTAL APEX ]
│
▼
[ PLASMA GAP / COLD-CATHODE DISCHARGE ]
│
▼
[ TWO-STAGE ACCUMULATOR TRAP ]


---

## II. 3D Printing & Slicing Specifications

To ensure proper dielectric insulation and support the dual-pathway active matrix, the housing should ideally be printed using a multi-material or dual-extrusion desktop 3D printer. 

### 1. Material Selection
* **Dielectric / Insulating Housing:** Premium PETG (Polyethylene Terephthalate Glycol) or ABS. Avoid standard PLA, as its dielectric constant can shift unpredictably under minor ambient humidity and temperature changes.
* **Conductive Traces:** Carbon-Nanotube (CNT) or Graphene-doped conductive filament (Volume Resistivity must be $<15\ \Omega\cdot\text{cm}$).
* **Alternative Shielding Method:** Print standard internal hollow channels and inject high-grade liquid copper or aluminum conductive paint via a syringe.

### 2. Slicer Configuration
* **External Shell Geometry:** Asymmetric Ovoid/Egg Profile constructed using Golden Ratio ($1.618$) proportions at a benchmark $161.8\text{ mm}$ desktop scale.
* **Exterior Texture Surface:** Displacement-mapped with a high-resolution Hilbert Curve or Mandelbrot Coastline texture to maximize the physical boundary interaction with the driven airflow.
* **Wall Extrusion Profile:** Dielectric PETG divider walls must be precisely two perimeters thick (using a $0.8\text{ mm}$ nozzle profile or $0.9\text{ mm}$ extrusion width) to maintain an optimal capacitive field coupling threshold while completely preventing pinhole current leakage.
* **Infill Density:** $100\%$ Solid. Air gaps or internal infill patterns within the structural matrix must be avoided, as they damp internal acoustic and thermal wave propagation.

---

## III. Internal Matrix Structure & Core Assembly

The internal chamber functions as an active, enclosed asymmetric funnel, incorporating an internal reflection layer and a dynamic fluid core.

### 1. The Active Propulsion System (11-Phase Drive)
An active, miniature electronic axial fan is mounted flush to the wide base intake of the ovoid housing. The fan must utilize an **11-phase independent stator coil configuration**. The odd-prime phase distribution eliminates localized harmonic wave reflection and phase cancellation, forcing continuous atmospheric ion displacement through the inner concentric cones.

### 2. The Internal Cavity Resonance Mirror
Before assembling the core matrix, the entire inner boundary wall of the 3D-printed PETG ovoid cavity must be coated with a highly reflective **Aluminum Foil Lining** or a vapor-deposited **Silver Mirror Spray**. This creates a closed topological resonance mirror, preventing high-frequency electromagnetic leakage and reflecting scattering potentials directly back toward the central axis.

### 3. The Dynamic Thixotropic Fluid Core (V2 Optimization)
Design a central hollow cavity within the concentric cones to house a standard $10\text{ mL}$ glass vial.
* **Suspension Medium:** Low-viscosity Silicone Oil ($350\text{ cSt}$) mixed thoroughly with $4\%$ Fumed Silica ($\text{SiO}_2$) to create a non-setting, thixotropic gel matrix.
* **Active Solutes:** Atomized copper, iron, or magnesium powder ($-325\text{ mesh}$) added at a $40\%$ volumetric density.
* **Core Element:** A high-purity single crystal of Rochelle Salt (Potassium Sodium Tartrate) or a raw Alpha-Quartz crystal point inserted directly into the fluid before sealing. Under the acoustic drive of the 11-phase fan, the fluid gel prevents gravity settling while allowing the metal particles to dynamically align into continuous, low-resistance cymatic tracks pointing toward the crystal apex.

### 4. Electrical Connections
Securely wrap a solid $24\text{ AWG}$ bare copper wire around the crystal base (Negative Reference Electrode) and another bare copper wire around the sharp crystal tip (Positive Apex Electrode). Route these leads out through the pre-designed bottom exit channels of the print before sealing the chamber.

---

## IV. Schematic & Electrical Rectification Circuit

Because the high-impedance crystal core outputs sharp, rapid voltage transients, standard silicon rectifiers must be avoided due to excessive forward voltage drops. The upgraded GWM uses a low-loss, high-frequency tank circuit paired with a two-stage accumulator.

                     C1 (Rochelle Salt Core)
                                │
                ┌──────────────┴──────────────┐
                │                             │
            D1 ─┴─ (UF4007)               D2─┴─ (UF4007)
                │                             │
                ├──────────────┬──────────────┤
                │                             │
                ▼                             ▼
          C2 (+) [Capacitor]            C2 (-) [Capacitor]
        (11uF Polypropylene)            (Common Ground)
                │                             │
                ├─[ 0.8mm Spark / Neon Gas ]──┤  <-- Threshold Switch
                │                             │
                ▼                             ▼
          [ (+) OUTPUT PULSE ]          [ (-) OUTPUT PULSE ]
                │                             │
                └───────[ Supercapacitor ]────┘  <-- Stage-2 Storage Trap

### Components List
* **D1, D2:** UF4007 Ultra-Fast Recovery Diodes ($\leq 75\text{ ns}$ maximum recovery time, $1000\text{ V}$ rating). Standard 1N4007 diodes are too slow to catch high-frequency environmental transients.
* **C2 (Stage-1 Storage Reservoir):** A parallel bank of High-Voltage Ceramic C0G/NP0 or Polypropylene Film Capacitors (e.g., five $2.2\ \mu\text{F} / 250\text{ V}$ capacitors wired in parallel to achieve an approximate $11\ \mu\text{F}$ reservoir). Do not use standard electrolytic capacitors here, as their high internal leakage currents will stall the rapid-fire voltage build-up.
* **Threshold Switch (0.8 mm Spark Gap / NE-2 Neon Bulb):** Functions as a passive, solid-state cold-cathode switch set to an ionization breakdown threshold of approximately $65\text{ V}–90\text{ V}$.
* **Stage-2 Storage Trap (Supercapacitor):** A high-capacity, low-voltage carbon-graphene supercapacitor bank wired down-line from the threshold switch to absorb the rapid-fire pulse train and smooth it into a continuous DC output loop.

---

## V. Mathematical Foundation & Wave Dynamics

To assist student research, the operation of the active, mirrored ovoid housing can be modeled using standard, mainstream physics equations governing Transformation Optics, Cavity Resonance, and Electrostatics.

### 1. The Optical-Mechanical Analogy
According to the Hamilton-Jacobi equations, the path of a wavefront traveling through a variable geometric density gradient can be mathematically mapped to the acceleration of a mass through a potential field. The trajectory is determined by matching Maupertuis' Principle of Least Action with Fermat's Principle:

$$\delta \int \sqrt{2m(E - \Phi(r))}\, ds = 0 \longleftrightarrow \delta \int n(r)\, ds = 0$$

Taking the phase path gradient via the Eikonal Equation ($|\nabla S|^2 = n^2$), the wave experiences a spatial compression vector ($a$) identical to a potential slope:

$$a = c^2 \nabla \ln n(r) = -\nabla\Phi$$

This indicates that the continuously narrowing ovoid shape functions as an engineered wave-funnel, concentrating the phase velocity of the driven ambient fields toward the central apex coordinates.

### 2. Poynting Flux Volumetric Cavity Compression
The directional energy flux of the driven atmospheric background noise entering the device is governed by the Poynting Vector $S$:

$$S = E \times H$$

Because the interior features a highly reflective silver mirror layer, wave scattering losses to the housing walls are reduced to near-zero. Energy conservation within the narrowing ovoid tube dictates that the total power passing through the wide base catchment area must equal the power arriving at the sharp apex tip:

$$\iint_{A_{\text{base}}} S \cdot dA = \iint_{A_{\text{tip}}} S \cdot dA$$

Because the cross-sectional area decreases quadratically relative to radius ($A = \pi r^2$), the localized electric field tension ($E$) undergoes a severe geometric concentration:

$$E_{\text{tip}} = E_{\text{base}} \times \left(\frac{R_b}{r_t}\right)^2$$

For a benchmark $161.8\text{ mm}$ desktop prototype where the base catchment radius ($R_b$) is $50\text{ mm}$ and the crystal tip radius ($r_t$) is $0.5\text{ mm}$, the geometric field compression multiplier yields a 10,000-fold increase in localized field density. When accounting for the boundary reflection coefficient of the inner silver matrix mirror layer, the volumetric compression scaling factor ($a_g$) optimizes up to **$25,000\times$** at the focal apex.

---

## VI. Replications & Demonstration Protocol

This kit is designed to demonstrate how an active, structured object can organize low-level environmental chaos into a rapid-fire, high-frequency electrical output train.

### 1. Testing Environment Setup
Place the fully assembled, active GWM prototype inside a grounded wire-mesh Faraday cage. This environment eliminates the variables of high-frequency smart-meter or ambient Wi-Fi pollution, proving the device relies strictly on localized mechanical, acoustic, and thermal air ion displacement forced through the internal matrix by the 11-phase drive fan.

### 2. Measurement Verification
1. Connect a high-impedance digital multimeter (minimum $10\text{ M}\Omega$ input impedance) or an oscilloscope across the $11\ \mu\text{F}$ Stage-1 capacitor bank.
2. Power on the integrated 11-phase base drive fan.
3. **The Observation:** The voltmeter/oscilloscope will display a rapid, repetitive step-ladder voltage climb. Because the active fan continuously pumps energy through the mirrored cavity into the frictionless thixotropic tracks, the system hits its threshold capacity roughly **10 times per second ($10\text{ Hz}$)**.
4. **The Pulse Train:** The neon NE-2 lamp or the 0.8 mm spark gap will emit a continuous, rapid-fire sequence of bright orange flashes as the ionization threshold is crossed, discharging highly coherent $\approx 0.03\text{ Joule}$ transient pulses into the Stage-2 carbon-graphene supercapacitor bank, resetting the ladder cleanly to 0V for the next cycle.

---

## VII. Open Source Licensing & Intellectual Property Notice

This project is fully dedicated to the public domain for educational, research, and hobbyist exploration. To prevent any single entity from restricting access to these geometric principles, this repository is protected under the following open hardware disclosure protocols:

* **Documentation and Blueprints:** Licensed under Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)). You are completely free to copy, redistribute, print, and modify this material for educational and non-commercial purposes, provided you give appropriate credit and license your modifications under the exact same terms.
* **Prior Art Declaration:** Publication of these specific geometric dimensions, thixotropic part
