# 二、Manta M4P Firmware Compilation

1. After ssh is connected to raspberry pie, enter at the command line：

   ```
   cd ~/klipper/
   ```

   ```
   make menuconfig
   ```

   Use the following configuration to compile the firmware (if the following options are not available, please update the Klipper firmware source code to the latest version)

   ​	*** [\*] Enable extra low-level configuration options** 

   ​	*** Micro-controller Architecture (STMicroelectronics STM32) --->** 

   ​	*** Processor model (STM32G0B1) --->** 

   ​	*** Bootloader offset (8KiB bootloader) --->** 

   ​	*** Clock Reference (8 MHz crystal) --->** 

   ​	*** Communication interface (USB (on PA11/PA12)) --->** 

   ![image-photo20](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo20.jpg)

   

2. After the configuration is selected, enter 'q' to exit the configuration interface. When asked whether to save the configuration, select "Yes"

   

3. Enter `make` to compile the firmware. When the `make` is completed, it will be displayed in the raspberry pie `home/pi/kliipper/out` file.The folder generates the  `klipper.bin`  firmware we need, which can be directly downloaded to the computer on the left side of the ssh software

   ![image-photo14](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo14.jpg)





