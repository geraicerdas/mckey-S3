### Repository Content
* **/firmware** : Arduino codes (.ino)
* **/hardware** : Schematic (.pdf)
* **/production** : gerber file for pcb manufacturing (.zip)

You can purchase this product from [![Generic badge](https://img.shields.io/badge/Indonesia-Tokopedia-<COLOR>.svg)](https://www.tokopedia.com/geraicerdas/mcplay-esp32-s2-makey-makey-custom-keyboard-mouse-scratch-compatible) 
[![Generic badge](https://img.shields.io/badge/Worldwide-Tindie-blue)](https://www.tindie.com/products/geraicerdas/cerdas-uwb-tracker/)

# mcplay
Makey Makey ESP32-S2 Version. This project is a rework of original design of Makey Makey board published by **[Sparkfun in this archived repo](https://github.com/sparkfun/MaKeyMaKey)**

Using the McPlay you can make anything into a key (get it?) just by connecting a few alligator clips. The McPlay is an invention kit that tricks your computer into thinking that almost anything is a keyboard. This allows you to hook up all kinds of fun things as an input.

The McPlay uses high resistance switching to detect when you've made a connection even through materials that aren't very conductive (like leaves, pasta or people). This technique attracts noise on the input, so a moving window averager is used to lowpass the noise. Instead using ATMega32u4, we use ESP32-S2 to communicates with your computer using the Human Interface Device (HID) protocol which means that it can act like a keyboard or mouse

<p float="left">
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/10/12/2cee952d-3018-4e5c-8a98-41ad8f05983e.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/10/12/0c145037-4c96-4122-a3d1-89af59041956.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/10/12/73f26814-8958-4a15-86ab-d3017e742ad2.jpg" width=805 />
</p>

## How To Use
The most simple way you can do is uses your fingers. Connect the McPlay to your computer using USB type C cable. Your computer will automatically detect it as ESP32 S2 HID. Now try touching the Earth bar while simultaneously touching the space circle pad. The LED above the SPACE key should light up, and a space command should be sent to your computer.

To make your custom key with the McPlay you need the following:
- A connection to a McPlay input. This can be done using alligator clips on the top side, or jumper wires on the bottom.
- Connection to a McPlay ground (Earth). Again, you'll connect to earth using either alligator clips or jumper wires.
- Some sort of key material. This is the fun/creative part! There's a world of McPlay keys out there. Anything that's even slightly conductive is just waiting to become a computer input. The classics, of course, are your fingers, bananas, and pencil scratchings.
- Something to activate the key, by connecting between the key material and the ground input. Your fingers work pretty well for this. Anything even slightly conductive will do though.

## Development logs
V1.0
- Initial design

## PCB and Parts
If you want to make the hardware yourself, just download the gerber file in production folder. Send it to your fav pcb manufacturer. And dont forget to get the Bill of materials :

## License
*We invests time and resources providing this open-source hardware, please support us by purchasing our products.*

*Designed by **[Insan Sains](https://www.youtube.com/insansains)** for **[Gerai Cerdas](https://geraicerdas.com)**, with contributions from the open source community. Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional information.*


