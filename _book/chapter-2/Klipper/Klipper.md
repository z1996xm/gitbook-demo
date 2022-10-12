# 1、Klipper

## 1.1 Preparation

### 1.1.1 Download system image

Download the system image of the built-in WebUI you like. Currently, the mainstream includes Fluidd, Mainmail, etc.

Built in Fluidd system: <a href="https://github.com/fluidd-core/FluiddPI/releases" title="超链接title">https://github.com/fluidd-core/FluiddPI/releases</a>

![image-20221008112605131](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008112605131.png)

Built in Mainsail  system: <a href="https://github.com/mainsail-crew/MainsailOS/releases" title="超链接title">https://github.com/mainsail-crew/MainsailOS/releases</a>

![image-20221008113014189](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008113014189.png)

Or refer to <a href="https://www.klipper3d.org/Installation.html" title="超链接title">Klipper's official installation instructions</a> to use Octoprint

### 1.1.2 Download and install Raspberry Pi Imager

Download and install the official burning software of Raspberry Pie  <a href="https://www.raspberrypi.com/software/" title="超链接title">https://www.raspberrypi.com/software/</a> 



## 1.2 Burn Image

 1.Insert the Micro SD card reader into the computer.

 2.Select System.

​													  	![image-20221008115705299](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008115705299.png)

3. Select "User defined", and then select the image downloaded to the computer.

   ![image-20221008115807257](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008115807257.png)

   4. Select the SD card to be burned (burning the image will format the SD card. Be careful not to select the wrong drive letter, or it will

   Format data on other storage), click "Burn".

   ![image-20221008120015759](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008120015759.png)

   5. Wait for the burning to complete.

   ![image-20221008120046939](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008120046939.png)



## 1.3 Set WIFI

Note: If you use the network cable port instead of WIFI, you can skip this step

1. Reseat the card reader

2. Find the "fluiddpi-wpa-supplicant.txt" or "mainmail-wpa supplicant.txt" file in the boot disk of the SD card and open it with VSCode (do not open it with the notepad that comes with Windows)

   ![image-20221008141627368](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008141627368.png)

3. Delete the '#' character at the beginning of the four lines in the red box, and set the correct WIFI name and password before saving

![image-20221008141700263](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008141700263.png)



## 1.4 Connecting raspberry pie with ssh software

1. Install the ssh software Mobaxterm:<a href="https://mobaxterm.mobatek.net/download-home-edition.html" title="超链接title">https://mobaxterm.mobatek.net/download-home-edition.html</a> 

2. Insert the SD card into the raspberry pie, and wait for the system to start after power on, about 1-2 minutes

3. The raspberry pie will be automatically assigned an IP after it is connected to WIFI or plugged into the Internet cable

4. Enter the router management interface to find the IP address of Raspberry Pie

5. Or use <a href="https://angryip.org/" title="超链接title">https://angryip.org/</a> Tool, scan all IP addresses under the current LAN, and use the

Reorder the machine names, and find the devices whose host names are Fluidd or Mainmail, as shown in the following figure

6. Open the installed Mobaxterm software, click "Session", click "SSH" in the pop-up window, enter the IP address of raspberry pie in the Remote host column, and click "OK" (Note: computers and raspberry pie must Under the same LAN)

![image-20221008142314172](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008142314172.png)

7. Enter login as: pi login password: raspberry to enter the SSH terminal interface

![image-20221008142339959](C:\Users\admin\AppData\Roaming\Typora\typora-user-images\image-20221008142339959.png)