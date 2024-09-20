# Synthetic Ice Core Logbook

## Table of Contents
- [System Development and Setup](#system-development-and-setup)
  - [Updated Heat Jacket, Pulley System and Stepper Motor Setup](#updated-heat-jacket-pulley-system-and-stepper-motor-setup)
  - [Pump System](#pump-system)
- [Guide: How to Operate the System](#guide-how-to-operate-the-system)
- [Ice record](#ice-record)

## System Development and Setup

### Updated Heat Jacket, Pulley System and Stepper Motor Setup

The heat jacket used when freezing the synthetic ice core is being lifted by a pulley system connected to a stepper motor. The controls of this pulley system and stepper motor have been updated (summer 2024) with a custom PCB and controller case.

The custom PCB has been designed in the ECAD suite of Autodesk fusion ([see files here - current version is V14](https://github.com/vgkinis/synthetic_ice_core/tree/main/Fusion_PCB_Project/ECAD_files)). The Gerber files from the ECAD project have then been sent to JCLPCB in China (delivery with DHL priority plus).

See images of of the ECAD PCB:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_schematic.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_outline.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_outline_DIGI.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_outline_ANA.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_outline_9PIN.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_3D_top.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_3D_bottom.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_3D_side.png)

Additionally, a case to mount on the pulley system has been made to contain the arduino and PCB:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_case_side.png)

The mounting brackets are fastened to the case with 4 modified autowrentching thin-head M4 screws that fit in the narrow space in the case:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/M4_autowrench.png)

The MCAD files for these can be found with [the ECAD files](https://github.com/vgkinis/synthetic_ice_core/tree/main/Fusion_PCB_Project/ECAD_files).

The physical PCB can be seen in the following photos:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_IMG.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_case_open1.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_CONX.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_case_open.png)
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/PCB_case_closed.png)

On the stepper motor side the connections are as follows:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/Stepper_connections.png)

The connections have so far been as follows:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/Stepper_CONX.png)

The connection between the PCB and the stepper motor is achieved with a custom cable with a female dsub 9pin plug:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/DSUB_CONX.png)

This cable will then be connected to the stepper motor through a connector- see diagram:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/Fusion_PCB_Project/Images/CONX_diagram.JPG)

### Pump System

Water used for the synthetic ice cores must first be degassed. This is done by pumping on the water while heating and stirring it. Since this means a lot of vapor will be pumped a condensation trap is necessary.

A diagram of the setup can be seen here:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/experiments/Initial_test/IMG/diagram.JPG)

The actual setup looks like this:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/experiments/Initial_test/IMG/setup.png)

The condensation trap consists of en closed vacuum volume before the pump inlet submerged in a liquid nitrogen filled dewar held up with a 3D printed bracket:
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/experiments/Initial_test/IMG/condensation_trap.png)

When heated, stirred and pumped the outgassing looks like this: [Watch the video on YouTube](https://www.youtube.com/watch?v=-hlvExogXq0)

## Guide: How to Operate the System


## Ice Record

- Attempt No. 1: Pumped 30 minutes at 35 C (left for a long time). Heated at 150V over approx 2 days. Resulting ice core had a big column of bubbles surrounded by clear ice. Likely cause condensation nuclei.
- Attempt No. 2: Pumped 30 minutes at 35 C put in freezer immediately. Heated at 150V over approx 2 days. Resulting ice core had a smaller column of bubbles but was otherwise pretty clear.
- Attempt No. 3: Pumped 60 minutes at 35 C put in freezer immediately. Heated at 150V over approx 2 days.

### Result from Attempt 3 

Needs to be closer inspected - are these bubbles or impurities?
![image](https://github.com/vgkinis/synthetic_ice_core/blob/main/experiments/Initial_test/IMG/IMG_20240916_103403841_AE.jpg)
