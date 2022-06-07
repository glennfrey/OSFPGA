# FPGA - Fabric, Design and Architecture
FPGA - Fabric, Design and Architecture

![](bannerfpga.png)
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
History of programmable logic
- Programmable logic devices:
   * PLA – Programmable logic arrays
   * CPLD – Complex programmable logic device
   * FPGA
- Generate customisable hardware
- Study the effect of area, speed, power of the digital circuits


What is an FPGA?
* A “field programmable” gate array: Integrated circuit designed to be configured by a designer. FPGA configuration is specified using HDL similar to an ASIC (application specific Integrated circuit). Logic design in FPGA is different it uses LUTs, Flip-flops, configurable logic blocks.

ASIC vs FPGA
- ASIC(Application Specific Integrated Circuit) is designed from RTL to layout. Layout must be sent to semiconductor foundary for fabrication. ASIC cannot be reprogrammed.
- FPGA (Field Programmable Gate Array) is designed from RTL to bitstream. Design programmed on the FPGA which is bought off-the-shelf. FPGA can be re-programmed.

- Applications
   - Hardware acceleration
   - Signal processing
   - Device controllers
   - Embedded systems
   - Aerospace
   - High performance computing
   - Machine learning

FPGA Architecture
- Configurable logic blocks (CLB)-- Implement combinatorial and sequential logic. Based on LUT and Flip-flop/latches
- Look-up Tables (LUT) which implement the logic functions using truth table
- Carry and Control Logic- Implements arithmetic operations
- Flip Flops (FFs)/ Latches
- Memory Elements
- Programmable I/O blocks - Configurable I/Os for external interface connections
- Programmable interconnect- Wires to connect inputs, CLBs

## Vivado counter
![](fpgaday1/fpgaday1.png)
![](fpgaday1/fpgaday1createproj.png)
![](fpgaday1/fpgaday1boardparts.png)
![](fpgaday1/fpgaday1addcounterdesign.png)
![](fpgaday1/fpgaday1addtestbench.png)
![](fpgaday1/fpgaday1countersimulation.png)
![](fpgaday1/fpgaday1counterselaboration.png)
![](fpgaday1/fpgaday1counterselaborationioplanning.png)
![](fpgaday1/fpgaday1counterselaborationconstraints.png)
![](fpgaday1/fpgaday1counterssynthesistimingreport.png)
![](fpgaday1/fpgaday1counterssynthesistsolved.png)
![](fpgaday1/fpgaday1counterssynthesiswizardconstraint.png)
![](fpgaday1/fpgaday1counterssynthesisconstraintsummary.png)
![](fpgaday1/fpgaday1counterssynthesispositiveslack.png)
![](fpgaday1/fpgaday1counterssynthesisschematic.png)
![](fpgaday1/fpgaday1implementation.png)
![](fpgaday1/fpgaday1implementationutilization.png)
![](fpgaday1/fpgaday1implementationutilization2.png)
![](fpgaday1/fpgaday1implementatiocomplete.png)
![](fpgaday1/fpgaday1writebitstreamcomplete.png)
![](fpgaday1/fpgaday1openhardwaremngrautoconnect.png)

## VIO Counter

Different ways of programming
- Local programing on the Basys3 board
- Remote programing
   – Inputs through Virtual Input/Output and Outputs observed on the board
   – Inputs through Virtual Input/Output and Outputs observed on the Integrated Logic Analyzer (ILA)
![](fpgaday1/fpgaday1ipcatalogvio.png)
![](fpgaday1/fpgaday1vioioplanning.png)
![](fpgaday1/fpgaday1viobitstream.png)

## Day OpenFPGA2
## Part 1: OpenFPGA Intro

OpenFPGA

- To improve the design and development times of current methodologies to produce an FPGA which involve several hardware and software engineers and development for several months. OpenFPGA an Open source framework can be used to quickly generate a fabric for a custom FPGA (specific to your design).
   – Automation techniques used
   – Reduces FPGA development cycle of a new FPGA to a few days
   – Provides open source design tools

