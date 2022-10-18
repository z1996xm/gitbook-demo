# 一、Steps to use Raspberry pi CM4

## 1.1  Download system image

Download the system image of the built-in WebUI you like. Currently, the mainstream includes Fluidd, Mainmail, etc.

Built in Fluidd system: <a href="https://github.com/fluidd-core/FluiddPI/releases" title="超链接title">https://github.com/fluidd-core/FluiddPI/releases</a>

![image-photo1](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo1.jpg)

Built in Mainsail  system: <a href="https://github.com/mainsail-crew/MainsailOS/releases" title="超链接title">https://github.com/mainsail-crew/MainsailOS/releases</a>

![image-photo2](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo2.jpg)

Or refer to <a href="https://www.klipper3d.org/Installation.html" title="超链接title">Klipper's official installation instructions</a> to use Octoprint

### 1.1.2 Download and install Raspberry Pi Imager

Download and install the official burning software of Raspberry Pie  <a href="https://www.raspberrypi.com/software/" title="超链接title">https://www.raspberrypi.com/software/</a> 



## 1.2 Burn Image

 1.Insert the Micro SD card reader into the computer.

 2.Select System.

![image-photo3](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo3.jpg) 

3. Select "User defined", and then select the image downloaded to the computer.

   ![image-photo4](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo4.jpg) 

   4. Select the SD card to be burned (burning the image will format the SD card. Be careful not to select the wrong drive letter, or it will

   Format data on other storage), click "Burn".

   ![image-photo5](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo5.jpg) 

   5. Wait for the burning to complete.

   ![image-photo6](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo6.jpg) 



## 1.3 Set WIFI

Note: If you use the network cable port instead of WIFI, you can skip this step

1. Reseat the card reader

2. Find the "fluiddpi-wpa-supplicant.txt" or "mainmail-wpa supplicant.txt" file in the boot disk of the SD card and open it with VSCode (do not open it with the notepad that comes with Windows)

   ![image-photo7](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo7.jpg)

3. Delete the '#' character at the beginning of the four lines in the red box, and set the correct WIFI name and password before saving

![image-photo8](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo8.jpg)



## 1.4 Connecting raspberry pie with ssh software

1. Install the ssh software Mobaxterm:<a href="https://mobaxterm.mobatek.net/download-home-edition.html" title="超链接title">https://mobaxterm.mobatek.net/download-home-edition.html</a> 

2. Insert the SD card into the raspberry pie, and wait for the system to start after power on, about 1-2 minutes

3. The raspberry pie will be automatically assigned an IP after it is connected to WIFI or plugged into the Internet cable

4. Enter the router management interface to find the IP address of Raspberry Pie

   ![image-photo9](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo9.jpg)

5. Or use <a href="https://angryip.org/" title="超链接title">https://angryip.org/</a> Tool, scan all IP addresses under the current LAN, and use the

   ![image-photo10](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo10.jpg)

Reorder the machine names, and find the devices whose host names are Fluidd or Mainmail, as shown in the following figure

6. Open the installed Mobaxterm software, click "Session", click "SSH" in the pop-up window, enter the IP address of raspberry pie in the Remote host column, and click "OK" (Note: computers and raspberry pie must Under the same LAN)

![image-photo11](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo11.jpg)

7. Enter login as: pi login password: raspberry to enter the SSH terminal interface

![image-photo12](https://raw.githubusercontent.com/z1996xm/gitbook-demo/master/photo/photo12.jpg)