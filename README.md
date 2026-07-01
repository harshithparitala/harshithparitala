<h1 align="center">Harshith Paritala</h1>
<h3 align="center">ASIC / Physical Design Engineer · RTL Design · FPGA Development · Open-Source VLSI</h3>

<p align="center">
Electronics & Communication Engineer specializing in RTL-to-GDSII digital design flows, physical implementation, and open-source silicon (Sky130 / OpenLane). Building accelerator architectures and semiconductor devices from RTL through tapeout.
</p>

<p align="center">
<a href="mailto:saiharshith.paritala@gmail.com">Email</a> ·
<a href="https://github.com/harshithparitala">GitHub</a> ·
<a href="#">LinkedIn</a>
</p>

---

## About

I'm a 2026 B.Tech graduate in Electronics & Communication Engineering from Amrita Vishwa Vidyapeetham, Coimbatore, focused on ASIC Physical Design, Digital Design Verification, and FPGA development. My work spans the full digital design stack — writing RTL in Verilog/SystemVerilog/VHDL, verifying it with testbenches and assertions, and carrying designs through synthesis, place-and-route, and static timing analysis using both open-source (OpenLane, OpenROAD, Sky130 PDK) and commercial (Cadence Innovus) toolchains.

Alongside implementation work, I do research in reconfigurable hardware architecture (CGRA scalability using the HyCube framework) and compound semiconductor devices (GaN HEMT modeling in Silvaco TCAD). I hold the Samsung ISWDP Fellowship (Levels 1 & 2) and maintain technical documentation for every project I ship — from constraint files and timing reports to architecture write-ups.

I'm currently deepening my skills in advanced physical design: clock tree synthesis, timing closure, multi-corner STA, and ECO flows.

---

## Core Expertise

| Domain | Focus |
|---|---|
| **RTL Design** | Verilog, SystemVerilog, VHDL — combinational & sequential digital logic |
| **ASIC Physical Design** | Floorplanning, placement, CTS, routing, timing closure (OpenROAD, Cadence Innovus) |
| **Physical Verification** | DRC, LVS, tapeout-readiness sign-off using Sky130 |
| **Design Verification** | Testbench development, functional coverage, waveform-based debug |
| **FPGA Development** | Basys3 (Artix-7), PYNQ, VSD Squadron Mini — synthesis to hardware validation |
| **Open-Source ASIC Flow** | OpenLane, Sky130 PDK, Yosys, full RTL-to-GDSII flows |
| **Research** | CGRA architecture exploration, GaN HEMT device simulation |

---

## Technical Stack

**Languages & HDLs**

| Category | Tools |
|---|---|
| HDLs | Verilog, SystemVerilog, VHDL |
| Programming | Python, C, C++ |
| Scripting | TCL |

**EDA & Physical Design**

| Category | Tools |
|---|---|
| Physical Design | Cadence Innovus, OpenROAD, OpenLane |
| Synthesis | Yosys, Vivado |
| Simulation | ModelSim, Vivado Simulator, EDA Playground |
| Device Simulation | Silvaco TCAD, Ansys HFSS |
| PCB Design | KiCad, LTspice |
| PDKs | Sky130 (SkyWater 130nm) |

**Platforms & Tools**

| Category | Tools |
|---|---|
| Hardware Platforms | Basys3, PYNQ, VSD Squadron Mini (CH32V RISC-V), Arduino, ESP32/ESP8266 |
| Operating Systems | Linux, Windows |
| Version Control | Git, GitHub |

---

## Featured Projects

### 8-bit ALU — RTL to GDSII
**Full-flow ASIC implementation** carried from RTL through GDSII using Cadence Innovus.
- **Problem:** Demonstrate an end-to-end digital implementation flow with quantifiable timing and area closure.
- **Approach:** Synthesized and place-and-routed an 8-bit ALU, applying SDC constraints, clock tree synthesis, and static timing analysis to close on setup/hold.
- **Tools:** Cadence Innovus, Verilog, SDC
- **Key Achievements:** Delivered a complete, sign-off-ready design with documented timing (WNS/TNS), utilization, and DRC metrics.
- **Repository:** [link]

### Physical Verification for Tapeout Readiness — Sky130
**Open-source physical verification** project preparing a design for tapeout.
- **Problem:** Ensure a physical layout meets DRC and LVS sign-off criteria on an open PDK.
- **Approach:** Ran design rule and layout-vs-schematic checks against the Sky130 PDK to validate tapeout readiness.
- **Tools:** Sky130 PDK, open-source PV tools
- **Repository:** [link]

### 3×3 Systolic Array — Dual-Mapped ASIC & FPGA
**Parallel matrix-multiplication accelerator** implemented for both open-source silicon and FPGA fabric.
- **Problem:** Explore compute-bound scalability of systolic architectures under real hardware constraints.
- **Approach:** Designed a 3×3 systolic array in Verilog, mapped it to Sky130 ASIC flow (`tt-gf180-systolic-array`) and separately synthesized it for Artix-7 FPGA (`systolic_array-3x3-matrix`), verifying parallel throughput on both targets.
- **Tools:** Verilog, OpenLane/Sky130, Vivado, Basys3
- **Key Achievements:** Validated the same architecture across two physically distinct implementation targets.
- **Repositories:** [link] · [link]

