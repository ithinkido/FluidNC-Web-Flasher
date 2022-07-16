<p align="center"><img src="https://raw.githubusercontent.com/ithinkido/FluidNC-Web-Flasher/main/images/FluidNC._full.svg?sanitize=true" width=100%></p>

# FluidNC Web Flash Tool
A quick and easy way of flashing your ESP32 board with[FluidNC](https://github.com/bdring/FluidNC#readme) direct from the comfort of your browser

The Web Serial API has [Limited browser support](https://developer.mozilla.org/en-US/docs/Web/API/Serial) - Basically just Chrome and Edge.  

## Flash Details.

FluidNC firmware will be flashed according to the following location table,

| Offset(hex) | Offset(decimal) | Bin Location |
| ----------- | --------------- | ------------ |
|0x1000|4096|bootloader_dio_80m.bin|
|0x8000|32768|partition.bin|
|0xe000|57344|boot_app0.bin.bin|
|0x10000|65536|firmware.bin|

## Flashing

1. Using Chrome or Edge, visit [FluidNC Web Flash Tool](https://ithinkido.github.io/FluidNC-Web-Flasher)
2. Plug your board into your computer
3. Select the firmware type you want ( WiFi or BT)
4. Click the `Install` button
5. You should be prompted to select a USB port, pick the port your device is connected to. (This step requires drivers, presumably you already have them if you are here though!)
6. It should now start flashing, when its finished you should have a flashed board!  
  
  
![visitors](https://visitor-badge.glitch.me/badge?page_id=ithinkido.FluidNC-Web-Flasher)
