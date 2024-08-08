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































































































































































































