- Need for custom FPGAs?
   – Accelerate domain-specific applications: FPGA architectures have to be custom made, to provide maximum computing. Prototyping and producing a custom FPGA is costly and time-consuming.
   - Customise your own FPGA fabric using a set of templates (> 20 FPGA architectures- in xml files optimised for different applications)
   - Generates Verilog netlists describing an FPGA fabric based on an XMLbased description file: VPR’s (Versatile Place and Route) architecture description language
   - Allows you to write your own FPGA fabric (for a specific application) using OpenFPGA’s architecture description language
   - Automatically generates Verilog testbenches to validate the correctness of FPGA fabric
   - Bitstream generation support based on the same XML-based description file 

Running the tool
- The VTR detailed instruction can be found in this link: https://docs.verilogtorouting.org/en/latest/quickstart/
- In this workshop we don't have to Build OpenFPGA as it is done on cloud as well as build VTR.
- we can run VPR on a Pre-Synthesized Circuit and observe the result files then visualize (GUI) circuit implementation.
- Run the entire VTR flow automatically
   – Implement our own circuit in this workshop(counter.v) on a pre-existing FPGA architecture Earch.xml which can be found in $VTR_ROOT/vtr_flow/arch.
   – Use an automated approach (Odin II and ABC are automatically run) using python script
   – Perform timing simulation on the generated fabric

## Part 2: VPR
- To run VPR on a Pre-Synthesized Circuit you can check this link for more detailed information https://docs.verilogtorouting.org/en/latest/vpr/
   – Packing (combines primitives into complex blocks)
   – Placement (places complex blocks within the FPGA grid)
   – Routing (determines interconnections between blocks)
   – Analysis (analyzes the implementation)
● Input files are Blif file and Earch.xml
``$VTR_ROOT/vpr/vpr \
> $VTR_ROOT/vtr_flow/arch/timing/EArch.xml \
> $VTR_ROOT/vtr_flow/benchmarks/blif/tseng.blif \ --
> route_chan_width 100``
Run VPR on a Pre-Synthesized Circuit
● BLIF Netlist (.blif) - The technology mapped circuit to be implement on the target FPGA is specified as a Berkely Logic Interchange Format (BLIF) netlist. The netlist must be flattened and consist of only primitives (e.g. .names, .latch, .subckt). Clock and delay constraints can be specified with an SDC File.
● Outputs:
   - .net file: The circuit .net file is an xml file that describes a post-packed user circuit. It represents the user netlist in terms of the complex logic blocks of the target architecture. This file is generated from the packing stage and used as input to the placement stage in VPR.
![](fpgaday2/fpgaday2vprcommand.png)
![](fpgaday2/fpgaday2vprdisplay.png)
![](fpgaday2/fpgaday2vprblockselected.png)
![](fpgaday2/fpgaday2vprtogglenetsnets.png)
![](fpgaday2/fpgaday2vprtogglenetslogicalconnections.png)
![](fpgaday2/fpgaday2vprproceedplacement.png)
![](fpgaday2/fpgaday2vprproceedplacementdisplay.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplay.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplayrrcongested.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplaycritpath.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplayroutingutil.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplayblkinternal.png)
![](fpgaday2/fpgaday2vprproceedroutingdisplaynetpackplacegenerated.png)
![](fpgaday2/fpgaday2vprreport.png)
![](fpgaday2/fpgaday2vprslackreportnoconstraint.png)
![](fpgaday2/fpgaday2vprslackreportcosntraintfle.png)
![](fpgaday2/fpgaday2vprslackreportcosntraint.png)
## Part 3: VTR
VTR
● To check installation:
``$VTR_ROOT/vtr_flow/scripts/run_vtr_task.py basic_flow``
– Expected output: ``k6_N10_memSize16384_memData64_40nm_timing/ch_intrinsics...OK``
● To run command VTR for Counter input the following command:
``$VTR_ROOT/vtr_flow/scripts/run_vtr_flow.pl \
> $VTR_ROOT/doc/src/quickstart/counter.v \
> $VTR_ROOT/vtr_flow/arch/timing/EArch.xml \
> -temp_dir . \
> --route_chan_width 100``
● To open GUI for above design
``$VTR_ROOT/vpr/vpr \
   > $VTR_ROOT/vtr_flow/arch/timing/EArch.xml \
   > counter --circuit_file counter.pre-vpr.blif \
   > --route_chan_width 100 \
   > --analysis --disp on``
