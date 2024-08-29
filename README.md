# Contents

<div class="toc">
	<ul>
    		<li><a href="#header-1">Sky130 Day 1 - Inception of open-source EDA, OpenLANE and Sky130 PDK</a></li>
		<ul>
        		<li><a href="#header-1-1">Sky130_D1_SK3  - Get familiar to open-sorce EDA tools</a></li>
 		<ul>
			<li><a href="#header-1-1-1">SKY_L1 - OpenLANE Directory Structure in detail</a></li>
		</ul>
		<ul>
			<li><a href="#header-1-1-2">SKY_L2 - Design Preparation Step</a></li>
		</ul>
		<ul>
			<li><a href="#header-1-1-3">SKY_L3 - Review files after design prep and run synthesis</a></li>
		</ul>
		<ul>
			<li><a href="#header-1-1-4">SKY_L4 - OpenLANE Project Git Link Description</a></li>
		</ul>
		<ul>
			<li><a href="#header-1-1-5">SKY_L5 - Steps to characterize synthesis results</a></li>
		</ul>
		</ul>
 </div>



<div class="toc">
	<ul>
    		<li><a href="#header-2">Sky130 Day 2 - Good Floorplan vs Bad Floorplan and Introduction to library cells</a></li>
		<ul>
        		<li><a href="#header-2-1">SKY130_D2_SK1 - Chip Floor planning considerations</a></li>
 		<ul>
			<li><a href="#header-2-1-1">SKY_L1 - Utilization factor and aspect ratio</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-1-2">SKY_L2 - Concept of pre-placed cells</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-1-3">SKY_L3 - De-coupling capacitors</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-1-4">SKY_L4 - Power planning</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-1-5">SKY_L5 - Pin placement and logical cell placement blockage</a></li>
		</ul>
			<ul>
			<li><a href="#header-2-1-6">SKY_L6 - Steps to run floorplan using OpenLANE</a></li>
		</ul>
			<ul>
			<li><a href="#header-2-1-7">SKY_L7 - Review floorplan files and steps to view floorplan</a></li>
		</ul>
			<ul>
			<li><a href="#header-2-1-8">SKY_L8 - Review floorplan layout in Magic</a></li>
		</ul>  
  </ul>

<ul>
        		<li><a href="#header-2-2">SKY130_D2_SK2 - Library Binding and Placement</a></li>
 		<ul>
			<li><a href="#header-2-2-1">SKY_L1 - Netlist binding and initial place design</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-2-2">SKY_L2 - Optimize placement using estimated wire-length and capacitance</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-2-3">SKY_L3 - Final placement optimization</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-2-4">SKY_L4 - Need for libraries and characterization</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-2-5">SKY_L5 - Congestion aware placement using RePlAce</a></li>
		</ul>	
  	
</ul>

<ul>
        		<li><a href="#header-2-3">SKY130_D2_SK3 - Cell design and characterization flows</a></li>
 		<ul>
			<li><a href="#header-2-3-1">SKY_L1 - Inputs for cell design flow</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-3-2">SKY_L2 - Circuit design step</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-3-3">SKY_L3 - Layout design step</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-3-4">SKY_L4 - Typical characterization flow</a></li>
		</ul>			
</ul>

<ul>
        		<li><a href="#header-2-4">SKY130_D2_SK4 - General timing characterization parameters</a></li>
 		<ul>
			<li><a href="#header-2-4-1">SKY_L1 - Timing threshold definitions</a></li>
		</ul>
		<ul>
			<li><a href="#header-2-4-2">SKY_L2 - Propagation delay and transition time</a></li>
		</ul>
  </ul>
 </div> 
 





<div class="toc">
	<ul>
    		<li><a href="#header-3">Sky130 Day 3 - Design library cell using Magic Layout and ngspice characterization</a></li>
		<ul>
        		<li><a href="#header-3-1">SKY130_D3_SK1 - Labs for CMOS inverter ngspice simulations</a></li>
 		<ul>
			<li><a href="#header-3-1-1">SKY_L0 - IO placer revision</a></li>
		</ul>
			<ul>
			<li><a href="#header-3-1-2">SKY_L1 - SPICE deck creation for CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-1-3">SKY_L2 - SPICE simulation lab for CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-1-4">SKY_L3 - Switching Threshold Vm</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-1-5">SKY_L4 - Static and dynamic simulation of CMOS inverter</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-1-6">SKY_L5 - Lab steps to git clone vsdstdcelldesign</a></li>
		</ul>
  </ul>

<ul>
        		<li><a href="#header-3-2">SKY130_D3_SK2 - Inception of Layout ÃÂ CMOS fabrication process</a></li>
 		<ul>
			<li><a href="#header-3-2-1">SKY_L1 - Create Active regions</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-2-2">SKY_L2 - Formation of N-well and P-well</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-2-3">SKY_L3 - Formation of gate terminal</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-2-4">SKY_L4 - Lightly doped drain (LDD) formation</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-2-5">SKY_L5 - Source and drain formation</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-2-6">SKY_L6 - Local interconnect formation</a></li>
		</ul>
	         <ul>
			<li><a href="#header-3-2-7">SKY_L7 - Higher level metal formation</a></li>
		</ul>
  	         <ul>
			<li><a href="#header-3-2-8">SKY_L8 - Lab introduction to Sky130 basic layers layout and LEF using inverter</a></li>
		</ul>
	         <ul>
			<li><a href="#header-3-2-9">SKY_L9 - Lab steps to create std cell layout and extract spice netlist</a></li>
		</ul>
</ul>


<ul>
        		<li><a href="#header-3-3">SKY130_D3_SK3 - Sky130 Tech File Labs</a></li>
 		<ul>
			<li><a href="#header-3-3-1">SKY_L1 - Lab steps to create final SPICE deck using Sky130 tech</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-3-2">SKY_L2 - Lab steps to characterize inverter using sky130 model files</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-3-3">SKY_L3 - Lab introduction to Magic tool options and DRC rules</a></li>
		</ul>
		<ul>
			<li><a href="#header-3-3-4">SKY_L4 - Lab introduction to Sky130 pdk's and steps to download labs</a></li>
		</ul>
  <ul>
			<li><a href="#header-3-3-5">SKY_L5 - Lab introduction to Magic and steps to load Sky130 tech-rules</a></li>
		</ul>
  <ul>
			<li><a href="#header-3-3-6">SKY_L6 - Lab exercise to fix poly.9 error in Sky130 tech-file</a></li>
		</ul>
  <ul>
			<li><a href="#header-3-3-7">SKY_L7 - Lab exercise to implement poly resistor spacing to diff and tap</a></li>
		</ul>
			 <ul>
			<li><a href="#header-3-3-8">SKY_L8 - Lab challenge exercise to describe DRC error as geometrical construct</a></li>
		</ul>
	 <ul>
			<li><a href="#header-3-3-9">SKY_L9 - Lab challenge to find missing or incorrect rules and fix them</a></li>
		</ul>
</ul>				
 </div> 





<div class="toc">
	<ul>
    		<li><a href="#header-4">Sky130 Day 4 - Pre-layout timing analysis and importance of good clock tree</a></li>
		<ul>
        		<li><a href="#header-4-1">SKY130_D4_SK1 - Timing modelling using delay tables</a></li>
 		<ul>
			<li><a href="#header-4-1-1">SKY_L1 - Lab steps to convert grid info to track info</a></li>
		</ul>
			<ul>
			<li><a href="#header-4-1-2">SKY_L2 - Lab steps to convert magic layout to std cell LEF</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-1-3">SKY_L3 - Introduction to timing libs and steps to include new cell in synthesis</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-1-4">SKY_L4 - Introduction to delay tables</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-1-5">SKY_L5 - Delay table usage Part 1</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-1-6">SKY_L6 - Delay table usage Part 2</a></li>
		</ul>
			<ul>
			<li><a href="#header-4-1-7">SKY_L7 - Lab steps to configure synthesis settings to fix slack and include vsdinv</a></li>
		</ul>
  </ul>

<ul>
        		<li><a href="#header-4-2">SKY130_D4_SK2 - Timing analysis with ideal clocks using openSTA</a></li>
 		<ul>
			<li><a href="#header-4-2-1">SKY_L1 - Setup timing analysis and introduction to flip-flop setup time</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-2-2">SKY_L2 - Introduction to clock jitter and uncertainty</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-2-3">SKY_L3 - Lab steps to configure OpenSTA for post-synth timing analysis</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-2-4">SKY_L4 - Lab steps to optimize synthesis to reduce setup violations</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-2-5">SKY_L5 - Lab steps to do basic timing ECO</a></li>
		</ul>
</ul>


<ul>
        		<li><a href="#header-4-3">SKY130_D4_SK3 - Clock tree synthesis TritonCTS and signal integrity</a></li>
 		<ul>
			<li><a href="#header-4-3-1">SKY_L1 - Clock tree routing and buffering using H-Tree algorithm</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-3-2">SKY_L2 - Crosstalk and clock net shielding</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-3-3">SKY_L3 - Lab steps to run CTS using TritonCTS</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-3-4">SKY_L4 - Lab steps to verify CTS runs</a></li>
		</ul>
