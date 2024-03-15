# NASSCOM-VSD-SOC
This repository consists of a 5 Day workshop conducted by NASSCOM and VSD on SOC Design and Planning. Also, this includes all the 5 Days learning from videos provided by VSD and LAB work on the OpenLANE tool provided by NASSCOM.<br><br>
Author- Tanmay Agrawal
<br>
## Table Of Content
<ol>
  <li>
    <a href= "#day-1">Day-1: Inception of open-source EDA, OpenLANE and Sky130 PDK.</a>
  </li>
  <li><a href="day-2">Day-2: Inception of open-source EDA, OpenLANE and Sky130 PDK.</a></li>
  <li><a href="day-3">Day-3: Inception of open-source EDA, OpenLANE and Sky130 PDK.</a></li>
  <li><a href="day-4">Day-4: Inception of open-source EDA, OpenLANE and Sky130 PDK.</a></li>
  <li><a href="day-5">Day-5: Inception of open-source EDA, OpenLANE and Sky130 PDK.</a></li>
</ol>
<br>

## DAY-1
### Title: Inception Of Open-Source EDA, OpenLANE and Sky130 PDK.
<hr>
<h5>CONTENT:</h5>
<ol>
  <li>SKY130_D1_SK1: How to talk to computers</li>
  <li>SKY130_D1_SK2: SOC Design and OpenLANE</li>
  <li>SKY130_D1_SK3: Get familiar to open-source EDA tools</li>
</ol>
<hr>

### 1. SKY130_D1_SK1: How to talk to computer
<hr>
<img src="./day11.png">
<br>
This is the Arduino Leonardo board consisting of a Processor/SOC and various other interconnecting devices and peripherals.<br>
The highlighted part in the above figure is the on block where the entire VLSI moves around.<br><br>
The picture below dipicts the layout of the entire microcontroller board.<br>
<img src="./day12.png">
<br>
Thus, this picture consists of various interconnect devices, external chips and various other devices present. Few features of this layout are:<br>
<ul>
  <li>The Centre part the processor/ SOC is the layout of the Chip that is highlighted on an Arduino Board.</li>
  <li>It comprises of various other devices like SRAM, EEPROM, ADCs and various other components that are combined and placed to make a microcontroller board </li>
</ul>
<br>
But, our main objective is to design a Processor/ SOC so the picture below depicts the design of a QFN-48 Package with the chip in the middle of it connected by bond wires or interconnect wires.
<br>
<img src="day13.png">
<br>
Also this Package comprises of a Die, I/O Pads, core. The layout of this is depicted below:<br>
<img src="day14.png">
<br>
Now, the core of this SOC consists of the Two major parts these are:<br>
<ul>
  <li>Foundry IP's: These the factories that helps to implement the design on the silicon wafer and also to make chips by there intelligence. These chips made by the foundrys are termed as foundry Intellectual Property.</li>
  <li>Macros: These are like a pure digital logics.</li>
</ul>
<img src="day15.png">
<br>
As, we are using RISC V Architecture also called Instruction Set Architecture (ISA) to design an SOC. The picture below depicts the flow from RTL2GDS.
<img src="day16.png">
<br>
Now, Let's move on to how the Software Applications connects to Hardwares.<br>
Shown, below is the entire flow of how the software connects to Hardware.
<br>
<img src="day17.png">
<br>
Now, we are taking the example of a stop watch flow and the implementation is done using RISCV Architecture.<br>
<img src="day18.png">
<br>
Thus, deep diving into the flow we observed that there is one more process after the Assembler is the use of HDL(Hardware Descriptive Language).<br>
We, convert the Binary Code into the HDL that signifies that what is the function that the entire hardware will be performing with that bit stream.<br>
Then, the next step after this is we synthesize the RTL flow for Physical Design Implementation.<br>
<img src="day19.png">
<br>
<hr>

### 2. SKY130_D1_SK2: SOC Design and OpenLANE

<hr>
<br>
 Let's understand the standard RTL to GDSII Flow. This is described below using the flow diagram:
 <br>
 <img src="day120.png">
 <br>
 Now, let's take the first stage in the flow:<br>
 Synthesis: It Converts RTL to a circuit out of components from the standard cell library (SCL).<br>
 <img src="day21.png">
 <br>
 The other stage is:<br>
 Floor and Power Planning: It is divided into two categories that are :<br>
 <ol>
   <li>Chip-Floor Planning: Partition the chip die between different system building blocks and place the I/O Pads.</li>
   <li>Macro-Floor Planning: Dimensions, pin locations, rows definition.</li>
 </ol>
 <img src="day22.png"><br><img src="day23.png"><br>
 Power Planning: The power network is connected by multiple vdd, vss and gnd.
 <br>
 <img src="day24.png">
 <br>
 The next stage is:<br>
 Placement: Placing the cells on the floorplan rows, aligned with the sites.<br>
 <img src="day25.png">
 <br>
 Placement is divided into 2 steps: Global and Detailed Placement.<br>
 <img src="day26.png">
 <br>
 The next stage is:<br>
 <img src="day27.png">
 <br>
The next stage is:<br>
 <img src="day27.png">
 <br>
 The next stage is:<br>
 <img src="day27.png">
 <br>
 <hr>

### 3. SKY130_D1_SK3: Get familiar to open-source EDA tools
 
 <hr>
 
 
 
 
 
 
 
