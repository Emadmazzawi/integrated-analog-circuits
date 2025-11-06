# Analog Circuit Design Projects

A collection of CMOS analog circuit designs implemented and simulated using Cadence Virtuoso. These projects demonstrate various amplifier topologies and design techniques for modern applications.

## 🎯 Projects Overview

This repository contains four comprehensive analog circuit design exercises, each focusing on different amplifier architectures and specifications:

| Project | Type | Key Specs | Application |
|---------|------|-----------|-------------|
| Exercise 1 | Baseband Amplifier | 20dB gain, 20MHz BW | Wi-Fi 6 Systems |
| Exercise 2 | Low Power Amplifier | 40dB gain, 2MHz BW, 20µW | Sensor Applications |
| Exercise 3 | Two-Stage OTA | 60dB gain, 100MHz GBW | General Purpose |
| Exercise 4 | Fully Differential Amp | 3x gain, >80dB DR | High-Performance |

---

## 🛠 Design Tools

- **Simulator:** Cadence Virtuoso
- **Technology:** CMOS
- **Design Methodology:** Custom analog IC design
- **Analysis Types:** DC, AC, Transient, Noise, Stability


---

## 🔬 Projects

### Exercise 1: Wi-Fi 6 Baseband Amplifier

**Objective:** Design a baseband amplifier for Wi-Fi 6 communication systems.

**Specifications:**
- **DC Gain:** 20 ± 0.1 dB
- **3-dB Bandwidth:** 20 ± 0.1 MHz
- **Max Power Consumption:** 200 µW
- **Supply Voltage:** VDD = 1.2V

**Key Features:**
- Single-stage amplifier topology
- Optimized for high-density wireless environments
- Achieved gain: 20.01 dB
- Achieved bandwidth: 20.05 MHz
- Actual power: 480 µW (exceeded target)

**Highlights:**
- All transistors operate in saturation region
- Trade-off analysis between gain, bandwidth, and power
- Detailed component selection rationale



---

### Exercise 2: Low Power Sensor Amplifier

**Objective:** Design a low-power amplifier optimized for sensor applications.

**Specifications:**
- **DC Gain:** 40 dB
- **3-dB Bandwidth:** 2 MHz
- **Max Power Consumption:** 20 µW
- **Supply Voltage:** VDD = 1V

**Key Features:**
- Differential pair with active loads
- Current mirror biasing
- Achieved gain: 39 dB
- Achieved bandwidth: 1.77 MHz
- Actual power: 21.61 µW

**Highlights:**
- Ultra-low power design techniques
- Systematic transistor sizing methodology
- DC and AC sweep analysis for optimization


---

### Exercise 3: Operational Transconductance Amplifier (OTA)

**Objective:** Design a two-stage CMOS OTA with high gain and stability.

**Specifications:**
- **Min Small Signal Gain:** 60 dB
- **Min GBW:** 100 MHz
- **Phase Margin:** >45°
- **Load Capacitance:** 10 pF
- **Supply Voltage:** VDD = 1V, VSS = -1V

**Key Features:**
- Two-stage architecture with Miller compensation
- Common-mode feedback (CMFB) circuit
- Achieved gain: 61.8 dB
- Achieved GBW: 121.24 MHz
- Phase margin: 113.44°
- Power: 6.063 mW

**Highlights:**
- Frequency compensation using Rc-Cc network
- High input impedance (2.7 GΩ)
- Excellent CMRR (65.6 dB)
- Slew rate: 5.13 V/µs


---

### Exercise 4: Fully Differential Amplifier

**Objective:** Design a fully differential two-stage operational amplifier with CMFB.

**Specifications:**
- **Closed Loop Gain:** 3
- **Dynamic Range:** >80 dB
- **Settling Error:** <0.5 mV
- **Settling Time:** <50 ns
- **Phase Margin:** >60°
- **Load Capacitance:** 10 pF
- **Supply Voltage:** VDD = 1.8V

**Key Features:**
- Fully differential topology
- Resistor-based CMFB circuit
- Four separate bias sub-circuits
- Achieved gain: 9.03 dB (closed-loop)
- Phase margin: 61.43°
- Gain margin: -13.23 dB
- Power: 35.64 mW

**Highlights:**
- NMOS differential pair with PMOS current mirror
- Miller compensation for stability
- CMRR: 6.2 KdB (extremely high)
- Slew rate: 0.88 V/µs


---

## 🎓 Key Learnings

Throughout these projects, we gained extensive experience in:

1. **Analog Circuit Design:**
   - Transistor sizing and biasing techniques
   - Trade-offs between gain, bandwidth, and power consumption
   - Operating point analysis and optimization

2. **Amplifier Topologies:**
   - Single-stage amplifiers
   - Differential pairs with active loads
   - Two-stage operational amplifiers
   - Fully differential architectures

3. **Frequency Compensation:**
   - Miller compensation techniques
   - Pole-zero analysis
   - Stability criteria (phase margin, gain margin)

4. **Circuit Analysis:**
   - DC operating point simulation
   - AC frequency response analysis
   - Transient behavior and slew rate
   - Noise analysis and dynamic range
   - Common-mode rejection ratio (CMRR)

5. **Design Methodology:**
   - Systematic design approach
   - Iterative optimization
   - Performance vs. specifications validation
   - Design documentation

---

## 📖 How to Use

### Viewing Documentation

Each project folder contains:
- **README.md:** Quick overview and key results
- **Design_Exercise_X.pdf:** Complete design report with schematics, simulations, and analysis

### Understanding the Designs

1. Start with the project-specific README for an overview
2. Review the PDF documentation for detailed analysis
3. Check the device dimension tables for transistor sizing
4. Study the simulation results and plots

### Replicating the Designs

To replicate these designs in Cadence Virtuoso:

1. Use the provided device dimensions and component values
2. Follow the schematic diagrams in the documentation
3. Set up the appropriate bias circuits
4. Configure simulations according to the specifications
5. Verify operating points match the documented values

---

## 📊 Performance Summary

| Parameter | Ex1 | Ex2 | Ex3 | Ex4 |
|-----------|-----|-----|-----|-----|
| **Gain** | 20.01 dB | 39 dB | 61.8 dB | 9.03 dB (CL) |
| **Bandwidth** | 20.05 MHz | 1.77 MHz | 121.24 MHz (GBW) | 52.19 MHz (GBW) |
| **Power** | 480 µW | 21.61 µW | 6.063 mW | 35.64 mW |
| **Phase Margin** | N/A | N/A | 113.44° | 61.43° |
| **Supply** | 1.2V | 1V | ±1V | 1.8V |

---

## 🤝 Contributing

These designs were created as part of an academic course in analog circuit design. While this is primarily an archive of completed work, suggestions and discussions are welcome through issues.

---

## 📝 License

This project is shared for educational purposes. Please cite appropriately if using these designs as reference material.


---

## 🙏 Acknowledgments

- Course instructors for guidance and feedback
- Cadence Design Systems for simulation tools
- Academic institution for providing resources

---

**Note:** All simulations and designs were performed using industry-standard tools and methodologies. Results may vary based on process technology and simulation parameters.
