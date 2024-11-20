Download GIMP Plugin here

https://github.com/LinuxBeaver/GIMP-GEGL-PLUGIN_Stripes/releases

## Render stripe blinds with GEGL
![image](https://github.com/user-attachments/assets/b7701d64-0af9-48c4-96f9-66e02975d0e2)

## OS specific location to put GEGL Filter binaries 

**Windows**
C:\Users\USERNAME\AppData\Local\gegl-0.4\plug-ins
 
**Linux**
 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
 **Linux (Flatpak)**
 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

![image](https://github.com/LinuxBeaver/GEGL-glossy-balloon-text-styling/assets/78667207/f15fb5eb-c8d7-4c08-bbac-97048864e657)


## Compiling and Installing

For Linux run "build_plugin_linux.sh" for Windows run "build_plugin_windows.sh" for manual compiling read below.

Packages needed to compile are **ninja**, **meson**, and **GEGL**

**Linux**

To compile and install you will need the GEGL header files (libgegl-dev on Debian based distributions or gegl on Arch Linux) and meson (meson on most distributions).

meson setup --buildtype=release build
ninja -C build

**Windows**

The easiest way to compile this project on Windows is by using msys2. Download and install it from here: https://www.msys2.org/

Open a msys2 terminal with C:\msys64\mingw64.exe. Run the following to install required build dependencies:

pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl

Then build the same way you would on Linux:

meson setup --buildtype=release build
ninja -C build

## Extra preview of this based Gimp plugin

![image](https://github.com/user-attachments/assets/5ea53a72-16cf-4037-85f0-23c3cef0ede4)

![image](https://github.com/user-attachments/assets/25ff08b2-b42c-4a48-b6ca-ad8633216a09)

![image](https://github.com/user-attachments/assets/5bf51f66-eff0-4570-bf93-3c19a3961b6c)


