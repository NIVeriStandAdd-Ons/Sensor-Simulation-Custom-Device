Sensor Simulation 1.2.0

Migrating from previous versions of this Add-on
----------------------------------------------------------------------------------------------
0. Read the release notes from your version of the add-on to this version. Some notes are important and dictate additional actions you must take.
1. Follow the instructions for installing the add-on and drivers (below). This will update your files on disk to be the latest version.
2. Open system definitions containing the add on with System Explorer, save and close them. This will force a mutation.

***ADD ON INSTALL***
To install this add-on:
-*With NI VeriStand closed*:
1. Copy the contents of the "Built" directory into your "<Public Documents>\National Instruments\<NI VeriStand Version>\Custom Devices\" directory.

***KNOWN ISSUES***

***CHANGE LOG***
1.2.0
<Bug> fixed a critical issue causing the 5 wire LVDT simulation to be incorrect, as we were not taking the transfer ratio into account and incorrectly using sensitivty instead of 'difference over sum gain'. After upgrading, users of 5 wire LVDTs need to revisit the configuration page and enter the transfer ratio and difference over sum gain.

1.1.0
<Bug> Fixed a few rare bitfile parsing issues
<Bug> Fixed an issue where a warning like code 61003 would be treated as an error and shut down the veristand engine
<Feature> Performance increased by more than 50%

1.0.5
<Bug> Fixed a critical issue preventing the use of this device with FPGA IP containing more than one resolver

1.0.4
<Change> Several changes to source build setup. Not noticeable unless using the source.

1.0.2
<Bug> Fixed critical error preventing the use of the device if there were FPGA devices in the sysdef

1.0.1
<Bug> Resolved a crash if you use this custom device along with the Engine simulation custom device

1.0 - Release