# Sprint1

FPGA implementation by james10952001 of [Sprint One](https://github.com/james10952001/Sprint1 "Sprint One") arcade game released by Kee Games in 1978
Port to MiSTer by Alan Steremberg

The original Sprint game had a steering wheel with a quadrature encoder. This version implements a converter from the digital joystick inputs.

In this version the gear number is displayed below the track. This is because on MiSTer there is no physical gearshifter control.


# Keyboard inputs :
```
   F1          : Coin + Start 1P
   F2          : Coin + Start 2P
   LEFT,RIGHT arrows : Steering

   MAME/IPAC/JPAC Style Keyboard inputs:
     5           : Coin 1
     6           : Coin 2
     1           : Start 1 Player
     2           : Start 2 Players
     D,G         : Player 2 Movements
   

 Joystick support. (Converts the digital joystick to a simulated quadrature encoding)
```
 
# ROMs
```
                                *** Attention ***

ROM is not included. In order to use this arcade, you need to provide a correct ROM file.

Find this zip file somewhere. You need to find the file exactly as required.
Do not rename other zip files even if they also represent the same game - they are not compatible!
The name of zip is taken from M.A.M.E. project, so you can get more info about
hashes and contained files there.

To generate the ROM using Windows:
1) Copy the zip into "releases" directory
2) Execute bat file - it will show the name of zip file containing required files.
3) Put required zip into the same directory and execute the bat again.
4) If everything will go without errors or warnings, then you will get the a.*.rom file.
5) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using Linux/MacOS:
1) Copy the zip into "releases" directory
2) Execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file

To generate the ROM using MiSTer:
1) scp "releases" directory along with the zip file onto MiSTer:/media/fat/
2) Using OSD execute build_rom.sh
3) Copy generated a.*.rom into root of SD card along with the Arcade-*.rbf file
```