![](fpgaday2/fpgaday2vprcounterv.png)
![](fpgaday2/fpgaday2vprcounterblif.png)
![](fpgaday2/fpgaday2vprcounterblifdisplay.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaylogicalcon.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaycritpath.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaynoanalysis.png)
![](fpgaday2/fpgaday2vprcounterblifdisplayplacementcomplete.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaytogglerr.png)
![](fpgaday2/fpgaday2vprcounterblifdisplayroutingcomplete.png)
● To run VPR for Post implimentation netlist timing simulation
- We need to provide the vpr --gen_post_synthesis_netlist option to generate the post-implementation netlist and dump the timing information in Standard Delay Format(SDF):
``$VTR_ROOT/vpr/vpr \
> $VTR_ROOT/vtr_flow/arch/timing/EArch.xml \
> counter.pre-vpr.blif --gen_post_synthesis_netlist on``
![](fpgaday2/fpgaday2vprcounterblifpostsynthesis.png)
![](fpgaday2/fpgaday2vprcounterblifpostsynthesisvfile.png)
![](fpgaday2/fpgaday2vprcounterblifprimitivesntestbench.png)
![](fpgaday2/fpgaday2vprcounterblifvivadopostsimulation.png)
![](fpgaday2/fpgaday2vprcounterblifvivadosources.png)
![](fpgaday2/fpgaday2vprcounterblifvivadoeditcounter.png)
![](fpgaday2/fpgaday2vprcounterblifvivadosimulation.png)
![](fpgaday2/fpgaday2vprcounteprevprblif.png)
![](fpgaday2/fpgaday2vprcounteprevprblifedited.png)
![](fpgaday2/fpgaday2vprcounteprevprblifcomman.png)
![](fpgaday2/fpgaday2vprcounteprevprblifcommandsucceeded.png)
![](fpgaday2/fpgaday2vprcounteprevprblifreportslack.png)
![](fpgaday2/fpgaday2vprcounteprevprbliflogblocks.png)
![](fpgaday2/fpgaday2vprcounteprevprblifloglogicelement.png)
![](fpgaday2/fpgaday2vprcounteprevprbliflogdetail.png)
![](fpgaday2/fpgaday2vprcounteprevprblifpower.png)
![](fpgaday2/fpgaday2vprcounteprevprblifcounterpwr.png)
![](fpgaday2/fpgaday2vprcounteprevprblifcounterpwr2.png)
## Day 3 Introduction to RISC-V core programming on Vivado
## Part 1: RVMyth vivado rtl-to-synthesis
![](fpgaday3/fpgaday3testedit.png)
![](fpgaday3/fpgaday3riscvwaveform.png)
![](fpgaday3/fpgaday3riscvwithILA.png)
![](fpgaday3/fpgaday3riscvwithILAelaboraiton.png)
![](fpgaday3/fpgaday3riscvwithILAconstraints.png)
## Part 2: RVMyth Vivado synthesis-to-bitstream
![](fpgaday3/fpgaday3riscvwithILAutilazationrptt.png)
![](fpgaday3/fpgaday3riscvwithILAsummary.png)
![](fpgaday3/fpgaday3riscvwithILschematic.png)
![](fpgaday3/fpgaday3riscvwithILfloorplan.png)
![](fpgaday3/fpgaday3riscvwithILfloorplan0.png)
![](fpgaday3/fpgaday3riscvwithILfloorplanhighlightnets.png)
![](fpgaday3/fpgaday3riscvwithILtimingsummary.png)
![](fpgaday3/fpgaday3riscvwithILwirtebitstreamnotarget.png)


