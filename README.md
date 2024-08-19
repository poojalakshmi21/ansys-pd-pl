# Sky130 Day 1 - Inception of open-sorce EDA, OpenLANE and Sky130 PDK
## Sky130_D1_SK3  - Get familiar to open-sorce EDA tools
### SKY_L1 - OpenLANE Directory Structure in detail
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

### SKY_L2 - Design Preparation Step
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

### SKY_L3 - Review files after design prep and run synthesis
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

### SKY_L4 - OpenLANE Project Git Link Description
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

### SKY_L5 - Steps to characterize synthesis results
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

# Sky130 Day 2 - Good Floorplan vs Bad Floorplan and Introduction to library cells
## Sky130_D2_SK1 - Chip Floor planning considerations
### SKY_L1 - Utilization factor and aspect ratio
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

### SKY_L2 - Concept of pre-placed cells
**Notes**

2. Define locations of Preplaced cells:

a. Preplaced cells are the black boxes having some specific functionality that is implemented once separately and then can be instantiated multiple times.

![image](https://github.com/user-attachments/assets/b4c34c06-0c1c-484a-a4a2-52878a2d3e24)

b. Preplaced cells are macros or IPs like memory, clock-gating cell, comparator, mux.

![image](https://github.com/user-attachments/assets/3f38493d-cdb0-4fbc-a465-a45f8165150e)

c. The arrangement of these IPs in a chip is referred as floorplanning. These IPs/blocks have user-defined locations, and hence are placed in the chip before automated placement-and-routing, and are called as preplaced cells. Automated placement and routing tools place the remaining logical cells in the design onto the chip. Place the preplaced cells on the basis of design scenario or design background.

### SKY_L3 - De-coupling capacitors
**Notes**

3. Place the pre-placed cells closer to the input area and surround the preplaced cells with decoupling capacitors.

a. Decoupling capacitors are the huge capacitors that are completely filled with charge. Voltage across the decoupling capacitor is equivalent to the supply voltage. If power supply is 1V, decap will be charged till 1V. Decoupling capacitor is placed very near and parallel to the circuit. Everytime the circuit switches, it draws current from decap, whereas the RL network is used to replenish the charge into decap. As the name suggests, decoupling capacitor decouples the circuit from the main supply. With the help of decap local communication is taken care.

![image](https://github.com/user-attachments/assets/aa3209ca-8313-4674-9042-2604e5ebe5f6)

### SKY_L4 - Powerplanning
**Notes**

4. Powerplanning

Possibilities of ground bounce and voltage droop issues due to usage of a single power supply is solved by powerplanning. 

![image](https://github.com/user-attachments/assets/ec7ce61c-a748-4a66-a85e-01c409e071d3)

![image](https://github.com/user-attachments/assets/fab8c983-d395-4ec2-8485-0f5933bd25d7)

![image](https://github.com/user-attachments/assets/32e0aa7a-b643-4da5-9851-37af465d58b5)

![image](https://github.com/user-attachments/assets/4937e2f5-904c-46f9-9b73-4a0521c26ab8)

Mltiple power supply through mesh structure for VDD and VSS.

![image](https://github.com/user-attachments/assets/b36d615d-88f5-4663-9ebf-5ca0986eb9cb) 

### SKY_L5 - Pin Placement and logical cell placement blockage.
**Notes**

5. Pin Placement and logical cell placement blockage.

Pin Placement

   ![image](https://github.com/user-attachments/assets/9601af54-467f-4b2f-8648-74cb34438fe7)

   ![image](https://github.com/user-attachments/assets/3eccb2e6-4849-4765-b612-f11411ef080f)

Clock ports are bigger than the data ports because clock drives all seq cells continuosly, basically they drives all the flops in the full chip. So, we need the least resistance path for the clocks. 

Logical cell placement blockage

![image](https://github.com/user-attachments/assets/72424990-49c7-4642-be51-aebd47c9463a)

We block the area between core and die to avoid placement of any logical cells in those areas by automated placement and routing tools because that area is reserve for the pin locations.

### SKY_L6 - Steps to run floorplan using OpenLANE

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

### SKY_L7 - Review floorplan files and steps to view floorplan

![image](https://github.com/user-attachments/assets/c4e3b3cf-b271-4ac8-8716-c88c93f5d3a1)

Opening def file: 

![image](https://github.com/user-attachments/assets/2e2638cc-e5b7-491e-aaa4-90a84f93dd04)

Viewing the floorplan in magic:

![image](https://github.com/user-attachments/assets/4037ffe9-c81b-4ef0-b693-1fbc9459f63d)

![image](https://github.com/user-attachments/assets/e1575759-f690-4709-bbac-8eff7d17a305)

### SKY_L8 - Review floorplan layout in Magic 

Viewing layout after the floorplan using magic tool:

To open the layout:

![image](https://github.com/user-attachments/assets/e5d5a059-1b34-4439-b041-fb9dc9e1c010)

![image](https://github.com/user-attachments/assets/d268292e-0c96-4208-9b64-e9404c8f2afa)

![image](https://github.com/user-attachments/assets/8ff5e68a-bda2-45cc-bd3a-6d05894c2499)

![image](https://github.com/user-attachments/assets/25d392ec-d2ef-4ef3-9a2a-836446cbbb6b)

Floorplan does place the standard cells. They are present in the lower left corner of the layout:

![image](https://github.com/user-attachments/assets/504478bd-c95c-4d7a-98d9-cf7e0ba52a1b)

## SKY130_D2_SK2 - Library Binding and Placement  
### SKY_L1 - Netlist binding and initial place design 

1. Bind netlist with physical cells:

The netlist contains different gates and the shape of each gate defines its functionality. Example: By the shape of OR gate we understand that it will perform OR operation. But in reality, we don't have such shapes for different gates, we just have a box structure for each gate that has some width and height (physical dimension).

![image](https://github.com/user-attachments/assets/396f129f-e41f-4d17-a86f-64c02c17249d)

![image](https://github.com/user-attachments/assets/e43fe760-c054-48b8-bc8e-3fad243b94f6)

![image](https://github.com/user-attachments/assets/5379a1ee-a77a-4b95-8a32-0c81cddad7a5)


2. Placement:

After having proper shapes and sizes to each gate, these shapes and sizes are placed onto the floorplan. Now we have the floorplan, netlist, and physical view of the logic gates.

![image](https://github.com/user-attachments/assets/b52f4d9b-2ae9-4149-8585-6713df6a1606)

### SKY_L2 - Optimize placement using estimated wire-length and capacitance

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

### SKY_L3 - Final placement optimization

![image](https://github.com/user-attachments/assets/06d7a0be-3694-4b57-8ae3-7e0fc4c1cba5)

The elements FF1, 1 ,2 and FF2 logics are abutted, that is, there is no time delay between signal passed from FF1 to FF2. There are multiple reasons to do abutment, let's say this particular section of the circuit works at a very high speed and zero time delay is required, and don't want to waste delays on wires, and therefore, the abutment is done for those logics. This is a classic example of high frequency ckt usages.

![image](https://github.com/user-attachments/assets/1c97a956-7490-4507-a2eb-1127e191b80a)

![image](https://github.com/user-attachments/assets/3aceb05d-286e-4676-ac5f-45e3760d421e)

### SKY_L4 - Need for libraries and characterization

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

### SKY_L5 - Congestion aware and placement and RePlAce 




## SKY130_D2_SK3 - Cell design and characterization flows  
### SKY_L1 - Inputs for cell design flow 
### SKY_L2 - Circuit design step 
### SKY_L3 - Layout design step 
### SKY_L4 - Typical characterization flow
 
## SKY130_D2_SK4 - General timing characterization parameters  
### SKY_L1 - Timing threshold definitions
### SKY_L2 - Propagation delay and transition time

# SKY130 Day3 - Design library cell using Magic Layout and ngspice characterization
## SKY130_D3_SKY1 - Labs for CMOS inverter ngspice simulations
### SKY_L0 - IO placer revision
### SKY_L1 - SPICE deck creation for CMOS inverter
### SKY_L2 - SPICE simulation lab for CMOS inverter
### SKY_L3 - Switching Thershold Vm
### SKY_L4 - Static and dynamic simulation of CMOS inverter
### SKY_L5 - Lab steps to git clone vsdstdcelldesign

## SKY130_D3_SKY2 - Inceptions of  Layout AA CMOS fabrication process
### SKY_L1 - 
### SKY_L2 - 
### SKY_L3 - S
### SKY_L4 - S
### SKY_L5 - L

## SKY130_D3_SKY3 - Sky130 Tech File Labs
### SKY_L1 - Sr
### SKY_L2 - SP
### SKY_L3 - S
### SKY_L4 - Sta
### SKY_L5 - L

# SKY130 Day4 - 
## SKY130_D4_SKY1 - 
### SKY_L1 - 

# SKY130 Day 5 - 
## SKY130_D5_SKY1 - 
### SKY_L1 -



















2. Library Binding & Placement

a. Netlist binding & initial place design

i. Library contains the information on the size & timing of the standard cells & IPs/macros

ii. Same standard cells can have multiple sizes based on the drive strength of the cells

iii. If we place the cells very close to the others (abutment), the cell delay is minimal, otherwise, we may have to use buffers if the distance between the two cells is big.

b. Optimize placement using estimated wire length & capacitance

i. So, if two cells are far away from each other, the wire resistance & capacitance is very high causing very high RC delay

ii. Slew depends upon the capacitance value & high capacitance values will produce bad slew

c. Final Optimization

i. Abutment is preferred for critical paths since the delay between the cells is negligible and the circuit can work extremely fast.

d. Need for libraries & characterization

i. Library characterization & modeling: Logic synthesis -> Floorplanning -> Placement -> CTS -> Routing -> STA

ii. One thing is common in all these stages – gates/cells

iii. In each of the ASIC design flow needs to have the library information on the cells

e. Congestion Aware placement using RePIAce

i. After floorplan, next stage is placement stage

ii. Two sub-stages for placement: 1. Global placement (coarse & no legalization) 2. Detailed placement (legalization happens in detailed placement)

iii. Legalization: Cells should be exactly inside the rows, no overlap on other cells, should be abutted, important from timing point of view

iv. The command run_placement is performed. Wire length reduction is the focus here.












































































































































































































































