
#Oculus Rift Development Kit 1
Firmware, Schematics, and Mechanicals for the Oculus Rift Development Kit 1.

Firmware

The Tracker firmware uses the CooCox CoIDE for development along with the gcc-arm-embedded toolchain.

The ST-Link/V2 is the cheapest way to load firmware onto a Tracker board, though any SWD compatible programmer should work. You can follow these steps to set up a build environment and load firmware onto the board:

Install ST-Link drivers if you haven't: http://www.st.com/web/en/catalog/tools/PF258167
Install CoCenter: http://www.coocox.org/CooCox_CoIDE.htm
Through CoCenter, install CooCox and CoFlash
Install gcc-arm-embedded: https://launchpad.net/gcc-arm-embedded/+download
Set up gcc-arm-embedded in CooCox: http://www.coocox.org/CoIDE/Compiler_Settings.html
Clone our RiftDK1 repository to C:\CooCox\CoIDE\workspace
Open the Tracker.coproj
Build
Plug the ST-Link into the board's 10 pin SWD header.
Plug in USB to power the board.
Download code to Flash
Enjoy!
Note that the USB Product ID is set to 0x0001, which matches the production version of the Tracker. If you modify the firmware in a way that changes the USB interface, please change the Product ID to 0x0000.

Mechanical

The Mechanical folder contains STEP files of the Rift DK1 housing, control box, and case.

Schematics

The Schematics folder contains a pdf of the schematic, as well as Altium Designer files of the schematic and board layout.