</ul>	

<ul>
        		<li><a href="#header-4-4">SKY130_D4_SK4 - Timing analysis with real clocks using openSTA</a></li>
 		<ul>
			<li><a href="#header-4-4-1">SKY_L1 - Setup timing analysis using real clocks</a></li>
		</ul>
		<ul>
			<li><a href="#header-4-4-2">SKY_L2 - Hold timing analysis using real clocks</a></li>
		</ul>
	<ul>
			<li><a href="#header-4-4-3">SKY_L3 - Lab steps to analyze timing with real clocks using OpenSTA</a></li>
		</ul>
	<ul>
			<li><a href="#header-4-4-4">SKY_L4 - Lab steps to execute OpenSTA with right timing libraries and CTS assignment</a></li>
		</ul>
	<ul>
			<li><a href="#header-4-4-5">SKY_L5 - Lab steps to observe impact of bigger CTS buffers on setup and hold timing</a></li>
		</ul>
	</ul>	
 </div> 










 








# <h1 id="header-1">Sky130 Day 1 - Inception of open-source EDA, OpenLANE and Sky130 PDK</h1>
## <h1 id="header-1-1">Sky130_D1_SK3  - Get familiar to open-sorce EDA tools</h1>
## <h1 id="header-1-1-1">SKY_L1 - OpenLANE Directory Structure in detail</h1>

**Notes**

pdks:  contains all pdk information. pdk used for this workshop is skywater-130nm. OpenLANE is built around this pdk. 

