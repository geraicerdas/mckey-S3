### Repository Content
* **/firmware** : Arduino codes (.ino)
* **/hardware** : Schematic (.pdf)
* **/production** : gerber file for pcb manufacturing (.zip)

You can purchase this product from [![Generic badge](https://img.shields.io/badge/Indonesia-Tokopedia-<COLOR>.svg)](https://www.tokopedia.com/geraicerdas/mckey-s3-makey-makey-w-esp32-s3-scratch-compatible-wireless-keyboard-dengan-header-88351) 
[![Generic badge](https://img.shields.io/badge/Worldwide-Tindie-blue)](https://www.tindie.com/products/geraicerdas/cerdas-uwb-tracker/)

# McKey-S3
Makey Makey ESP32-S3 Version. This project is a rework of original design of Makey Makey board published by **[Sparkfun in this archived repo](https://github.com/sparkfun/MaKeyMaKey)**

Using the McKey-S3 you can make anything into a key (get it?) just by connecting a few alligator clips. The McKey-S3 is an invention kit that tricks your computer into thinking that almost anything is a keyboard. This allows you to hook up all kinds of fun things as an input.

The McKey-S3 uses high resistance switching to detect when you've made a connection even through materials that aren't very conductive (like leaves, pasta or people). This technique attracts noise on the input, so a moving window averager is used to lowpass the noise. Instead using ATMega32u4, we use ESP32-S3 to communicates with your computer using the Human Interface Device (HID) protocol which means that it can act like a keyboard or mouse. 

You can use both USB connection and BLE connection in just one board. Please keep in mind to push GPIO0 button 3 times to switch the connection.

<p float="left">
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/11/27/fae8f0bc-fc4c-481d-b03c-79a37490d833.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/11/27/cf09b666-48f8-47da-8387-0f948930cf40.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/11/27/4bb9865b-8d9b-4791-9afb-7f83494ce0e5.jpg" width=805 />
</p>

## How To Use
The most simple way you can do is uses your fingers. Connect the McKey-S3 to your computer using USB type C cable. Your computer will automatically detect it as ESP32-S3 HID. Now try touching the Earth bar while simultaneously touching the space circle pad. The LED above the SPACE key should light up, and a space command should be sent to your computer.

To make your custom key with the McKey-S3 you need the following:
- A connection to a McKey-S3 input. This can be done using alligator clips on the top side, or jumper wires on the bottom.
- Connection to a McKey-S3 ground (Earth). Again, you'll connect to earth using either alligator clips or jumper wires.
- Some sort of key material. This is the fun/creative part! There's a world of McKey-S3 keys out there. Anything that's even slightly conductive is just waiting to become a computer input. The classics, of course, are your fingers, bananas, and pencil scratchings.
- Something to activate the key, by connecting between the key material and the ground input. Your fingers work pretty well for this. Anything even slightly conductive will do though.

## Development logs
V2.3
- Changed indicator LEDs (BLE and USB)
V2.2
- Added battery charging circuit
V2.1
- Changed PCB Color to Red
V1.0
- Initial design

## PCB and Parts
If you want to make the hardware yourself, just download the gerber file in production folder. Send it to your fav pcb manufacturer. And dont forget to get the Bill of materials :

## License
*We invests time and resources providing this open-source hardware, please support us by purchasing our products.*

*Designed by **[Insan Sains](https://www.youtube.com/insansains)** for **[Gerai Cerdas](https://geraicerdas.com)**, with contributions from the open source community. Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional information.*


