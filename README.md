# WLED-Controller
An all-in-one controller for WS2812B LED strips, made for WLED. With Adapters for LEDs everywhere.

I made this because these WS2812B strips and WLED look so good, but all the other WLED controllers are quite expensive, and I would rather make it by myself. I set out to make it as small as possible, even if that means making it harder for me.

On the controller PCB, I integrated basically a esp32 c3 supermini. That is the bulk of it, but I also put some capacitors on the LED PWR line for smoothing the power out. I also added a P-channel MOSFET to allow for a soft start.

The various adapter PCBs adapt the specified port into 5v and GND and output it to a USB-C, inspired by Framework's modules

### Images:
![](https://github.com/Choccy-vr/WLED-Controller/blob/main/images/USB-WLED-Controller.png)
#### Schematic
![](https://github.com/Choccy-vr/WLED-Controller/blob/main/images/PCB-Schematic.png)
#### Adapters
##### SATA Adapter
![](https://github.com/Choccy-vr/WLED-Controller/blob/main/images/Sata_Adapter.png)
##### Barrel Jack Adapter
![](https://github.com/Choccy-vr/WLED-Controller/blob/main/images/Barrel_Adapter.png)

### BOM
|Product Name      |Product Description     |Product Link                                                                                          |Product unit price|Product amount|Product Cost|Total (Before Tax + Shipping)|Total |
|------------------|------------------------|------------------------------------------------------------------------------------------------------|------------------|--------------|------------|-----------------------------|------|
|Main PCB(A)       |The main control PCB    |https://jlcpcb.com/                                                                                   |$8.71             |5             |$35.45      |$59.27                       |$67.38|
|Sata Adapter PCB  |Sata adapter            |https://jlcpcb.com/                                                                                   |$1.02             |5             |$5.10       |                             |      |
|Barrel Adapter PCB|Barrel adapter          |https://jlcpcb.com/                                                                                   |$1.02             |5             |$5.10       |                             |      |
|Antenna           |Antenna                 |https://www.digikey.com/en/products/detail/pulse-electronics/ANT3216A063R2400A/3927186                |$0.22             |1             |$0.22       |                             |      |
|Bulk Cap          |Cap for LEDs            |https://www.digikey.com/en/products/detail/rubycon/35PX470MEFC10X12-5/3134236                         |$0.34             |10            |$3.44       |                             |      |
|Sata Connector    |Connector for SATA PCB  |https://www.digikey.com/en/products/detail/amphenol-cs-fci/10034814-001LF/1001349                     |$6.84             |1             |$6.84       |                             |      |
|USB-C             |Male USB C              |https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/UP20-C-F-G-FL-P12-TR/24818610|$1.30             |2             |$2.60       |                             |      |
|Barrel Jack       |Connector for Barrel PCB|https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/PJ-002A/96962                |$0.52             |1             |$0.52       |                             |      |

