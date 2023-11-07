# Description  
## Important information
[RTC Dashboard](https://ccm.whirlpool.oncloudone.com/ccm/web/projects/EES%20Platform%20Vertical%20Axis%20(Change%20Management)#action=com.ibm.team.dashboard.viewDashboard&team=VA-2021-Mini-Proj)  

This Firmware is designed for a 256K (RX130, R5F51306) Amazon ACU (P2) and a Sensored PSC Motor. 

This Firmware (and IAP FW) is compatible with the 512K RX130 micro (R5F51308), but has been adjusted to fit inside the same space as the 256K RX130 micro. This was done to allow the use of the same firmware on an ACU with a 256K or 512K micro.

This Firmware supports both the ITM and Panasonic electronic pressure sensor. Selection is determined by virtual pin used in the setting file.

## Tool Information
* MAC Revision: 1.19.0.0
* GESE Version: 1.0.17.0

## Setting file                                                                                    
- **FVT_Setting_File_ITM**: TBD
- **FVT_Setting_File_Panasonic** : TBD
- **ACU_Config1**: TBD
   

## Class B signature
* System SHA256:  TBD

## Memory Usage                                                          
  * ROM: TBD (x/262,144)  
    * x bytes of readonly  code memory
    * x bytes of readonly  data memory
    * x IAP (Size: 12,288 bytes)
    * x Setting File (Size: 38912 bytes, Starting position: 4294916096 (this was done to force it to fit in 256K space))                                                     
  * RAM: TBD (x/32,768)
    * x bytes of readwrite code memory
    * x bytes of readwrite data memory (+ 4 absolute)
      
## Download Instructions
  * Download this firmware by using the buttons under the project name.  
  * Go to version tab to check other versions.   

## FILE TO BE USED FOR VALIDATION FROM BINARY PACKAGE DOWNLOAD: 
File starting with: IAP_CFW is a MERGED file with IAP + Core Firmware + FVT setting file  
Before START any validation, ensure CHIP is ERASED.  
This file CAN ONLY be programmed with a FLASH PROGRAMMER.

File to be used ***only when update is done with MAC/NTL***  
File starting with: CFW is the merge of Core Firmware + FVT setting file

Boot-loader firmware: TBD [Track Build Item 1246665](https://ccm.whirlpool.oncloudone.com/ccm/resource/itemName/com.ibm.team.workitem.WorkItem/1246665) (1242032 V00.01.06)

  This version uses version 01.00.00 of the IAP FW for the RX130 (256K) (Stream: IAP_RX130_256K_COM12_ACU)