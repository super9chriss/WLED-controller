# WLED controller
A ESP32 C3 based microcontroller which is made to be used with WLED to use 12V or 24V ledsttrips.
I made this project since i want to add some lighting to my wall since its very dark, i wanted to learn something from this project so i made it into a devboard instead of a simpeler PCB design.
You can attach a 12 or 24V power supply to the Vin port which will directly power the ledstrip so this needs to have the same voltage rating and you can then use the ESP32 to adress the ledstrip.
<div align="center">
  <img width="398" height="529" alt="image" src="https://github.com/user-attachments/assets/4555378d-5bb7-4ddb-8267-bbb905b79478" />
</div>

## Features

* **Microcontroller:** ESP32-C3-WROOM-02 with Wi-Fi and Bluetooth LE.
* **Power Input:** Supports 12V or 24V DC via dedicated screw terminals.
* **Logic Level Shifter:** Integrated SN74AHCT125DR to convert 3.3V logic to 5V for reliable LED data.
* **Connectivity:** USB-C receptacle for easy firmware flashing.
* **Led strip ports:** GPIO 1,3,4 and 5 are on the right side of the board(from bottom to top so top is 5 and bottom is 1) and can be used for ledstrips.
## How to use

1. Order the PCBA and lightstrip + powersupply.
2. Install WLED to the esp using https://install.wled.me/ if it doesnt work follow the steps on the website to install some drivers.
3. Configure WLED first connect the esp to wifi so you can remotly control the ledstrips, then add in the hardware setup which leds you are using, how many leds u use and on which pin the leds are connected(GPIO 1,3,4 and/or 5).
<img width="724" height="852" alt="image" src="https://github.com/user-attachments/assets/39d42956-7088-4010-9291-ce13f03111df" />

4. Disconnect the esp from your computer, and only then power it using the power supply also connect the ledstrip if you havent done this yet, and enjoy using the WLED controller.

## PCB and schematic
| **PCB Layout** | **Schematic** |
| :---: | :---: |
|<img width="631" height="833" alt="image" src="https://github.com/user-attachments/assets/119ed411-2456-4698-88f2-4330cc2fb148" /> |  <img width="1138" height="781" alt="image" src="https://github.com/user-attachments/assets/00773907-2f10-4260-8016-b3555b877f7d" />|
|<img width="630" height="830" alt="image" src="https://github.com/user-attachments/assets/197add46-af1c-42e5-811d-455a2a2342d4" />|
|<img width="629" height="834" alt="image" src="https://github.com/user-attachments/assets/de5445f0-077e-4c5c-9f63-0c2e1741de60" />|


## Wiring diagram
<img width="394" height="561" alt="image" src="https://github.com/user-attachments/assets/fb74e88c-656a-4cf5-8348-ee65d7d92e28" />

## BOM
|Component            |price|link                                                                                                                                                                                                                                                                          |
|---------------------|-----|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|ledstrip + powersuply|21.79|https://nl.aliexpress.com/item/1005007038025239.html?spm=a2g0o.cart.0.0.3f5461d7XIU4zl&mp=1&pdp_npi=6%40dis%21EUR%21EUR%2032.67%21EUR%2021.79%21%21EUR%2021.79%21%21%21%402103917f17685608530224732ebad8%2112000039180039618%21ct%21NL%21-1%21%211%210%21&gatewayAdapt=glo2nld|
|PCB                  |41.46|https://cart.jlcpcb.com/smt-order/?pcbFileNo=4c66db31f77f4dcd8bb62a3aeb8100a0                                                                                                                                                                                                 |