## Day 4 Introduction to SOFA FPGA Fabric IP
## Part1 SOFA counter area]
![](fpgaday4/fpgaday4configlocation.png)
![](fpgaday4/fpgaday4generatetestbenchfpg.png)
![](fpgaday4/fpgaday4generatetestbenchfpgainside.png)
![](fpgaday4/fpgaday4vprarchi.png)
![](fpgaday4/fpgaday4vmakefile.png)
![](fpgaday4/fpgaday4vlogfiles.png)
![](fpgaday4/fpgaday4vlogopenshellfpga.png)
![](fpgaday4/fpgaday4vlogvprstd.png)
## Part2 SOFA counter timing]
![](fpgaday4/fpgaday4vlogvprstdareareport.png)
![](fpgaday4/fpgaday4vlogvprstdareareport2.png)
![](fpgaday4/fpgaday4countersdc.png)
![](fpgaday4/fpgaday4changegeneratetestbenchfpga.png)
![](fpgaday4/fpgaday4changegeneratetestbenchfpgaedit.png)
![](fpgaday4/fpgaday4changegeneratetestbenchfpgaeditlog.png)
![](fpgaday4/fpgaday4changegeneratetestbenchfpgaeditreport.png)
![](fpgaday4new/fpgaday4upcounterconfedit.png)
![](fpgaday4new/fpgaday4upcountergeneratetestbenchfpga.png)
![](fpgaday4new/fpgaday4upcountersetupsimulationreport.png)
![](fpgaday4new/fpgaday4upcounterholdsimulationreport.png)
## Part3 SOFA counter post impl
![](fpgaday4new/fpgaday4postupcountergeneratetbfpga.png)
![](fpgaday4new/fpgaday4postupcounterfile.png)
![](fpgaday4new/fpgaday4postupcounterfileclock.png)
![](fpgaday4new/fpgaday4postupcounterfilegenerated.png)
![](fpgaday4new/fpgaday4postsimulationupcounter.png)
![](fpgaday4new/fpgaday4postsimulationupcountertbcod.png)
![](fpgaday4new/fpgaday4postsimulationupcounterprimitivescode.png)
![](fpgaday4new/fpgaday4postsimulationupcounterresult.png)
![](fpgaday4new/fpgaday4upcounterraceact.png)
## Part4 counter power
![](fpgaday4new/fpgaday4vprpowergeneratetestbenchfpgaedit.png)
![](fpgaday4new/fpgaday4vprarchxmlfilescodeaddedforpoweranalysis.png)
![](fpgaday4new/fpgaday4poweranalysistasksimulation.png)
![](fpgaday4new/fpgaday4poweranalysisbreakdown.png)
![](fpgaday4new/fpgaday4poweranalysisbreakdown2.png)

## Day 5 RISC-V core on custom SOFA fabric
## Part1 SOFA-RVMyth run
![](fpgaday5rvmythgeneratetbfpga.png)
![](fpgaday5simulationconf.png)
![](fpgaday5rvmythvprarchedited.png)
![](fpgaday5/fpgaday51stcommandopenfpgashelllog.png)
![](fpgaday5/fpgaday51stcommandvprstdoutlog.png)
## Part2 SOFA-RVMyth timing and area
![](fpgaday5/fpgaday51stcommandvprstdoutlogcrctstat.png)
![](fpgaday5/fpgaday51stcommandvprstdoutloglogicelements.png)
![](fpgaday5/fpgaday5timinganalysissdcadditioningeneratetbfpga.png)
![](fpgaday5/fpgaday5timinganalysissetupreport.png)
![](fpgaday5/fpgaday5timinganalysholdreport.png)
![](fpgaday5/fpgaday5timinganalysopenshellfpga.png)
![](fpgaday5/fpgaday5timinganalysvprstdoutlog.png)


## Part3 RVMyth-post impl netlist
![](fpgaday5/fpgaday5corepostsynthesisgenerated.png)
![](fpgaday5/fpgaday5corepostsynthesiscode.png)
![](fpgaday5/fpgaday5corepostsynthesiscodeclock.png)

## Part4 SOFA-RVMyth Vivado simulation
![](fpgaday5/fpgaday5testv.png)
![](fpgaday5/fpgaday5primitives.png)
![](fpgaday5/fpgaday5vivadowithfiles.png)
![](fpgaday5/fpgaday5vivadosimulation.png)
![](fpgaday5/fpgaday5vivadosimulation2.png)
![](fpgaday5/fpgaday5vivadoomplementation.png)
![](fpgaday5/fpgaday5poweranalysis.png)
![](fpgaday5/fpgaday5poweranalysisaddlinesvpr_archxml.png)