![image](https://github.com/user-attachments/assets/d09a9b84-881c-4b0c-9962-b5955112f8bf)

skywater-pdk contains all the pdk related files, that is, timing related files, lef files, tech lef, cell lef and so on.

![image](https://github.com/user-attachments/assets/5b16b931-b9ae-4ff5-a1a8-dd0573cab1dd)

libs.ref contains the timing related files, lef files, tech lef, cell lef and so on.
libs.tech are those files specific to the tool

![image](https://github.com/user-attachments/assets/50f9e3c2-24de-449f-a727-ddc8200797f2)

![image](https://github.com/user-attachments/assets/2b9fad37-68cd-4404-8d60-c6c47184274f)

Directory used to invoke the tool

## <h1 id="header-1-1-2">SKY_L2 - Design Preparation Step</h1>
**Notes**

![image](https://github.com/user-attachments/assets/bfb277ff-e167-496b-93a9-20e27a434e1e)

![image](https://github.com/user-attachments/assets/d4709367-92fb-439f-80f2-59f49afdea3c)

src: souce, where verilog file for RTL is present 
config.tcl: bypasses any configuration that is already done into a plane. Many of the switches uses the deafault value. For example, clock period is set, verilog files are picked from a specific path and so on.

![image](https://github.com/user-attachments/assets/4eca0e18-e141-4c78-95a5-de6d297bfc7f)

![image](https://github.com/user-attachments/assets/c958d0d1-1a9b-4ed0-a486-4811cf41b766)

![image](https://github.com/user-attachments/assets/b3f6025e-d0a2-473b-ab32-2e087af8664a)

sky130A_sky130_fd_sc_hd_config.tcl overrides the default value in config.tcl
The clock period in config.tcl was 5ns and was overriden by sky130A_sky130_fd_sc_hd_config.tcl to 24.73ns

![image](https://github.com/user-attachments/assets/23038855-6913-495f-b37a-ee0fdcd809da)

Design preparation is completed.

![image](https://github.com/user-attachments/assets/6a137249-30fa-4486-aaab-55ec415d94d7)

And the run folder is created under design folder. 

## <h1 id="header-1-1-3">SKY_L3 - Review files after design prep and run synthesis</h1>
**Notes**

![image](https://github.com/user-attachments/assets/e45675be-97da-4e37-812f-a8ddfd9d9484)

![image](https://github.com/user-attachments/assets/74cbbb2f-20cd-4b63-af00-562f888480f6)

![image](https://github.com/user-attachments/assets/9d40afa0-a6f6-4534-b8aa-f8f218a3c2e2)

Tech Lef information is available. Metal layer related, that is wire information and cell level related information is available. 

![image](https://github.com/user-attachments/assets/d9041b49-f66e-4ea0-8037-b07678fa6a12)

Various files under Results, Reports, Logs..

Apart from config.tcl which is avaialbale under Designs folder and Runs folder, the config.tcl available under 08-08_09-20 basically shows which all default parameters are being taken by the run.

![image](https://github.com/user-attachments/assets/6396da72-8b85-481c-ae86-5f0e027962f0)

![image](https://github.com/user-attachments/assets/252dca00-e378-4c70-b5b8-6e2cd1371f83)

Use the run_synthesis command to run the Synthesis flow 

## <h1 id="header-1-1-4">SKY_L4 - OpenLANE Project Git Link Description</h1>
**Notes**

https://github.com/efabless/openlane

The OpenLane Flow 
![image](https://github.com/user-attachments/assets/b2f278bc-e560-4f98-9290-25f56680219f)

Going through OpenLane Documentation

https://openlane.readthedocs.io/en/latest/reference/interactive_mode.html

![image](https://github.com/user-attachments/assets/bc0b943e-86e7-4cdf-916b-a9f1b9c62def)

Links for Fossi Dial Up:

https://www.youtube.com/live/9Lw83kFtnc4?si=w8iuuy94h0yD7bzc

https://www.youtube.com/live/EczW2IWdnOM?si=o09PSbgX_HbZi59s

## <h1 id="header-1-1-5">SKY_L5 - Steps to characterize synthesis results</h1>
**Notes**

Task 1: To find flop ratio, that is number of D-FlipFlops or total no. of cells

![image](https://github.com/user-attachments/assets/6aa7420e-fd9a-4348-b2cb-be7f1cbb1e83)

No. of cells = 14876

No. of D-FFs = 1613

Clock count = No. of D-FFs/No. of cells = 1613/14876 = 0.1084

Percentage = 10.84%

After the syntehsis is complete:
1. Results folder:![image](https://github.com/user-attachments/assets/d3904ce9-ac66-4798-9c5e-804d4e7090a9)

Opened the following:

a. picorv32a.synthesis.v (contains synthesised netlist and the abc has completed all the mappings)

![image](https://github.com/user-attachments/assets/76098864-122a-4f2d-ad8b-7e7e091db9a4)

2. Report folder: ![image](https://github.com/user-attachments/assets/469fe773-0b83-46b8-aab6-02c6eb07ed11)

Opened the following: 

a. less 1-yosys_2.stat.rpt:
![image](https://github.com/user-attachments/assets/a891457a-72ad-405a-a04f-75408d5c0ccb)

b. less opensta_main.timing.rpt:
![image](https://github.com/user-attachments/assets/7fe9c7a9-fb0a-4782-903b-9792eeeff9d1)

# <h1 id="header-2">Sky130 Day 2 - Good Floorplan vs Bad Floorplan and Introduction to library cells</h1>
## <h1 id="header-2-1">Sky130_D2_SK1 - Chip Floor planning considerations</h1>
### <h1 id="header-2-1-1">SKY_L1 - Utilization factor and aspect ratio</h1>
**Notes**

1. Define width and height of Core and Die:

a. Consider a netlist and convert the gates and flip-flops into physical dimensions (square/rectangular box).

![image](https://github.com/user-attachments/assets/ef921f9f-21e1-4b5e-b8b0-f4b8ab806e99)

b. Ignore all the wires for now and assume the following dimensions for a standard cell and flip flops: 

![image](https://github.com/user-attachments/assets/e79cf04e-c59a-4bde-9c96-df8ec8e0a57f)

Place all the gates and flipflops in a single plate by combining all of them into one physical dimension and calculate the area occupied by the netlist on a Silicon Wafer. Minimum area occupied by the netlist is as shown below:

![image](https://github.com/user-attachments/assets/8a477cc8-5cc3-405f-840d-baafc666ca2d)

c. Silicon Wafer contains a lot of Dies inside it and inside each Die there is a Core region. A Core is the section of the chip where the fundamental logic of the design is placed. A Die, encapsulates the core. These dies are imprinted multiple times in the silicon wafer to increase its throughput.

![image](https://github.com/user-attachments/assets/cbfa757f-3bca-4073-ba1e-c099510bc8a2)

f. Place all the logical cells (from b) inside the core and calculate the utilization factor. If logical cells occupy the complete area of the core, the utilization factor would be 1 which is not the practical scenario.

Utilization factor = (Area occupied by Netlist/ Total area of the Core)

Aspect ratio = (Height of Core)/(Width of Core)

If the aspect ratio is 1, it signifies that the chip is square-shaped else rectangle. For the following example the Utilization factor and Aspect ratio are both 1: 

![image](https://github.com/user-attachments/assets/f3a4e65e-1562-4394-87b0-0db1ae9f5390)

Some more examples:

![image](https://github.com/user-attachments/assets/ae046f7d-14f7-44c9-993a-31f74a6dc664)

![image](https://github.com/user-attachments/assets/85132317-efe0-488c-a157-3ca81fbe8e4e)

### <h1 id="header-2-1-2">SKY_L2 - Concept of pre-placed cells</h1>
**Notes**

2. Define locations of Preplaced cells:

a. Preplaced cells are the black boxes having some specific functionality that is implemented once separately and then can be instantiated multiple times.

![image](https://github.com/user-attachments/assets/b4c34c06-0c1c-484a-a4a2-52878a2d3e24)

b. Preplaced cells are macros or IPs like memory, clock-gating cell, comparator, mux.

![image](https://github.com/user-attachments/assets/3f38493d-cdb0-4fbc-a465-a45f8165150e)

c. The arrangement of these IPs in a chip is referred as floorplanning. These IPs/blocks have user-defined locations, and hence are placed in the chip before automated placement-and-routing, and are called as preplaced cells. Automated placement and routing tools place the remaining logical cells in the design onto the chip. Place the preplaced cells on the basis of design scenario or design background.

### <h1 id="header-2-1-3">SKY_L3 - De-coupling capacitors</h1>
**Notes**

3. Place the pre-placed cells closer to the input area and surround the preplaced cells with decoupling capacitors.

a. Decoupling capacitors are the huge capacitors that are completely filled with charge. Voltage across the decoupling capacitor is equivalent to the supply voltage. If power supply is 1V, decap will be charged till 1V. Decoupling capacitor is placed very near and parallel to the circuit. Everytime the circuit switches, it draws current from decap, whereas the RL network is used to replenish the charge into decap. As the name suggests, decoupling capacitor decouples the circuit from the main supply. With the help of decap local communication is taken care.

![image](https://github.com/user-attachments/assets/aa3209ca-8313-4674-9042-2604e5ebe5f6)

### <h1 id="header-2-1-4">SKY_L4 - Powerplanning</h1>
**Notes**

4. Powerplanning

Possibilities of ground bounce and voltage droop issues due to usage of a single power supply is solved by powerplanning. 

![image](https://github.com/user-attachments/assets/ec7ce61c-a748-4a66-a85e-01c409e071d3)

![image](https://github.com/user-attachments/assets/fab8c983-d395-4ec2-8485-0f5933bd25d7)

![image](https://github.com/user-attachments/assets/32e0aa7a-b643-4da5-9851-37af465d58b5)

![image](https://github.com/user-attachments/assets/4937e2f5-904c-46f9-9b73-4a0521c26ab8)

Mltiple power supply through mesh structure for VDD and VSS.

![image](https://github.com/user-attachments/assets/b36d615d-88f5-4663-9ebf-5ca0986eb9cb) 

### <h1 id="header-2-1-5">SKY_L5 - Pin Placement and logical cell placement blockage.</h1>
**Notes**

5. Pin Placement and logical cell placement blockage.

Pin Placement

   ![image](https://github.com/user-attachments/assets/9601af54-467f-4b2f-8648-74cb34438fe7)

   ![image](https://github.com/user-attachments/assets/3eccb2e6-4849-4765-b612-f11411ef080f)

Clock ports are bigger than the data ports because clock drives all seq cells continuosly, basically they drives all the flops in the full chip. So, we need the least resistance path for the clocks. 

Logical cell placement blockage

![image](https://github.com/user-attachments/assets/72424990-49c7-4642-be51-aebd47c9463a)

We block the area between core and die to avoid placement of any logical cells in those areas by automated placement and routing tools because that area is reserve for the pin locations.

### <h1 id="header-2-1-6">SKY_L6 - Steps to run floorplan using OpenLANE</h1>

Standard cell placement takes place during Placement stage and not during Floorplanning. 

By executing `less README.md`, here we can see global variable, syntesis, floorplanning, placement, CTS, Routing and so on.

![image](https://github.com/user-attachments/assets/01e7b31e-b527-4bff-8385-38b004888735)

![image](https://github.com/user-attachments/assets/291cdf5a-1bb4-44fd-a994-6fba47fd87f3)

The variables like FP_CORE_UTIL and so on are called the switches. These switches are set under the .tcl files present under confirguration folders, that is, default value.

![image](https://github.com/user-attachments/assets/e4ba39ba-c276-4217-9937-7d1941365da2)

Precendence for the .tcl files containing the default values are:

1. ![image](https://github.com/user-attachments/assets/ad0b68cd-1d9b-4f74-ac34-e110cb03adad)

2. ![image](https://github.com/user-attachments/assets/90dc5110-9677-457b-bfde-f771c780e9cd)

   `FP_CORE_UTIL = 65`, `FP_IO_VMETAL = 4`, `FP_IO_HMETAL = 3`

4. ![image](https://github.com/user-attachments/assets/ed0d5bb3-ea49-4a3a-b141-74a50c9217e1)

    `FP_CORE_UTIL = 50`, `FP_IO_VMETAL = 2`, `FP_IO_HMETAL = 3`

   Using `run_floorplan`

   ![image](https://github.com/user-attachments/assets/b83f88de-2542-40fa-bb92-6d33731cc10a)

### <h1 id="header-2-1-7">SKY_L7 - Review floorplan files and steps to view floorplan</h1>

![image](https://github.com/user-attachments/assets/c4e3b3cf-b271-4ac8-8716-c88c93f5d3a1)

Opening def file: 

![image](https://github.com/user-attachments/assets/2e2638cc-e5b7-491e-aaa4-90a84f93dd04)

Viewing the floorplan in magic:

![image](https://github.com/user-attachments/assets/4037ffe9-c81b-4ef0-b693-1fbc9459f63d)

![image](https://github.com/user-attachments/assets/e1575759-f690-4709-bbac-8eff7d17a305)

### <h1 id="header-2-1-8">SKY_L8 - Review floorplan layout in Magic</h1>

Viewing layout after the floorplan using magic tool:

To open the layout:

![image](https://github.com/user-attachments/assets/e5d5a059-1b34-4439-b041-fb9dc9e1c010)

![image](https://github.com/user-attachments/assets/d268292e-0c96-4208-9b64-e9404c8f2afa)

![image](https://github.com/user-attachments/assets/8ff5e68a-bda2-45cc-bd3a-6d05894c2499)

![image](https://github.com/user-attachments/assets/25d392ec-d2ef-4ef3-9a2a-836446cbbb6b)

Floorplan does place the standard cells. They are present in the lower left corner of the layout:

![image](https://github.com/user-attachments/assets/504478bd-c95c-4d7a-98d9-cf7e0ba52a1b)

## <h1 id="header-2-2"> SKY130_D2_SK2 - Library Binding and Placement</h1>
### <h1 id="header-2-2-1">SKY_L1 - Netlist binding and initial place design</h1>

1. Bind netlist with physical cells:

The netlist contains different gates and the shape of each gate defines its functionality. Example: By the shape of OR gate we understand that it will perform OR operation. But in reality, we don't have such shapes for different gates, we just have a box structure for each gate that has some width and height (physical dimension).

![image](https://github.com/user-attachments/assets/396f129f-e41f-4d17-a86f-64c02c17249d)

![image](https://github.com/user-attachments/assets/e43fe760-c054-48b8-bc8e-3fad243b94f6)

![image](https://github.com/user-attachments/assets/5379a1ee-a77a-4b95-8a32-0c81cddad7a5)


2. Placement:

After having proper shapes and sizes to each gate, these shapes and sizes are placed onto the floorplan. Now we have the floorplan, netlist, and physical view of the logic gates.

![image](https://github.com/user-attachments/assets/b52f4d9b-2ae9-4149-8585-6713df6a1606)

### <h1 id="header-2-2-2">SKY_L2 - Optimize placement using estimated wire-length and capacitance</h1>

continuing placement of cells

![image](https://github.com/user-attachments/assets/53cf4cc9-740a-4e28-b6f0-3013d47187d6)

3. Optimize Placement:

Optimised placement: This is the stage where wire length and capacitance are estimated. And based on that insert repeaters (To maintain signal intergrity, we would need something in the intermediate steps to reproduce what the input ports are saying. And hence we require repeaster. Repeaters are buffers that re-conditions your original signal, make a new signal which replicates the original signal and sends them forward). 

More the repeaters, more the loss of areas. 

![image](https://github.com/user-attachments/assets/152e1778-31a3-4c1c-aba8-4fe8c7e33633)

Slew is dependend on the value of the capacitor, the higher the value of the capacitor: the amount of charge required to charge the capacitor will be high and the slew will be even bad.

![image](https://github.com/user-attachments/assets/8656cfc6-5459-486b-a5ee-e51de727513b)

Repeaters are added for the belwo instance:

![image](https://github.com/user-attachments/assets/7566682c-8134-40cd-82de-07d60ea1d054)

![image](https://github.com/user-attachments/assets/942091ca-edcb-4dfc-a9b8-a66f06e7c2da)

### <h1 id="header-2-2-3">SKY_L3 - Final placement optimization</h1>

![image](https://github.com/user-attachments/assets/06d7a0be-3694-4b57-8ae3-7e0fc4c1cba5)

The elements FF1, 1 ,2 and FF2 logics are abutted, that is, there is no time delay between signal passed from FF1 to FF2. There are multiple reasons to do abutment, let's say this particular section of the circuit works at a very high speed and zero time delay is required, and don't want to waste delays on wires, and therefore, the abutment is done for those logics. This is a classic example of high frequency ckt usages.

![image](https://github.com/user-attachments/assets/1c97a956-7490-4507-a2eb-1127e191b80a)

![image](https://github.com/user-attachments/assets/3aceb05d-286e-4676-ac5f-45e3760d421e)

### <h1 id="header-2-2-4">SKY_L4 - Need for libraries and characterization</h1>

SetUp Timing Analysis

Since the clocks have not built, we need to check the data path considering there are no clocks or the clocks are ideal. Ideal clock means that the time required for a clock to reach any of the flip flops is zero.

**Need for characterisation**

**Part 1 - Concepts and theory - NLDM, CCS timing, power and noise chcarcterization**

**Step 1: Logic Synthesis:** Typical IC design flow that every design needs to go through if it wants to be implemented onto a chip. So, the first step to do that is logic synthesis. If we have a functionality that is coded in the form of RTL, the first step is to convert the functionality into legal hardware is referred to as logic synthesis. So, the output of logic synthesis is an arrangement of gates that will represent your original functionality that you have described using an RTL. This is the first step of an IC design flow.

![image](https://github.com/user-attachments/assets/aff81504-6d1c-4901-99ba-1aa76d85289e)

**Step 2: Floorplanning:** In this step, we import the output of logic synthesis or the netlist that we get out of the logic synthesis and decide the size of the core and die. So the size of the core and die is completely dependent on the amount of gates and the shapes and sizes of the gates present in the output of the logic synthesis step.

![image](https://github.com/user-attachments/assets/e605fa0b-31b7-4f71-a152-78f6dae44e7b)

**Step 3: Placement:** After floorplanning, the placement stage is there, and then CTS (Clock Tree Synthesis). And then finally we have the routing stage.

![image](https://github.com/user-attachments/assets/2125c691-a4b1-459d-9e0a-b4bc906efb83)

**Step 4: CTS:** CTS is nothing but to have zero skew or clock being spread across logic cells at an equal time.   

![image](https://github.com/user-attachments/assets/419bc88d-3262-42da-a0fe-9a3ddb1334ef)

**Step 5: Routing:** 

Below is an example of maze routing: 

![image](https://github.com/user-attachments/assets/e0167b41-0a50-4005-89d5-aaf3fe2d0a31)

![image](https://github.com/user-attachments/assets/2eaaa05f-fc1f-4385-bc72-a1a4b41afe3f)

Library characterization is very important and this collection of gates if you place it in some area, that area is referred to as Library.

 ### <h1 id="header-2-2-5">SKY_L5 - Congestion aware and placement and RePlAce <h1>

After routing, it is placement stage.

Placement in Openlane occurs in 2 stages: 

a. Global placement 
b. Detail placement.

There are different tools to do both of these functionality.

**Global placement**: coarse placement, no legalization happening

What is legalization? --> The standard cells are placed in standard cell rows, they should be exactly inside the row abutted with each other. And there should be no overlaps. Legalization is more required from a timing point of view.

**Detail placement**: legalization happens here

When we do run_placement, first global placement happens. Global placement, the main objective is **reducing the wire length**. In Openlane, we use the concept of HPWL means **half-perimeter wire length**. Reduction of HPWL is the main focus and converging the overflow (OVFL) means a decrease in the OVFL value means the placement is going right.

So, previously I had done till floorplan, for running the placement from the previous day's floorplan in Openlane, no need to run synthesis and floorplan again.

Just do the following steps:

a. package require openlane 0.9

b. prep - design picorv32A 

c. run_synthesis

d. run_floorplan

e. run_placement

![image](https://github.com/user-attachments/assets/5ac30851-b8a5-40e5-b8d9-4797936cab53)

In placement stage, the standard cells are fixed.

![image](https://github.com/user-attachments/assets/d3c5eb3e-c77e-4df1-8dcb-a78542dc2614)

![image](https://github.com/user-attachments/assets/9601543f-849d-44a3-bbba-b12570394b0d)

Note: Power Distribution Network gets created during floorplan but in Openlane flow right now, the order is different. The floorplan does not create the Power Distribution Network. Here, in Openlane flow, PDN is done post floorplan, placement, and CTS.

## <h1 id="header-2-3">SKY130_D2_SK3 - Cell design and characterization flows </h1>
### <h1 id="header-2-3-1">SKY_L1 - Inputs for cell design flow </h1>

We have a placed and routed design here. Standard cells are placed in a section called Library. Library is a place where you keep all your standard cells, macros, IPs, decaps, etc.

![image](https://github.com/user-attachments/assets/c340f1db-f6c3-4b22-9322-896182c2b871)

Library has got cells with different functionalities, different sizes, and different threshold voltages (Vt).

![image](https://github.com/user-attachments/assets/3696bd0e-4e61-45b4-ab16-f21d79318dfb)

The next step is to take one of the inverters and understand its cell design flow. This inverter has to be represented in the form of its shape, in the form of its timing behavior, in the form of its drive strength, and in the form of its power characteristics, and so on. A small inverter has to go through a typical cell design flow.

Cell design flow is divided into 3 parts:


![image](https://github.com/user-attachments/assets/23bd2e3b-e5e6-41b4-a983-1cdfafe2c9ec)

1. **Inputs**: inputs to design your inverter, Process design kits (pdks) provided by the foundry.

a. **DRC & LVS rules**: tech file --> has 5he rules like poly width, extension over active, etc.

![image](https://github.com/user-attachments/assets/50d23017-d71f-4367-a2c3-83d720624ef4)

![image](https://github.com/user-attachments/assets/566582a9-c73d-4648-841d-39442554940d)

b. **SPICE models**

![image](https://github.com/user-attachments/assets/8d83b632-b9ee-4914-a2ad-3f8fef2e30d7)

### <h1 id="header-2-3-2">SKY_L2 - Circuit design step </h1>

c. **Library & user-defined specs**: Cell-height, supply voltage, metal layers, pin location, drawn gate length, etc

![image](https://github.com/user-attachments/assets/0581ea5a-3d0f-4e79-9bac-bff786b8379a)

![image](https://github.com/user-attachments/assets/45bfb442-fb9b-42df-8bfe-2a296965da09)

2. **Design Steps**
a. **Circuit design**: implement the function and model nmos and pmos to meet the library requirement, will get the information about W/L of the nmos and pmos in this step. Once we know the value of W/L for the transistors, next step is to implement these values in the layout called as layout design. Output of the Circuit design step is CDL (circuit description language)

![image](https://github.com/user-attachments/assets/f7007bfc-6dea-4fbd-8752-1bc596e79563)

b. **Layout design**: First step is to get the function implemented through the mos transistors. The next step is to get the pmos network graph and nmos network graph. Output of the layout design - GDSII, LEF, extracted spice netlist/ckt

![image](https://github.com/user-attachments/assets/a0c01820-7763-4e04-a98d-ae8b6cc18689)

### <h1 id="header-2-3-3">SKY_L3 - Layout design step </h1>

Next step is to obtain the Euler's path.

![image](https://github.com/user-attachments/assets/52bcc0fc-2adf-4764-b872-83bdab8f8aca)

Once you obtain a Euler's path, draw a stick diagram out of it.

![image](https://github.com/user-attachments/assets/9f575b1c-255f-451a-a593-59b6b08419c2)

Next step is to convert this stick diagram into a proper/typical layout according to the rules from the inputs.

![image](https://github.com/user-attachments/assets/f45e50d2-e4c9-4836-bf67-651dc131c038)

Next step is to extract the parasitics and characterize them in terms of timing.

![image](https://github.com/user-attachments/assets/0715a97c-1dcc-4f42-8a83-3bd212bc36e4)

### <h1 id="header-2-3-4"> SKY_L4 - Typical characterization flow </h1>

c. **Characterization**

![image](https://github.com/user-attachments/assets/3651383b-bf29-4cb6-b9a4-7b35f6a9c856)

So, what we have till this step: layout of buffer, description of buffer, extracted spice netlist, subckts, nmos pmos spice models, etc.

![image](https://github.com/user-attachments/assets/bf4e1e93-6627-49c6-8ca1-88c14b9d4927)

![image](https://github.com/user-attachments/assets/a1fdd922-3223-4e95-8ebd-b92f0d5615d0)

![image](https://github.com/user-attachments/assets/063f3288-d914-42e7-bbf5-a77a0c7f4aa7)

![image](https://github.com/user-attachments/assets/c472f485-b0e1-4c69-8cc1-4f4f62b75f68)

3. **Outputs**
these are actually used by the EDA tools.
 
## <h1 id="header-2-4">SKY130_D2_SK4 - General timing characterization parameters  </h1>
### <h1 id="header-2-4-1">SKY_L1 - Timing threshold definitions</h1>

1. **Timing Characterisation**

![image](https://github.com/user-attachments/assets/042148f9-064b-458e-b439-b75408970577)

a. **Timing Threshold definitions**

![image](https://github.com/user-attachments/assets/f1e82acb-129e-4fa2-abff-f8475c819134)

b. **Slew low rise threshold - 20%** and **Slew high rise threshold - 20%**

![image](https://github.com/user-attachments/assets/afc89abe-9b2f-46dc-bbe1-2b3853bae394)

![image](https://github.com/user-attachments/assets/83a7ccd1-352d-484e-b1d9-131691a135b2)

c. **Slew low fall threshold - 20%** and **Slew high fall threshold - 20%**

![image](https://github.com/user-attachments/assets/3deaeb2b-d366-4e0e-a554-800a47008442)

![image](https://github.com/user-attachments/assets/f11ea15b-5d12-4801-8347-79a06b7deaf0)

d. **in rise threshold - 50%:** and **out rise threshold - 50%:** 

![image](https://github.com/user-attachments/assets/6ec481fb-4cac-4698-a1ab-bb140a9f3c86)

![image](https://github.com/user-attachments/assets/af867bf6-c56d-4f81-8130-46290a5392af)

e. **in fall threshold - 50%:** and **out fall threshold - 50%:** 

![image](https://github.com/user-attachments/assets/c2ffdc88-f157-4854-b71a-37ac997ec820)

![image](https://github.com/user-attachments/assets/0cc350f7-7df0-4a81-9ed8-3ab1ea0a3c68)

### <h1 id="header-2-4-2">SKY_L2 - Propagation delay and transition time</h1>

f. **Propagation delay:**

![image](https://github.com/user-attachments/assets/7e58eaa8-7a27-4741-82eb-636ad3cecfbf)

g. **Transition time:**

![image](https://github.com/user-attachments/assets/a5559602-9d2a-4092-b2a7-9a39bd7896f4)

![image](https://github.com/user-attachments/assets/a8f376a4-859d-466c-b2bb-9984fd455232)

![image](https://github.com/user-attachments/assets/fad295e6-5ebb-4e0e-b9f9-93788d288f1d)

g. **Output current waveform and Output voltage waveform:**

# <h1 id="header-3"> SKY130 Day3 - Design library cell using Magic Layout and ngspice characterization</h1>
## <h1 id="header-3-1">SKY130_D3_SKY1 - Labs for CMOS inverter ngspice simulations</h1>
### <h1 id="header-3-1-1">SKY_L0 - IO placer revision</h1>

In Openlane, we can do the changes on the fly. If suppose, we have already done the floorplan and observed a lot of congestion, we can change utilization factor even now. In our case, we have placed the IO pins equidistant, now we will be changing it to some other input output pin strategy.

![image](https://github.com/user-attachments/assets/c6ae9fda-4555-44e7-bf01-9e85d29d0dca)

IO placers are open source EDA tool used to place the IO's around the core. 

setting the following variable to 2:

![image](https://github.com/user-attachments/assets/8103d9d7-7b5f-4308-a533-39b700cf930e)

and running floorplan again:

![image](https://github.com/user-attachments/assets/eab28b70-25ed-40ed-bd3f-e7960566fc60)

![image](https://github.com/user-attachments/assets/27dc3909-4d9c-41e1-ac85-ef5f912c95f3)

Again opened the layout in Magic and the def is updated (in the same folder only where previous def was there) and the IO pin placement is changed.

![image](https://github.com/user-attachments/assets/81abcbbb-bc9c-448d-8057-0c0804fd6065)

### <h1 id="header-3-1-2"> SKY_L1 - SPICE deck creation for CMOS inverter</h1>

SPICE simulations: 350nm, 250nm mos are available.

1. Create a SPICE deck for VTC CMOS characteristics: SPICE deck is nothing but a netlist, a connectivity information

a. When we say W/L of mos it means it is the W/L of the channel of mos.

b. In cmos, generally pmos should be wider than the nmos. Ideally, pmos should be twice or thrice of the nmos. But the spice deck we are creating is having nmos and pmos of the same W/L.

![image](https://github.com/user-attachments/assets/291ca74c-c8c1-4c85-824a-b8f17ecccdcd)

Here M1 = pmos, M2 = nmos

![image](https://github.com/user-attachments/assets/cddce7ee-23da-479a-a32a-c7a3de795526)

Syntax of Mosfet in the SPICE: M1 Drain Gate Source Substrate type W L = M1 out in vdd vdd pmos 0.375u 0.25u

### <h1 id="header-3-1-3"> SKY_L2 - SPICE simulation lab for CMOS inverter</h1>

![image](https://github.com/user-attachments/assets/f4b7a7a4-d473-4355-a7e5-4d96d74747c3)

Syntax of Mosfet in the SPICE: M1 Drain Gate Source Substrate type W L = M2 out in 0 0 nmos 0.375u 0.25u

Output load is connected between out and 0:

![image](https://github.com/user-attachments/assets/3d5b8a62-f221-45f0-9b7c-09290b9a6d15)

![image](https://github.com/user-attachments/assets/cf2147ca-dda9-4f86-b968-b28a2d49c31d)

![image](https://github.com/user-attachments/assets/280fa3f8-4fdc-4e76-a7aa-dbfb53b62cdd)

![image](https://github.com/user-attachments/assets/8a02688b-a0d5-4c50-bc66-acc778d17409)

2. SPICE simulation in ngspice:

![image](https://github.com/user-attachments/assets/d213ad6b-fbfc-47b0-8071-f118ca847294)

Wn, Wp --> nmos and pmos channel width

Ln, Lp --> nmos and pmos channel length

Wn/Ln = Wp/Lp = 1.5

![image](https://github.com/user-attachments/assets/4241a5b8-88d2-404b-822a-0d900425ff8e)

The above VTC is shifted towards the left from the centre. 

3. Now, upon increasing the pmos width to 0.9375 (2.5 times of nmos channel width) = pmos is bigger than nmos here

Wn/Ln = 1.5, Wp/Lp = 3.75

![image](https://github.com/user-attachments/assets/ef99bd3d-4389-4201-ba1f-0e58927019fe)

Now the VTC is at the centre.

### <h1 id="header-3-1-4">SKY_L3 - Switching Thershold Vm</h1>

4. Analysis of the 2 VTCs obtained in previous 2 points (2 & 3).

![image](https://github.com/user-attachments/assets/2b1258f1-4a4a-4084-ad74-5a735f52465b)

Shape of both the waveforms are similar, that means CMOS is a robust device, when input is low, ouput is high and vice-versa and this is for kinds of CMOS. Therefore, Cmos logic is even and widely used for any of the logic gate designing. 

What defines the robustness of the CMOS?

a. Switching threshold, Vm: It is a point where Vin=Vout

![image](https://github.com/user-attachments/assets/d7d1bb95-a58c-4e49-bf5a-520a45ebcc72)

This brings us to many conclusion here:

i. This area is very critical area for CMOS inverter bcoz input=output.

![image](https://github.com/user-attachments/assets/0969252a-8847-4258-9874-0d97f9501d78)

ii. Both pmos and nmos are in saturation region in this area means both are kind of turned on that implies very high chance of leakage current. Direct current flow from power to ground means short ckt current.

![image](https://github.com/user-attachments/assets/37fd3d3e-4952-4982-a871-3fd8cc624b12)

iii. Here, Vin = Vout, means Gate voltage = Drain voltage which means Vgs >> threshold voltage.

![image](https://github.com/user-attachments/assets/4fe813a8-485b-4f5d-8dc1-3c724672f5ef)

### <h1 id="header-3-1-5"> SKY_L4 - Static and dynamic simulation of CMOS inverter</h1>

iv. Derivation of Vm: we are trying to proof robustness of switching threshold and trying to understand how does the switching threshold varies with varying pmos and nmos.

![image](https://github.com/user-attachments/assets/c555eba6-17c5-4835-9a1c-71b41448fc5c)

* We will also do transient analysis here and calculate the rise and fall delay. We will plot Vin and Vout with time on x-axis.

Dynamic simulation SPICE netlist:

![image](https://github.com/user-attachments/assets/36cfdaca-a2e9-4fb0-941b-45c84b5013f7)

![image](https://github.com/user-attachments/assets/4e01dc4f-c958-4453-b092-c0e790851b18)

![image](https://github.com/user-attachments/assets/334001aa-0325-4644-a744-eaf3be3440ee)

Rise and fall delays are calculated using the above waveform. Basically, we see at what times input and output 50% rise/fall happening and then subtract the two.

Ex: Rise delay = Time at Vout(50%) rise - time at Vin(50%) rise

* So, we have done both static and dynamic simulation for the 1st case when Wn/Ln = Wp/Lp and got the Vm from the VTC where it cuts the 45 degree line.

![image](https://github.com/user-attachments/assets/2ec2975b-9876-4110-baf6-f7cbb79a80af)

### <h1 id="header-3-1-6"> SKY_L5 - Lab steps to git clone vsdstdcelldesign</h1>

We will git clone one of the repositories that is custom made for this workshop.

Git repository link: https://github.com/nickson-jose/vsdstdcelldesign

How to git clone?

Click on the green Code button and then copy the URL.

![image](https://github.com/user-attachments/assets/d9297783-5b60-485a-96c4-f462bff073e4)

Now use git clone command in the terminal and paste the link.

A new folder vsdstdcelldesign is created.

![image](https://github.com/user-attachments/assets/303b85b9-01ac-4d2d-8695-9341eba383be)

Opening the mag file and seeing the different layers that are used in the building of the inverter. Copy the tech file to this vsdstdcell design dir itself as we will be frequently using it. The read line that we are seeing in the above inverter layout is the polysilicon.

![image](https://github.com/user-attachments/assets/d9215dfa-b424-46c3-9c8d-5e6ee16a77b9)

![image](https://github.com/user-attachments/assets/af3e3d2f-0c9c-48d4-9715-12704c5091f8)

![image](https://github.com/user-attachments/assets/418437db-a323-4096-98a2-bba79f0b3374)

![image](https://github.com/user-attachments/assets/4a0d9d4a-c7dd-4e4b-a413-e39c084809c5)

## <h1 id="header-3-2">SKY130_D3_SKY2 - Inceptions of  Layout AA CMOS fabrication process</h1>
### <h1 id="header-3-2-1">SKY_L1 - Create Active regions</h1>

**16-mask CMOS process**

**1. Selecting a substrate**
Substrate is something on which you fabricate your complete design. There are various kind of substrate available but we will go for the most common one which we use for most of the mobile devices or any kind of device or chip you see in the real time = p-type

![image](https://github.com/user-attachments/assets/2ba831b1-d4d3-4b0b-b3f8-830145e67f96)

**2. Creating active region for transistors**
a. Grow 40nm Silicon dioxide (SiO2) [act as an insulator] on the p-type substrate.

b. Deposit a layer of 80nm Si3N4 over it.

c. Deposit a layer of photoresist (1um) on top of it. Photoresist is a film, positive or negative film that see for old cameras. On this photoresist we are going to do some process.

d. Mask1 --> When we talk about layouts those are nothing but mask in fabrication term. We basically protect some desired area through masking. In the below snippet that red color is masking. If there is UV light, then the area underneath those red masks are protected while the other resions are exposed to those UV light. So, we basically wash those resist area those are directly exposed to the UV light.

![image](https://github.com/user-attachments/assets/269106a9-b026-487f-be95-47378f8d5ab8)

e. After washing the exposed photoresist region:

![image](https://github.com/user-attachments/assets/3d4b0798-407d-4dac-891f-819b75e2a6f0)

f. Next step is to remove the mask: (These all are process of photolithography)

![image](https://github.com/user-attachments/assets/f210afe9-cc00-4d4a-af05-8d2a9e2ffa38)

g. Etched off the Si3N4, Only the area underneath the photoresist will be protected, the remaing Si3N4 area will be etched off.

![image](https://github.com/user-attachments/assets/76c30e7d-4aab-4750-afab-43d1784c0ea0)

h. Next step is to remove the photoresist itself because Si3N4 itself will act as a very good protection layer to grow the oxides on the other area.

![image](https://github.com/user-attachments/assets/9ed787b4-835a-4391-8b7a-ffb6ae01b287)

i. Now we will put this complete thing into an oxidation furnace. A furnace is a place which works at very high temperature upto 900-1000 degree celsius that helps to grow the oxide in the other areas. We have grown the first layer of SiO2 in oxidation furnace itself. Now there will be second level of growth of oxidation.

![image](https://github.com/user-attachments/assets/81d7b19c-8d9d-4a3c-b670-23c76d335387)

These areas of thick deposition of Si3N4 are called as isolation region and the **transistors at both the side won't be able to communicate to each other because of this isolation region**. This process that we have done is referred to as **LOCOS.**

![image](https://github.com/user-attachments/assets/4bf74a38-4d4a-42d3-9f83-5ea50a996cc0)

j. remove or etch out the Si3N4.

![image](https://github.com/user-attachments/assets/0bc606ac-4f4e-490a-b238-1204293d7861)

k. So, we have got the 2 active regions where we actually grow transistors and the isolation region will protect transistors so that they are not communicating with each other. So, we have actually created an electrical isolation over here.

### <h1 id="header-3-2-2">SKY_L2 - Formation of N-well and P-well</h1>

**3. N-well and P-well formation**

N-well is used for pmos fabrication and P-well is used for nmos fabrication. Both can't be done at the same time. We need to protect the one area while we fabricate the other.

The same steps will be done here also, deposit a layer of photoresist then define pattren of layer you want to protect. So we are using Mask2 to protect one area first.

![image](https://github.com/user-attachments/assets/d54ae276-566c-4ead-8185-5416c8e9377e)

Mask2 view in the layout:  top view of CMOS inverter in Magic.

![image](https://github.com/user-attachments/assets/64f8c16d-aaeb-47fd-ac9f-79e077cf4538)

Next step is to expose this photoresist to the UV light. So, same this UV light will react only to the exposed photoresist area.

![image](https://github.com/user-attachments/assets/a8e77e54-7ed6-44b7-b104-902d608c011e)

When we wash this particular thing into a solution, that exposed area of photoresist will washed away.

Now, the right area is available for any chemical reactions or anything we have to do over here.

Next step is to remove the Mask2 also. And finally we have to create a p-well over here.

P-well is created using Boron. Boron is a p-type material and it is diffused into this particular p-type substrate using a process called as Ion implantation. So, Boron being a p-type creates a P-well over here and the energy that is needed to diffuse the Boron through the oxide layer present is about 200keV.

We will do the similar steps of the N-well creation also.

![image](https://github.com/user-attachments/assets/203bc7d1-ede5-4916-9941-245efb7ba0dc)

For N-well creation, we will use Phosphorous that is an n-type material and a bit heavier than Boron. Then again the Ion implantation of Phosphorous will be done to create the N-well.

![image](https://github.com/user-attachments/assets/8ddf66d4-1a2f-44a7-88f6-2796455a518c)

![image](https://github.com/user-attachments/assets/13eabd6e-95a2-4dec-a6b5-3fcc4c33da58)

So, we have created the wells over here but the depths of the wells are not finalized yet. So, this was just the well creation.

Next we have to diffuse the wells so that it occupies almost half of the substrate area. So that we have a clear room available for pmos and nmos fabrication.

So, the next step is to take this thing, this complete substrate into a high temperature furnace. It is called as Drive in furnace.

Push it to a very high temp for a very long time about 11 degree celcius for 4-5 hrs.

So, this will diffuse the Boro and Phosphorous atoms into the p-type substrate forming the clear wells. This is called as Twin tub process.

In N-well, we are going to create pmos transistor and in P-well, we are going to create nmos transistor.

![image](https://github.com/user-attachments/assets/049bab7d-878a-4862-90df-19aadc60f95c)

### <h1 id="header-3-2-3"> SKY_L3 - Formation of gate terminal </h1>

**4. Formation of 'gate'**

![image](https://github.com/user-attachments/assets/cb0c4897-ef53-4ba7-a61a-45c84de682e1)

![image](https://github.com/user-attachments/assets/04f31988-03af-4037-896e-0376d32721ed)

We are going to control the oxide capacitance and the doping concentration through the further steps. So the next step for the formation of gate is to control the doping concentration. Same masking steps again, repetetive steps.

Threshold Voltage controlling:

![image](https://github.com/user-attachments/assets/bda99152-50e1-4103-9547-75b329b164e6)

![image](https://github.com/user-attachments/assets/6a036bc7-b8e0-40b8-8f45-d7ab653653cb)

![image](https://github.com/user-attachments/assets/842b2922-e77e-4695-8076-d4bec728fa4a)

![image](https://github.com/user-attachments/assets/3d1ceb28-994d-4f07-b614-958ecb4696bb)

Fixing of oxide: that got damaged while Ion implantations.

![image](https://github.com/user-attachments/assets/889e3106-3ba7-4d8d-bd47-52ebef80fcad)

![image](https://github.com/user-attachments/assets/28952c15-460c-44dd-ac0b-3449b908b600)

Now the formation of gate step:

![image](https://github.com/user-attachments/assets/683f752e-e099-49e5-9d8c-0f87a25813cb)

![image](https://github.com/user-attachments/assets/dd1628cf-3ea7-444d-9355-90759755cd2b)

![image](https://github.com/user-attachments/assets/b448b66e-af6f-4b85-85fe-b1a36eb678df)

![image](https://github.com/user-attachments/assets/a170d767-a310-4873-b777-6c3b64b78bd5)

![image](https://github.com/user-attachments/assets/4f69e116-a329-479b-8077-4c4c4a5b9c2f)

![image](https://github.com/user-attachments/assets/f2bce12c-0726-4d91-8947-1c296b8a007a)

### <h1 id="header-3-2-4">SKY_L4 - Lightly doped drain (LDD) formation </h1>

What we want to achieve over here is the doping profile that is **P+,P-,N in N-well where we are trying to fabricate the PMOS**.

Similarly, for the NMOS that is being fabricated in the P-well, we need **N+,N-,P** doping profile.

![image](https://github.com/user-attachments/assets/2aaa04ae-1178-453b-9b8c-793bcfc36d83)

Why do we need these kind of doping profiles?

1. Hot electron effect:

   ![image](https://github.com/user-attachments/assets/9d7ea293-2858-40f8-9f93-bb5732f2a7e2)

2. Short channel effect:

   ![image](https://github.com/user-attachments/assets/c5bd2c56-7008-40c0-90fa-81310fec76b9)

   ![image](https://github.com/user-attachments/assets/7b1f5b44-a7df-4b4d-89e9-3370d119fe91)
 
![image](https://github.com/user-attachments/assets/dd14eccd-5b8a-4bc5-bbc0-404690e69a73)

![image](https://github.com/user-attachments/assets/cd7ee9fa-1087-4c05-bc6a-0eefdb38ab04)

![image](https://github.com/user-attachments/assets/43d79775-b6e7-4183-a33f-80ae91449e03)

![image](https://github.com/user-attachments/assets/79983f3a-2b3e-4290-b112-778298a863eb)

How to protect from further Source and Drain formation?

![image](https://github.com/user-attachments/assets/e110a969-c3ef-4d92-ba9e-ae274dd72192)

![image](https://github.com/user-attachments/assets/bc3c1805-6dc4-409b-8c52-3fb59f77717a)

![image](https://github.com/user-attachments/assets/cb2e6618-1af8-42df-8480-d783f21cecab)

![image](https://github.com/user-attachments/assets/6f72aee0-8d6d-441f-937f-7385d495b59a)

### <h1 id="header-3-2-5">SKY_L5 - Source and Drain formation</h1>

The next step is to add a thin layer of screen oxide to avoid the effect of channeling.

Channeling is an effect when you do a lot of ion implantation, if the vector velocity of our ions match with that of the crystaline structure of the p-type substrate, the ions might go deep inside the p-type substrate without even hitting any of the silicon atoms.

![image](https://github.com/user-attachments/assets/c69e929e-97ce-4487-a3ab-d7bfbcc80b18)

![image](https://github.com/user-attachments/assets/b13ea438-4a43-4034-a52e-0f5056ce588c)

![image](https://github.com/user-attachments/assets/2447aa7f-7752-4303-9bb2-0d37cea36aff)

![image](https://github.com/user-attachments/assets/8687cf76-fc6d-440c-ab74-75ff36f50af1)

![image](https://github.com/user-attachments/assets/3ffef2c2-3b09-4c58-8c12-8d6f6dd91135)

![image](https://github.com/user-attachments/assets/04dd0158-de19-423e-b56d-e8fcc8cf3f2f)

![image](https://github.com/user-attachments/assets/3010227c-5f81-4115-9405-bb7c4a828190)

![image](https://github.com/user-attachments/assets/3620069e-db5f-47ef-9344-29007c371f3a)

Put this half built pmos and nmos to high temperature furnace.

![image](https://github.com/user-attachments/assets/4a2ddab5-8ac1-41ba-9647-cce7c3743c58)

### <h1 id="header-3-2-6">SKY_L6 - Local interconnect formation</h1>

**7. Steps to form contacts and interconnects (local)**

Contacts are really very imp because thats the only thing that is accessible to an user through which you can control the electrical characteristics of pmos and nmos.

![image](https://github.com/user-attachments/assets/66c602b7-52d0-44e7-a2b3-4babd30dbb63)

![image](https://github.com/user-attachments/assets/2e2eee0f-f91e-4556-bc77-0ed397c2ff92)

![image](https://github.com/user-attachments/assets/44252201-e9c0-4786-98ab-d970dd52d929)

![image](https://github.com/user-attachments/assets/d4e73c24-724b-4ad1-9628-28acdba2ebdb)

![image](https://github.com/user-attachments/assets/f5926707-3774-4183-bdaf-9578dc175158)

![image](https://github.com/user-attachments/assets/e1ee7c2d-11fd-4e75-96df-361af20f643e)

![image](https://github.com/user-attachments/assets/311f00d2-95b7-4f46-9581-748d1f158c56)

![image](https://github.com/user-attachments/assets/9ea6368d-b1fb-43ff-ab8f-b6658e66476b)

![image](https://github.com/user-attachments/assets/6916e49d-bc88-499f-bc38-e0dc33a536df)

![image](https://github.com/user-attachments/assets/77c99b38-0e7a-4559-9475-2cd3a7b7766b)

![image](https://github.com/user-attachments/assets/6258d6bc-0d66-4836-b4d5-217b694a6a1a)

![image](https://github.com/user-attachments/assets/6cbedef4-ebc7-4b8e-baee-68f48799cdfd)

![image](https://github.com/user-attachments/assets/be0064bd-7d75-46fd-8689-3d7508d213a3)

### <h1 id="header-3-2-7">SKY_L7 - Higher level metal formation </h1>

**8. Higher level metal formation**

One thing to notice here is that we have non planar surface topography and its not a good idea to deposit the metal interconnects on this layer. There are some problems wrt metal discontinuity.

So, we need to planerious this surface.

![image](https://github.com/user-attachments/assets/612eba71-bec9-4fcf-a1d1-23486859a0c1)

![image](https://github.com/user-attachments/assets/856793c0-04c9-4f56-8870-508c024dfcb2)

![image](https://github.com/user-attachments/assets/e589ab7c-684b-4686-9302-4aed724b7f5e)

![image](https://github.com/user-attachments/assets/77e1075d-863d-48ad-9507-f7d91316c27b)

![image](https://github.com/user-attachments/assets/c7773fc1-8795-4b0f-a0e5-7ac6e06ae756)

![image](https://github.com/user-attachments/assets/722c6130-1b7f-4c81-852d-54bbc4525c88)

![image](https://github.com/user-attachments/assets/747d87e5-05b9-4615-ba15-22b3991cbd88)

![image](https://github.com/user-attachments/assets/8a463d06-b07f-45af-a9c6-dd7562db843d)

![image](https://github.com/user-attachments/assets/9e6be412-1743-479e-a5c3-399916e74060)

![image](https://github.com/user-attachments/assets/2de5e0f0-603d-42a3-866c-ff914c8ce206)

![image](https://github.com/user-attachments/assets/69c5edbe-8c78-4417-a772-b7e8e8f27c68)

![image](https://github.com/user-attachments/assets/c73cc91d-133c-4422-a6da-e7408f940b5c)

Till here, we have the local interconnects (0 level of metal), 1st level of interconnects (Aluminium interconnects). Now the next step is to again take this metal levels to the higher level metal.

![image](https://github.com/user-attachments/assets/1e3d6009-06e8-49ad-9a90-3130ecfb1f4e)

![image](https://github.com/user-attachments/assets/7fa5c347-97bb-4b0a-9352-f3658f1584ae)

![image](https://github.com/user-attachments/assets/9fe10431-d4a3-40dc-b6a6-c11e82e125f6)

TiN acts an additional layer to SiO2 and acts as the barrier between lower and higher metal layers.

![image](https://github.com/user-attachments/assets/a3f7e3b1-717c-4aef-b34d-67a076cc61f8)

![image](https://github.com/user-attachments/assets/6fc3d406-db7c-4ff4-a9fe-c8d11bb94634)

![image](https://github.com/user-attachments/assets/2a8f3c0e-8b30-4212-be44-1bc517a72c87)

![image](https://github.com/user-attachments/assets/25e57f5f-133d-48e0-91b5-933496c67784)

16 mask CMOS process will look like:

![image](https://github.com/user-attachments/assets/28f61c4f-2a85-4dab-93f7-a9549f1e1003)

### <h1 id="header-3-2-8">SKY_L8 - Lab introduction to Sky130 basic layers layout and LEF using inverter</h1>

**9. Lab introduction to Sky130 basic layers layout and LEF using inverter**
    
1. On the right side of the CMOS inverter layout, we have all color palets, these are basically the layers.

![image](https://github.com/user-attachments/assets/d71b8c82-0642-4472-a870-be2b52d83679)

Green is the ndifusion layer, for verifying you can go to the green color in the color palet and it will show ndiffusion written at the top right bar.

When the poly crosses n-diffusion, its an NMOS. Similarly, when the poly crosses p-diffusion, its a PMOS.

For verifying the NMOS, we selected the region and then wrote what in the tkcon, it came out to be NMOS.

![image](https://github.com/user-attachments/assets/c6123b75-b59a-4163-b1ff-7a032976862e)

Similarly, we did for PMOS.

![image](https://github.com/user-attachments/assets/8374b21b-3528-401a-b8fe-264fe91aea4f)

Now we will verify that the drain of PMOS and NMOS are connected.

For that, place your cursor at the output pin Y and press S twice, all the highlighed boundary in white in connected which shows that drains of both PMOS & NMOS are connected.

![image](https://github.com/user-attachments/assets/3bd160d9-21c2-453a-8132-29036c0f0cf1)

Now, check the connection of source of PMOS:

![image](https://github.com/user-attachments/assets/fc7765a7-78e7-4591-be16-915eea9d9948)

So, source of the PMOS is connected to VDD net.

Similarly, verified that the source of NMOS is connected to ground.

![image](https://github.com/user-attachments/assets/f55a71d9-a7db-4b49-b0c0-d450dcfe9208)

Lab steps to create std cell layout and extract spice netlist: https://github.com/nickson-jose/vsdstdcelldesign


### <h1 id="header-3-2-9">SKY_L9 - Lab steps to create std cell layout and extract spice netlist </h1>

How do we know what is the logical function of this inverter?

For that, we would first extract this SPICE and post that we will do simulations in ngspice.

To extract it on spice:

Open the tkcon window and see where we are and extract it in a file using the command extract all.

![image](https://github.com/user-attachments/assets/e7f764f1-cfa7-446b-a85a-403fb4ddb893)

![image](https://github.com/user-attachments/assets/0001ce17-e65d-4aaa-8855-6447b8614e82)

Now, we will use this ext file to create spice file to be used with the ngspice tool using command ext2spice.

![image](https://github.com/user-attachments/assets/e3083e3a-2601-4299-a9b8-d8cf83525463)

![image](https://github.com/user-attachments/assets/27cc5b4b-0d35-42cd-ae73-c30eee56a865)

Extracted spice netlist:

![image](https://github.com/user-attachments/assets/e238194d-5a97-42fc-807f-dfc934593d05)

![image](https://github.com/user-attachments/assets/a105a597-f0d0-4a80-bc0d-62829b09458e)

## <h1 id="header-3-3">SKY130_D3_SKY3 - Sky130 Tech File Labs</h1>
### <h1 id="header-3-3-1">SKY_L1 - Lab steps to create final SPICE deck using Sky130 tech</h1>

1.Netlist:

Double tick ones are defined in the netlist. We need to add some more lines to SPICE code for the below circuit.

![image](https://github.com/user-attachments/assets/064b848f-3616-4894-af9d-166b315f489f)

2. Edited SPICE netlist:

![image](https://github.com/user-attachments/assets/68fd99fb-92d1-4c25-821c-43f51b34c565)

We will run it in ngspice and will check the result.

![image](https://github.com/user-attachments/assets/18becc03-97d1-4a33-9c1a-52a3443012c8)

![image](https://github.com/user-attachments/assets/71e1d837-e94e-484b-ae56-e0b22ba80e72)

Plotted the Y vs time A

![image](https://github.com/user-attachments/assets/5231c533-2c38-4fa1-8337-466fa444f577)

![image](https://github.com/user-attachments/assets/6e01a6dd-9dd0-43a6-a266-b7f58a627ee2)

We can see the spikes, load is very less, will modify the netlist.

Edited netlist:

![image](https://github.com/user-attachments/assets/a4d352db-6d82-404a-88ed-e08f74d14386)

![image](https://github.com/user-attachments/assets/5231c533-2c38-4fa1-8337-466fa444f577)

![image](https://github.com/user-attachments/assets/205d83db-c249-40fa-9060-bbdcec6b540c)

### <h1 id="header-3-3-2">SKY_L2 - Lab steps to characterise inverter using sky130 model files</h1>

1. Rise Transition --> Time taken by the output to rise from 20 to 80% of the max value.

20% of 3.3 = 0.66, 80% of 3.3 = 2.64

![image](https://github.com/user-attachments/assets/080d12cf-364a-4bd4-a5af-8cb7e33f8ba8)

Rise transition = 0.064 ns

Similarly, Fall transition = 0.042 ns

2. Cell Fall/Rise delay --> cell propagation delay when the output is falling/rising between 50% of the values.

50% of 3.3 V = 1.65 V

So we will fine the time diff between input and output when the value is 1.65 V.

![image](https://github.com/user-attachments/assets/115d4973-c26c-4c09-9dae-b70e109aa685)

rise delay = 0.061 ns

Similarly, fall delay = 0.027 ns

So, we have got all the four parameters above, the cell characterization is done.

### <h1 id="header-3-3-3">SKY_L3 - Lab introduction to Magic options and DRC rules</h1>

![image](https://github.com/user-attachments/assets/fc054020-f092-4955-a8e2-57768a35b477)

![image](https://github.com/user-attachments/assets/29ae29cf-9531-4559-adf4-dc9dbb45c373)

![image](https://github.com/user-attachments/assets/74a50932-9864-4b91-be97-6beedcd25856)

Magic DRC documentation: http://opencircuitdesign.com/magic/

### <h1 id="header-3-3-4">SKY_L4 - Lab exercise to implement pdks and steps to download labs</h1>

![image](https://github.com/user-attachments/assets/d4be1157-64a3-4d37-81a9-8d5f6f854dc4)

Skywater documentation: https://skywater-pdk.readthedocs.io/en/main/rules/background.html

DRC rules: http://opencircuitdesign.com/magic/techref/maint2.html#drc

![image](https://github.com/user-attachments/assets/3deae950-9ebb-4fce-b205-d1e3e985bdd5)








### <h1 id="header-3-3-5">SKY_L5 - Lab introduction to Magic and steps to load Sky130 tech-rules</h1>


### <h1 id="header-3-3-6">SKY_L6 - Lab exercise to fix poly.9 error in Sky130 tech-file</h1>


### <h1 id="header-3-3-7">SKY_L7 - Lab exercise to implement poly resistor spacing to diff and tap</h1>


### <h1 id="header-3-3-8">SKY_L8 - Lab challenge exercise to describe DRC error as geometrical construct</h1>


### <h1 id="header-3-3-9">SKY_L9 - Lab challenge to find missing or incorrect rules and fix them</h1>



# <h1 id="header-4">SKY130 Day4 - Pre-Layout timing analysis and importance of good clock tree</h1>
## <h1 id="header-4-1">SKY130_D4_SK1 - </h1>
### <h1 id="header-4-1-1">SKY_L1 - </h1>
### <h1 id="header-4-1-2">SKY_L1 - </h1>
### <h1 id="header-4-1-3">SKY_L1 - </h1>
### <h1 id="header-4-1-4">SKY_L1 - </h1>
### <h1 id="header-4-1-5">SKY_L1 - </h1>
### <h1 id="header-4-1-6">SKY_L1 - </h1>
### <h1 id="header-4-1-7">SKY_L1 - </h1>

## <h1 id="header-4-2">SKY130_D4_SK2 - </h1>
### <h1 id="header-4-2-1">SKY_L1 - </h1>
### <h1 id="header-4-2-2">SKY_L1 - </h1>
### <h1 id="header-4-2-3">SKY_L1 - </h1>
### <h1 id="header-4-2-4">SKY_L1 - </h1>
### <h1 id="header-4-2-5">SKY_L1 - </h1>

## <h1 id="header-4-3">SKY130_D4_SK3 - </h1>
### <h1 id="header-4-3-1">SKY_L1 - </h1>
### <h1 id="header-4-3-2">SKY_L1 - </h1>
### <h1 id="header-4-3-3">SKY_L1 - </h1>
### <h1 id="header-4-3-4">SKY_L1 - </h1>

## <h1 id="header-4-4">SKY130_D4_SK4 - </h1>
### <h1 id="header-4-4-1">SKY_L1 - </h1>
### <h1 id="header-4-4-2">SKY_L1 - </h1>
### <h1 id="header-4-4-3">SKY_L1 - </h1>
### <h1 id="header-4-4-4">SKY_L1 - </h1>
### <h1 id="header-4-4-5">SKY_L1 - </h1>

# SKY130 Day 5 - Final steps for RTL2GDS using tritonRoute and openSTA
## SKY130_D5_SKY1 - 
### SKY_L1 -
### SKY_L1 -
### SKY_L1 -

## SKY130_D5_SK2 - 
### SKY_L1 -
### SKY_L1 -
### SKY_L1 -

## SKY130_D5_SK3 - 
### SKY_L1 -
### SKY_L1 -
### SKY_L1 -
### SKY_L1 -


































