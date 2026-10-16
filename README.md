# 6T SRAM Cell Characterization: CMOS & FinFET

## Overview
This repository contains the design, schematic capture, and performance characterization of 6T SRAM cells. The project evaluates and compares the static and dynamic metrics of SRAM topologies across multiple technology nodes, analyzing the performance shifts when transitioning from bulk CMOS to FinFET architectures. 

## Technology Nodes
The designs and simulations are implemented across the following process nodes:
* 180nm CMOS
* 90nm CMOS
* 45nm CMOS
* 18nm FinFET

## Characterization & Analysis
The project executes comprehensive performance evaluations using Cadence Virtuoso, including:
* **DC Analysis:** Static Noise Margin (SNM) extraction via read/write butterfly curves. 
* **Transient Analysis:** Read/write access times, delay metrics, and dynamic waveform behavior.
* **Thermal & Power Analysis:** Leakage and active power variations under thermal scaling (documented in power vs. temperature plots).

## Repository Structure
* `SRAM_FINFET/cmos_sram/` - Standard bulk CMOS schematics, layout data, and symbol views for 180nm, 90nm, and 45nm nodes.
* `SRAM_FINFET/SRAM/FINFET/` - FinFET-specific schematic implementations and characterization setups.
* `SRAM_FINFET/cds.lib` - Cadence library definition file.
* `*.oa` & `data.dm` - OpenAccess database files defining the cell views and properties.

## Getting Started
1. Clone the repository to your local Cadence working directory.
2. Ensure the required Generic Process Design Kits (GPDK 180/90/45) and your target FinFET PDK are installed.
3. Update the `cds.lib` file to correctly point to your local PDK installation paths.
4. Launch Virtuoso and open the respective schematic views to run ADE L/XL testbenches.

## Author
**Prerna Shringarpure**  
**Aribah Shirgaonker**  
**AbdulMannan Ansari**  
Vidyalankar Institute of Technology  
B.Tech, Electronics and Computer Science
