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
![](fpgaday1/fpgaday1ipcatalogvio.png)
![](fpgaday1/fpgaday1vioioplanning.png)
![](fpgaday1/fpgaday1viobitstream.png)

## Day OpenFPGA2
## Part 1: OpenFPGA Intro



## Part 2: VPR
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

![](fpgaday2/fpgaday2vprcounterv.png)
![](fpgaday2/fpgaday2vprcounterblif.png)
![](fpgaday2/fpgaday2vprcounterblifdisplay.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaylogicalcon.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaycritpath.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaynoanalysis.png)
![](fpgaday2/fpgaday2vprcounterblifdisplayplacementcomplete.png)
![](fpgaday2/fpgaday2vprcounterblifdisplaytogglerr.png)
![](fpgaday2/fpgaday2vprcounterblifdisplayroutingcomplete.png)
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



