---
title: "RTL to GDS II : Cadence Genus Inputs"
description: >-
  This blog breifly describes the rtl to gdsII and input files needed for Cadence Genus Synthesis and their functions.
author: Ravidu Munasinghe
date: 2025-03-08 10:00:00 -0500
categories: [Blogging, Digital IC Design]
tags: [Genus, Synthesis]
pin: false
blog: true
image:
  path: 
  alt: 
---

## RTL to GDS II
The RTL to GDSII flow is the end-to-end process of converting a hardware design from abstract code into a physical chip layout ready for fabrication. Following are the major steps involved in RTL to GDSII. This is an iterative process though it seems like a linear process. For example, Static Timing Analysis is ususally done after synthesis, placement, cts and routing to check whether any timing violations.

1. RTL Design & Verification - Specifications, RTL Design and Functional Verification
2. Synthesis - Compile RTL code into a Gate-Lvel Netlist using Standard Cell Libraries from the foundary (TSMC, Samsung).
3. Design for Test (DFT) - Insert Scan chanins to detect fabrication defects.
4. Floorplanning - Define Chip area, place macros blocks, and plan power distribution.
5. Place & Route (PnR) - Standard Cells are placed and interconnected with metal wires
6. Static Timing Analysis (STA) - Verify all timing paths meet setup/hold constraints across Process, Voltage and Temperature corners(PVT).
7. Physical Verification - Check the Design for Design Rule Check (DRC) files provided by foundary. Also check the design's Layout vs Schematic (LVS).
8. GDSII Tapeout - The final layout is streamed out as a GDSII file. This file will be sent to the foundary for fabrication.

## Cadence EDA Tools
Cadence provides comprehensive suite of tools covering every stage of the RTL to GDS II flow.

![RTL to GDSII Cadence EDA Tools](assets/img/blogs/digital/frontend/Cadence_Tools.png "Cadence EDA Tools for Digital IC Design")

## Cadence Genus Synthesis Solution


## Inputs for Genus

#### Standard Cell Libraries - .lib files


## References

- [Cadence White Paper - Best Full-Flow PPA](https://www.cadence.com/en_US/home/resources/white-papers/best-full-flow-ppa-wp.html)


<!-- ````sv
module counter (
  input  logic clk,
  input  logic rst_n,
  output logic [7:0] count
);
  always_ff @(posedge clk or negedge rst_n) begin
    if (!rst_n) count <= 8'h00;
    else        count <= count + 1;
  end
endmodule
````

````tcl
proc greet {name} {
  puts "Hello, $name!"
}

greet "World"
```` -->
