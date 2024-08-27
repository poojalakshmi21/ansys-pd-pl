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

## SKY130_D2_SK3 - Cell design and characterization flows  
### SKY_L1 - Inputs for cell design flow 

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

### SKY_L2 - Circuit design step 

c. **Library & user-defined specs**: Cell-height, supply voltage, metal layers, pin location, drawn gate length, etc

![image](https://github.com/user-attachments/assets/0581ea5a-3d0f-4e79-9bac-bff786b8379a)

![image](https://github.com/user-attachments/assets/45bfb442-fb9b-42df-8bfe-2a296965da09)

2. **Design Steps**
a. **Circuit design**: implement the function and model nmos and pmos to meet the library requirement, will get the information about W/L of the nmos and pmos in this step. Once we know the value of W/L for the transistors, next step is to implement these values in the layout called as layout design. Output of the Circuit design step is CDL (circuit description language)

![image](https://github.com/user-attachments/assets/f7007bfc-6dea-4fbd-8752-1bc596e79563)

b. **Layout design**: First step is to get the function implemented through the mos transistors. The next step is to get the pmos network graph and nmos network graph. Output of the layout design - GDSII, LEF, extracted spice netlist/ckt

![image](https://github.com/user-attachments/assets/a0c01820-7763-4e04-a98d-ae8b6cc18689)

### SKY_L3 - Layout design step 

Next step is to obtain the Euler's path.

![image](https://github.com/user-attachments/assets/52bcc0fc-2adf-4764-b872-83bdab8f8aca)

Once you obtain a Euler's path, draw a stick diagram out of it.

![image](https://github.com/user-attachments/assets/9f575b1c-255f-451a-a593-59b6b08419c2)

Next step is to convert this stick diagram into a proper/typical layout according to the rules from the inputs.

![image](https://github.com/user-attachments/assets/f45e50d2-e4c9-4836-bf67-651dc131c038)

Next step is to extract the parasitics and characterize them in terms of timing.

![image](https://github.com/user-attachments/assets/0715a97c-1dcc-4f42-8a83-3bd212bc36e4)

### SKY_L4 - Typical characterization flow

c. **Characterization**

![image](https://github.com/user-attachments/assets/3651383b-bf29-4cb6-b9a4-7b35f6a9c856)

So, what we have till this step: layout of buffer, description of buffer, extracted spice netlist, subckts, nmos pmos spice models, etc.

![image](https://github.com/user-attachments/assets/bf4e1e93-6627-49c6-8ca1-88c14b9d4927)

![image](https://github.com/user-attachments/assets/a1fdd922-3223-4e95-8ebd-b92f0d5615d0)

![image](https://github.com/user-attachments/assets/063f3288-d914-42e7-bbf5-a77a0c7f4aa7)

![image](https://github.com/user-attachments/assets/c472f485-b0e1-4c69-8cc1-4f4f62b75f68)

3. **Outputs**
these are actually used by the EDA tools.
 
## SKY130_D2_SK4 - General timing characterization parameters  
### SKY_L1 - Timing threshold definitions

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

### SKY_L2 - Propagation delay and transition time

f. **Propagation delay:**

![image](https://github.com/user-attachments/assets/7e58eaa8-7a27-4741-82eb-636ad3cecfbf)

g. **Transition time:**

![image](https://github.com/user-attachments/assets/a5559602-9d2a-4092-b2a7-9a39bd7896f4)

![image](https://github.com/user-attachments/assets/a8f376a4-859d-466c-b2bb-9984fd455232)

![image](https://github.com/user-attachments/assets/fad295e6-5ebb-4e0e-b9f9-93788d288f1d)

g. **Output current waveform and Output voltage waveform:**

# SKY130 Day3 - Design library cell using Magic Layout and ngspice characterization
## SKY130_D3_SKY1 - Labs for CMOS inverter ngspice simulations
### SKY_L0 - IO placer revision

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

### SKY_L1 - SPICE deck creation for CMOS inverter

SPICE simulations: 350nm, 250nm mos are available.

1. Create a SPICE deck for VTC CMOS characteristics: SPICE deck is nothing but a netlist, a connectivity information

a. When we say W/L of mos it means it is the W/L of the channel of mos.

b. In cmos, generally pmos should be wider than the nmos. Ideally, pmos should be twice or thrice of the nmos. But the spice deck we are creating is having nmos and pmos of the same W/L.

![image](https://github.com/user-attachments/assets/291ca74c-c8c1-4c85-824a-b8f17ecccdcd)

Here M1 = pmos, M2 = nmos

![image](https://github.com/user-attachments/assets/cddce7ee-23da-479a-a32a-c7a3de795526)

Syntax of Mosfet in the SPICE: M1 Drain Gate Source Substrate type W L = M1 out in vdd vdd pmos 0.375u 0.25u

### SKY_L2 - SPICE simulation lab for CMOS inverter

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

### SKY_L3 - Switching Thershold Vm

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

### SKY_L4 - Static and dynamic simulation of CMOS inverter

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







### SKY_L5 - Lab steps to git clone vsdstdcelldesign

## SKY130_D3_SKY2 - Inceptions of  Layout AA CMOS fabrication process
### SKY_L1 - Create Active regions
### SKY_L2 - Formation of N-well and P-well
### SKY_L3 - Formation of gate terminal 
### SKY_L4 - Lightly doped drain (LDD) formation
### SKY_L5 - Source AA drain formation
### SKY_L6 - Local interconnect formation
### SKY_L7 - Higher level metal formation
### SKY_L8 - Lab introduction to Sky130 basic layers layout and LEF using inverter
### SKY_L9 - Lab steps to create std cell layout and extract spice netlist 


## SKY130_D3_SKY3 - Sky130 Tech File Labs
### SKY_L1 - Sr
### SKY_L2 - SP
### SKY_L3 - S
### SKY_L4 - Sta
### SKY_L5 - L
### SKY_L5 - L
### SKY_L5 - L
### SKY_L5 - L
### SKY_L5 - L

# SKY130 Day4 - 
## SKY130_D4_SK1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 

## SKY130_D4_SK2 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 

## SKY130_D4_SK3 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 

## SKY130_D4_SK4 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 - 
### SKY_L1 -
### SKY_L1 -

# SKY130 Day 5 - 
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


