### PicoRV32a RISC-V SoC — RTL to GDSII
**Open-source RISC-V core** carried through gate-level simulation and physical implementation on Sky130.
- **Problem:** Implement and verify a RISC-V SoC using a fully open-source ASIC toolchain.
- **Approach:** Ran the PicoRV32a core through OpenLane, performed gate-level simulation (GLS) to confirm post-synthesis functional equivalence.
- **Tools:** OpenLane, Sky130 PDK, Verilog
- **Repository:** [link]

### CGRA Architecture Research — HyCube Scalability
**Reconfigurable architecture research** benchmarking routing efficiency in coarse-grained reconfigurable arrays.
- **Problem:** Evaluate how CGRA routing overhead scales with array size and interconnect topology.
- **Approach:** Used the HyCube framework and CGRA-ME compiler infrastructure to benchmark routing node utilization across configurations.
- **Tools:** HyCube, CGRA-ME
- **Key Achievements:** Achieved a 96.5% reduction in required routing nodes through architectural exploration.
- **Repositories:** `CGRA_ME` · `morpher_cgra` [links]

### Counter — ASIC vs. FPGA Comparison
**Comparative implementation study** of the same RTL design across ASIC and FPGA flows.
- **Problem:** Quantify differences in area, timing, and resource usage between ASIC and FPGA implementations of an identical design.
- **Approach:** Implemented a counter in Verilog and independently carried it through both an ASIC flow and FPGA synthesis, comparing results.
- **Tools:** Verilog, OpenLane/Sky130, Vivado
- **Repository:** [link]

### BCD-to-7-Segment Decoder with SystemVerilog Testbench
**Verification-focused project** demonstrating structured testbench methodology.
- **Problem:** Verify combinational decoder logic against expected truth-table behavior.
- **Approach:** Built a SystemVerilog testbench with self-checking assertions to validate decoder outputs across all input combinations.
- **Tools:** SystemVerilog
- **Repository:** `fulladder` / related decoder work [link]

### Square Wave Generator Metronome — VHDL, Basys3
**FPGA-based timing generator** with VGA and audio output.
- **Problem:** Generate a frequency-controlled square wave for a hardware metronome application.
- **Approach:** Designed a 4-bit frequency-controlled generator in VHDL with VGA display and passive buzzer interfacing, verified on Basys3 hardware.
- **Tools:** VHDL, Basys3
- **Repository:** [link]

### Pmod Keypad Interfacing — VHDL, Basys3
**Peripheral interfacing project** connecting a matrix keypad to FPGA fabric.
- **Approach:** Implemented keypad scanning and debounce logic in VHDL, interfaced via Pmod connector on Basys3.
- **Tools:** VHDL, Basys3
- **Repository:** [link]

---

## Research Experience

**CGRA Architecture — Scalability & Routing Efficiency**
Investigated architectural scalability of coarse-grained reconfigurable arrays using the HyCube framework and CGRA-ME compiler infrastructure, benchmarking routing node reduction across array configurations for compute-bound accelerator workloads.

**GaN HEMT Device Simulation — Silvaco TCAD**
Conducted device-level simulation and optimization of GaN High Electron Mobility Transistors targeting 650V-class power applications, under the supervision of Dr. Abhishek Raj, using Silvaco TCAD for device physics modeling.

---

## Experience

**Engineering Intern — Firmware & Systems, SATCARD (IIT Palakkad)**
Implemented OTA firmware update mechanisms for ESP32 modules over the A7672S cellular module, designing remote update and validation workflows for reliable field deployment. *(`NodeMCU-OTA-Updates`)*

**Hardware Intern — VLSI System Design**
Contributed to RTL verification and synthesis for ASIC prototyping using industry-standard toolchains, supporting design correctness ahead of physical implementation.

---

## Certifications

- Samsung ISWDP Fellowship — Level 1 & Level 2
- Fundamentals of SystemVerilog — Namaste FPGA

---

## GitHub Highlights

| Category | Focus Areas |
|---|---|
| **ASIC / Physical Design** | RTL-to-GDSII flows, Cadence Innovus, physical verification |
| **RTL & Verification** | Verilog, SystemVerilog, VHDL, testbench development |
| **FPGA** | Basys3, PYNQ, VSD Squadron Mini implementations |
| **Research** | CGRA architecture, GaN HEMT device modeling |
| **Embedded Systems** | ESP32 OTA firmware, sensor interfacing, PCB design |
| **Open Source** | OpenLane / Sky130 RTL-to-GDSII projects |

---

## Currently Learning

Advanced Physical Design · Clock Tree Synthesis · Multi-Corner STA · Timing Closure · ECO Flows · OpenROAD · Digital IC Design

---

## Connect

I'm actively pursuing roles in ASIC Physical Design, RTL/Digital Design, and Design Verification. Open to conversations about semiconductor design, open-source EDA, or accelerator architecture.

- **Email:** saiharshith.paritala@gmail.com
- **GitHub:** [github.com/harshithparitala](https://github.com/harshithparitala)
- **LinkedIn:** [add link]
