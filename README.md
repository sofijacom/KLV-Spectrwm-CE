# KLV-Spectrwm-CE

- KLV-Spectrwm-CE-1.0 Using PulseAudi0

![2023-11-01_750x422-thumb](https://github.com/sofijacom/KLV-Spectrwm-CE/assets/107557749/df55842b-549f-497f-a786-b03bbb1cb1ac)

##
- KLV-Spectrwm-CE-2.0 Using PipeWire

![2023-10-31_750x422-thumb](https://github.com/sofijacom/KLV-Spectrwm-CE/assets/107557749/608696ec-86f9-4126-ac12-ae0443bdca43)


# Assembly of KLV-Spectrwm-CE

1) Create a folder `KLV-Spectrwm-CE` typing in the terminal `mkdir -p KLV-Spectrwm-CE`

2) Open a terminal in the created folder `KLV-Spectrwm-CE` or go to the folder by typing in the terminal

   - `cd KLV-Spectrwm-CE`

3) Place the build script  `FR_minimal_void_spectrwm_CE_2.sh` in the created folder.
   
4) Make it executable.`chmod +x FR_minimal_void_spectrwm_CE_2.sh`

5) Enter in terminal `./FR_minimal_void_spectrwm_CE_2.sh`

6) Wait for the build to finish.

7) After the build is complete to package `07firstrib_rootfs` into `07KLV-Spectrwm-CE-x.x.sfs` where x.x is your build number.

8) Type in terminal.

```
mksquashfs 07firstrib_rootfs 07 KLV-Spectrwm-CE-x.x.sfs -noappend -comp xz -b 512k
```
  - where x.x is your build number.

9) Delete the `07firstrib_rootfs` folder.

##

FirstRib-KLA build script. 

```
./FR_minimal_void_spectrwm_CE_2.sh
```
FirstRib-KLA build script PLUG file.

Example of using a .plug file:

```
./build_firstrib_rootfs.sh void default amd64 f_00_Void_KLV_spectrwm_no-kernel.plug
```

***f_00_Void_KLV_spectrwm_no-kernel.plug***  builds a  ***(root filesystem)***  for the Void Linux-based Spectrwm desktop operating system, similar to **KLV-Spectrwm**.

To create a complete distribution, all other utilities, tools and configurations are downloaded from a centralized repository and installed as a .tar.gz file.
