# Símbolo y footprint de KiCad para el WIZnet W6300-EVB-Pico2

> [!NOTE]
> Also available in [English](README.md).

<table>
  <tr>
    <td><img src="images/W6300-EVB-Pico2-product.webp" alt="W6300-EVB-Pico2 (en ángulo)" width="260"></td>
    <td><img src="images/W6300-EVB-Pico2-top.jpg" alt="Vista superior" width="260"></td>
  </tr>
  <tr>
    <td><img src="images/W6300-EVB-Pico2-bottom.jpg" alt="Vista inferior" width="260"></td>
    <td><img src="images/W6300-EVB-Pico2-scale.jpg" alt="Placa junto a una regla" width="260"></td>
  </tr>
</table>

Este repositorio contiene un símbolo, footprint y modelo 3D de KiCad para el [WIZnet W6300-EVB-Pico2](https://docs.wiznet.io/Product/Chip/Ethernet/W6300/w6300-evb-pico2) — una placa con RP2350 y controlador Ethernet W6300 10/100 conectado vía QSPI, en el form factor de la Raspberry Pi Pico 2 con un conector RJ45 magjack integrado en uno de los lados cortos. La placa mide 80 × 21 mm.

El símbolo de KiCad expone los 40 pines del header de la Pico 2 más los tres puntos de prueba SWD, con etiquetas combinadas (`GP18/QSPI_IO0`, `GP22/RSTn`, etc.) en los ocho pines que el W6300 ocupa internamente. El footprint es un header through-hole de 2×20 a 2.54 mm de pitch con pads keyhole castelados, de modo que el módulo se puede montar a través de un header de pines de 2.54 mm o directamente surface-mount sobre una PCB portadora.

<table>
  <tr>
    <td width="40%" align="center"><img src="images/W6300-EVB-Pico2-symbol.jpg" alt="Símbolo en KiCad" width="100%"></td>
    <td width="60%" align="center"><img src="images/W6300-EVB-Pico2-footprint.png" alt="Footprint en KiCad" width="100%"></td>
  </tr>
</table>

## Instalación

Primero, clona o descarga este repositorio.

Agrega las librerías de símbolo y footprint en KiCad:

- **Preferences → Manage Symbol Libraries…** y agrega `kicad/WIZnet_W6300-EVB-Pico2.kicad_sym`
- **Preferences → Manage Footprint Libraries…** y agrega la carpeta `kicad/WIZnet_W6300-EVB-Pico2.pretty/`

Para que el modelo 3D resuelva la ruta, define una variable de entorno en KiCad:

- **Preferences → Configure Paths…**
- Agrega una entrada con nombre `WIZNET_W6300_LIB` y valor apuntando a la carpeta `kicad/` del repositorio clonado
