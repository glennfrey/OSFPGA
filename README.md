# OSFPGA
Open Source FPGA

![](risc-v/risc-v_banner.png)
### ABOUT THE WORKSHOP
The Workshop is a 5-day basic to advance program that is design for fresher and professional who wants to build a career in VLSI industry. It is a cloud based workshop that comprises of training courses that covers RISC-V specs, RISC-V software, How to implement RISC-V basic specs using TL-Verilog and Simulate your own RISC-V core. In short, you are going to write RTL and build RISC-V core on your own.
### AUTHOR OF THE WORKSHOP
#### Mr. Kunal Ghosh
Co-founder of VLSI System Design (VSD) Corporation Private Limited
#### 
### AGENDA
 [Day 1 Intro](#Day1-Intro)
  * [Part 1: FPGA introduction](#Part1-FPGA-introduction)
  * [Part 2: Vivado-counter](#Part2-Vivado-counter)
  * [Part 3: VIO Counter](#Part3-VIO-Counter)
 
 [Day OpenFPGA2](#Day2-OpenFPGA)
  * [Part 1: OpenFPGA Intro](#Part1-OpenFPGA-Intro)
  * [Part 2: VPR](#Part2-VPR)
  * [Part 3: VTR](#Part3-VTR)

 [Day 3 Introduction to RISC-V core programming on Vivado](#Day3-Introduction-to-RISC-V-core-programming-on-Vivado)
  * [Part 1: RVMyth vivado rtl-to-synthesis](#Part1-RVMyth-vivado-rtl-to-synthesis)
  * [Part 2: RVMyth Vivado synthesis-to-bitstream](#Part2-RVMyth-Vivado-synthesis-to-bitstream)

 [Day 4 Introduction to SOFA FPGA Fabric IP](#Day4-Introduction-to-SOFA-FPGA-Fabric-IP)
  * [Part 1: SOFA counter area](#Part1-SOFA-counter-area)
  * [Part 2: Fetch, decode, and execute logic](#Part2-SOFA-counter-timing)
  * [Part 3: SOFA counter post impl](#Part3-SOFA-counter-post-impl)
  * [Part 4: SOFA counter power](#Part4-SOFA-counter-power)

 [Day 5 RISC-V core on custom SOFA fabric](#Day5-RISC-V-core-on-custom-SOFA-fabric)
  * [Part 1: SOFA-RVMyth run](#Part1-SOFA-RVMyth-run)
  * [Part 2: SOFA-RVMyth timing and area](#Part2-SOFA-RVMyth-timing-and-area)
  * [Part 3: RVMyth-post impl netlist](#Part3-RVMyth-post-impl-netlist)
  * [Part 4: SOFA-RVMyth Vivado simulation](#Part4-SOFA-RVMyth-Vivado-simulation)
  
## Day1-Intro
## FPGA introduction







## Vivado counter
![fpgaday1](https://user-images.githubusercontent.com/93269547/171854840-3bb922b7-f1b9-40b4-9894-e6d65975d77a.png)
![fpgaday1createproj](https://user-images.githubusercontent.com/93269547/171854856-421979c6-9f2f-416a-b46d-28cbc39a0cee.png)
![fpgaday1boardparts](https://user-images.githubusercontent.com/93269547/171854887-b9af70e6-e9b9-49f8-bd63-5de7235e556b.png)
![fpgaday1addcounterdesign](https://user-images.githubusercontent.com/93269547/171854908-686871c0-92cc-4ec3-bc3e-05a4401640ca.png)
![fpgaday1addtestbench](https://user-images.githubusercontent.com/93269547/171854913-483c2fbd-5e3e-42c2-b921-4b65ca8ed0a2.png)
![fpgaday1countersimulation](https://user-images.githubusercontent.com/93269547/171854920-b1812845-738c-48aa-86e1-03a6c7ccc4a6.png)
![fpgaday1counterselaboration](https://user-images.githubusercontent.com/93269547/171854947-d3175bea-67c6-463a-9d80-e765c544f4f6.png)
![fpgaday1counterselaborationioplanning](https://user-images.githubusercontent.com/93269547/171854964-9e894f89-984c-4d2b-b9aa-650447548b32.png)
![fpgaday1counterselaborationconstraints](https://user-images.githubusercontent.com/93269547/171855045-dcd8e957-c302-4f54-ae61-2a4e414aeac0.png)
![fpgaday1counterssynthesistimingreport](https://user-images.githubusercontent.com/93269547/171855060-8e4f1252-695b-4680-9b30-6cf03d92faa0.png)
![fpgaday1counterssynthesistsolved](https://user-images.githubusercontent.com/93269547/171855069-12925146-ebb2-4f68-88e9-9f17461a13ca.png)
![fpgaday1counterssynthesiswizardconstraint](https://user-images.githubusercontent.com/93269547/171855076-32208e2d-882b-4d10-b4e2-fbbd6557b349.png)
![fpgaday1counterssynthesisconstraintsummary](https://user-images.githubusercontent.com/93269547/171855088-f7a9a475-7e54-4ce8-8c7c-80db4177b01e.png)
![fpgaday1counterssynthesispositiveslack](https://user-images.githubusercontent.com/93269547/171855118-f6087ff9-9b8d-43d5-963e-c9f64c819027.png)
![fpgaday1counterssynthesisschematic](https://user-images.githubusercontent.com/93269547/171855133-fd06dd43-52d5-476f-ab86-36893941e9dc.png)
![fpgaday1implementation](https://user-images.githubusercontent.com/93269547/171855142-36114075-88c9-4104-bad6-a477943260fa.png)
![fpgaday1implementationutilization](https://user-images.githubusercontent.com/93269547/171855153-21de0954-43c5-42d6-a2af-f4286d5757b5.png)
![fpgaday1implementationutilization2](https://user-images.githubusercontent.com/93269547/171855160-f52e3bc7-2b95-4b55-81de-ab32c892cad7.png)
![fpgaday1implementatiocomplete](https://user-images.githubusercontent.com/93269547/171855185-6e94c1d7-72b0-4126-8b28-8cb87ea4a9e5.png)
![fpgaday1writebitstreamcomplete](https://user-images.githubusercontent.com/93269547/171855203-3702a2a6-da1e-464e-9abf-774d7f690aeb.png)
![fpgaday1openhardwaremngrautoconnect](https://user-images.githubusercontent.com/93269547/171855215-7feb0fa0-ee67-46c0-934a-11d7847a3508.png)

## VIO Counter
![fpgaday1ipcatalogvio](https://user-images.githubusercontent.com/93269547/171855266-26ca29dc-005f-41cf-aef7-c90d40a0f626.png)
![fpgaday1vioioplanning](https://user-images.githubusercontent.com/93269547/171855274-332cabf3-f1a4-42b3-805e-185f33cf8b44.png)
![fpgaday1viobitstream](https://user-images.githubusercontent.com/93269547/171855289-dde8037b-82ca-4b42-b52c-2373f6844fda.png)






