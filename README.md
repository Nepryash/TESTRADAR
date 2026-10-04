# Radar_software
By: Vlad
Original date: 00/00/00



Refer to DSS Radar Program Manual for exact steps in setting up the project.

This is an alternate branch of the DSS Radar Program which already includes all the relevant SDK dependencies required for running the mmWave Program.
Warning: Due to size limitations, not all of the original files are present in this repository, and errors could occur as new functionality is enabled. 
In this case, the full dependency folders may need to be downloaded so missing components can be compared and re-added into the Dependency folder of this repo.

Notice: Due to the code still utilizing much of code written by Texas Instruments, external distribution of this code is likely not adviced.
But, the program should be fine to use for DSS internal usage.


This code was put together by importing the Out of Box demo code for AWR2944EVM radar board into CCS 20
This was used to import the "project structure", before the source code was replaced from the non-project code file contained
in the MCUPlus 4.7 SDK.

Originally the SDK Code was only used as a way to Debug the code when using the premade Binaries and 
Appdata for the mmWDemo_DDM/DDM and was not intended to be a functional set of code.

However, effectively pasting this debug code on top of the Radar Toolbox code made it accessible and usable.
Following this, the code functioned as a version of the mmWDemo_DDM code.

Following this, by changing the include and define settings within the CCS itself, the TDM Functionality of the code could be enabled.
Afterwards, the code's linker file was manipulated to better facilitate the memory management, as TDM processing chain required greater deal of memory compared to
DDM.

The radar code now compiles and effectively works as a customizable version of the mmWDemo_TDM out of box code.



