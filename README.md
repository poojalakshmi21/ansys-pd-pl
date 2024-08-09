# Sky130 Day 1 - Inception of open-sorce EDA, OpenLANE and Sky130 PDK
# Sky130_D1_SK3  - Get familiar to open-sorce EDA tools
# SKY_L1 - OpenLANE Directory Structure in detail
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

# SKY_L2 - Design Preparation Step
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

# SKY_L3 - Review files after design prep and run synthesis
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

# SKY_L4 - OpenLANE Project Git Link Description
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

# SKY_L5 - Steps to characterize synthesis results
**Notes**

Task 1: To find flop ratio, that is number of D-FlipFlops or total no. of cells

![image](https://github.com/user-attachments/assets/6aa7420e-fd9a-4348-b2cb-be7f1cbb1e83)

No. of cells = 14876

No. of D-FFs = 1613

Clock count = No. of D-FFs/No. of cells = 1613/14876 = 0.1084

Percentage = 10.84%











































































































































































































































