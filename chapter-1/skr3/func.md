# 2.SKR-3 Firmware Compilation

1. After ssh is connected to raspberry pie, enter at the command line：

​	 <code>cd ~/klipper/</code>.

​	 <code>make menuconfig</code>.

​	*** [\*] Enable extra low-level configuration options** 

​	*** Micro-controller Architecture (STMicroelectronics STM32) --->** 

​	*** Processor model (STM32H743) --->** 

​	*** Bootloader offset (128KB bootloader (SKR SE BX v2.0)) --->** 

​	*** Clock Reference (25 MHz crystal) --->** 

​	*** Communication interface (USB (on PA11/PA12)) --->** 

![test](C:\Users\admin\Desktop\test.jpg)

2. After the configuration is selected, enter 'q' to exit the configuration interface. When asked whether to save the configuration, select "Yes"

   

3. Enter make to compile the firmware. When the make is completed, it will be displayed in the raspberry pie home/pi/kliipper/out file.The folder generates the ` klipper we need Bin ` firmware, which can be directly downloaded to the computer on the left side of the ssh software

   ![1664439270(1)](C:\Users\admin\Desktop\1664439270(1).jpg)

   

4. Replace klipper Rename bin as "firmware. bin", and copy it to the SD card to update the firmware

   

5. 在命令行输入： <code>ls /dev/serial/by-id/</code>.Query the ID of the motherboard to confirm whether the firmware is successfully burned,If the burning is successful, a klipper device ID will be returned, as shown in the following figure

![image-20221006155403451](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221006155403451.png)

​		Copy and save this ID, which needs to be set in the configuration file



