# 一、Manta M4P pin definition

<table>
   <tr>
   <td>Peripheral</td><td>Function</td><td>Pin name</td><td>Pin No.</td><td>Comment</td></tr>
   <tr>
   <td rowspan="4">Motor-1</td>
   <td>STEP</td><td>PC6</td><td>38</td><td rowspan="16">All the GPIO related to stepper are converted to 5V output to driver (including STEP, DIR, EN, CS/UART, TMC SPI)</td>
   <tr>
   <td>DIR</td><td>PA14</td><td>46</td></tr>
   <tr>
   <td>EN</td><td>PC7</td><td>39</td></tr>
   <tr>
   <td>CS/UART</td><td>PB12</td><td>32</td></tr>
   <tr>
   <td rowspan="4">Motor-2</td>
   <td>STEP</td><td>PB10</td><td>30</td></tr>
   <tr>
   <td>DIR</td><td>PB2</td><td>29</td></tr>
   <tr>
   <td>EN</td><td>PB11</td><td>31</td></tr>
   <tr>
   <td>CS/UART</td><td>PC10</td><td>64</td></tr>
   <tr>
   <td rowspan="4">Motor-3</td>
   <td>STEP</td><td>PB0</td><td>27</td></tr>
   <tr>
   <td>DIR</td><td>PC5</td><td>26</td></tr>
   <tr>
   <td>EN</td><td>PB1</td><td>28</td></tr>
   <tr>
   <td>CS/UART</td><td>PC9</td><td>49</td></tr>
   <tr>
   <td rowspan="4">Motor-4</td>
   <td>STEP</td><td>PB3</td><td>57</td></tr>
   <tr>
   <td>DIR</td><td>PB4</td><td>58</td></tr>
   <tr>
   <td>EN</td><td>PD5</td><td>55</td></tr>
   <tr>
   <td>CS/UART</td><td>PA13</td><td>45</td></tr>
   <tr>
   <td rowspan="3">TMC SPI (spi1)</td>
   <td>MISO</td><td>PB14</td><td>34</td><td rowspan="3">LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td>
   <tr>
   <td>MOSI</td><td>PB15</td><td>35</td></tr>
   <tr>
   <td>SCK</td><td>PB13</td><td>33</td></tr>
   <tr>
   <td rowspan="2">Heater</td>
   <td>E0</td><td>PD8</td><td>40</td><td rowspan="2">is converted to 5V to MOSFET with flyback protection</td>
   <tr>
   <td>HB(heated bed)</td><td>PC8</td><td>48</td></tr>
   <tr> <td rowspan="2">Temperature</td>
   <td>TH0</td><td>PA0</td><td>17</td><td rowspan="1">4.7KOhm 0.1% pull up resistor for NTC100K,etc. 2.2KOhm 0.1% pull up resistor for PT1000 by jumper. with thermistor protection circuit</td>
   <tr>
   <td>THB</td><td>PC4</td><td>25</td><td>with thermistor protection circuit</td></tr>
   <tr><td rowspan="4">Endstop</td>
   <td>M1-STOP</td><td>PC0</td><td>13</td><td rowspan="4">Share with M*-DIAG, And high level exceeding 5V are clamped to 5V by diodes</td>
   <tr>
   <td>M2-STOP</td><td>PC1</td><td>14</td></tr>
   <tr>
   <td>M3-STOP</td><td>PC2</td><td>15</td></tr>
   <tr>
   <td>M4-STOP</td><td>PC15</td><td>5</td></tr>
   <tr>
   <td rowspan="3">2 wire FAN</td>
   <td>FAN0</td><td>PD2</td><td>52</td><td rowspan="3">is converted to 5V to MOSFET with flyback protection</td>
   <tr>
   <td>FAN1</td><td>PD3</td><td>53</td></tr>
   <tr>
   <td>FAN2</td><td>PD4</td><td>54</td></tr>
   <tr>
   <td rowspan="3">Misc</td>
   <td>RGB1(Neopixel/WS2812)</td><td>PD0</td><td>50</td><td rowspan="2">is converted to 5V</td>
   <tr>
   <td>RGB2(Neopixel/WS2812)</td><td>PD1</td><td>51</td></tr>
   <tr>
   <td>PS-ON</td><td>PC13</td><td>3</td></tr>
   <tr>
   <td rowspan="2">BLTouch</td>
   <td>SERVOS</td><td>PA1</td><td>18</td><td></td></tr>
   <tr>
   <td>PROBE</td><td>PC14</td><td>4</td><td></td></tr>
   <tr>
   <tr><td rowspan="2">USB-Device</td>
   <td>OTG_FS_DM</td><td>PA11</td><td>43</td><td></td></tr>
   <tr>
   <td>OTG_FS_DP</td><td>PA12</td><td>44</td><td></td></tr>
   <tr>
   <tr><td rowspan="18">LCD-FPC(EXP1 + EXP2)</td>
   <td>5V</td><td>5V</td><td></td><td>EXP1_10</td></tr>
   <tr>
   <td>GND</td><td>GND</td><td></td><td>EXP1_9</td></tr>
   <tr>
   <td>LCD_D7</td><td>PB5</td><td>59</td><td>EXP1_8</td></tr>
   <tr>
   <td>LCD_D6</td><td>PA9</td><td>37</td><td>EXP1_7</td></tr>
   <tr>
   <td>LCD_D5</td><td>PA10</td><td>42</td><td>EXP1_6</td></tr>
   <tr>
   <td>LCD_D4</td><td>PA15</td><td>47</td><td>EXP1_5</td></tr>
   <tr>
   <td>LCD_RS</td><td>PC3</td><td>16</td><td>EXP1_4</td></tr>
   <tr>
   <td>LCD_EN</td><td>PB9</td><td>63</td><td>EXP1_3</td></tr>
   <tr>
   <td>BTN_ENC</td><td>PB8</td><td>62</td><td>EXP1_2</td></tr>
   <tr>
   <td>BEEPER</td><td>PD6</td><td>56</td><td>EXP1_1</td></tr>
   <tr>
   <td>RESET</td><td>RESET</td><td>17</td><td>EXP2_8</td></tr>
   <tr>
   <td>SD_DETECT</td><td>PC13</td><td>3</td><td>EXP2_7</td></tr>
   <tr>
   <td>MOSI</td><td>PB15</td><td>35</td><td>EXP2_6. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td>BTN_EN2</td><td>PC12</td><td>2</td><td>EXP2_5</td></tr>
   <tr>
   <td>SD_CS</td><td>PA8</td><td>36</td><td>EXP2_4</td></tr>
   <tr>
   <td>BTN_EN1</td><td>PC11</td><td>1</td><td>EXP2_3</td></tr>
   <tr>
   <td>SCK</td><td>PB13</td><td>33</td><td>EXP2_2. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td>MISO</td><td>PB14</td><td>34</td><td>EXP2_1. LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI4, and is converted to 5V to TMC driver</td></tr>
   <tr>
   <td rowspan="4">Expansion SPI pin header(spi1)</td>
   <td>SPI1-CS</td><td>PB15</td><td>54</td><td></td></tr>
   <tr>
   <td>MISO</td><td>PA6</td><td>31</td><td rowspan="3">LCD-FPC SPI, Onboard SD card, expansion SPI pin header and TMC driver SPI, 4 features multiplexing the same hardware SPI1, and is converted to 5V to TMC driver</td>
   <tr>
   <td>MOSI</td><td>PA7</td><td>32</td></tr>
   <tr>
   <td>SCK</td><td>PA5</td><td>30</td></tr>
   <tr>
</table>

