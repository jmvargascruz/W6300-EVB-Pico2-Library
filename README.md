# KiCad Symbol and Footprint for the WIZnet W6300-EVB-Pico2

<img src="https://docs.wiznet.io/assets/images/w6300-evb-pico2-docs-836e9b64e0fb9d8b5365a435caa7f892.png" alt="WIZnet W6300-EVB-Pico2" width="600">

This repository contains a KiCad symbol, footprint and 3D model for the [WIZnet W6300-EVB-Pico2](https://docs.wiznet.io/Product/Chip/Ethernet/W6300/w6300-evb-pico2) — an RP2350 board with the W6300 10/100 Ethernet controller wired over QSPI, packaged in the Raspberry Pi Pico 2 form factor and extended on one short edge with an integrated RJ45 magjack.

## Installing this library

First, clone or download this repository.

Add the symbol and footprint libraries to KiCad:

- **Preferences → Manage Symbol Libraries…** and add `kicad/WIZnet_W6300-EVB-Pico2.kicad_sym`
- **Preferences → Manage Footprint Libraries…** and add the `kicad/WIZnet_W6300-EVB-Pico2.pretty/` folder

So that the 3D model resolves, define a path variable in KiCad:

- **Preferences → Configure Paths…**
- Add an entry with name `WIZNET_W6300_LIB` and value pointing to the `kicad/` folder of the cloned repository
