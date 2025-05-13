# Universal IoT Hub: Microprocesor pentru convergența protocolară în rețele inteligente

| | |
|-|-|
|`Author` | Barbier Ileana Geneviève & Brișan Andrei-Sebastian 

## Description
 # Scop:

Realizarea unui sistem hardware-software bazat pe un microprocesor (ESP32 + extensii) care funcționează ca un gateway universal IoT, capabil să interconecteze și să traducă între diferite protocoale: Matter, Zigbee, Z-Wave, BLE, Wi-Fi, Thread etc.

# Obiective:
1. Proiectarea arhitecturii unui microprocesor/microcontroler modular cu suport pentru extensii de protocoale.
2. Integrarea hardware a modulelor: Zigbee (ex: CC2652), Z-Wave (ZGM130S), Wi-Fi/BLE (ESP32), Thread (nRF52840).
3. Implementarea unei interfețe software care:
• Detectează dispozitive IoT din rețea indiferent de protocol.
• Le afișează într-un dashboard web (hostat pe ESP).
• Permite crearea de scenarii automate între dispozitive din protocoale diferite.
4. Implementarea unei aplicații mobile sau WebUI cu vizualizare în timp real.
5. Integrarea cu sisteme smart home existente (Google Home, Home Assistant, Apple HomeKit prin Matter).

## Motivation

## Architecture

### Block diagram

<!-- Make sure the path to the picture is correct -->
![Block Diagram](schematics/block_diagram.png)

### Schematic

![Schematic](schematics/kicad_schematic.png)

### Components


<!-- This is just an example, fill in with your actual components -->

| Device | Usage | Price |
|--------|--------|-------|
| ESP32-WROOM32 | Development board | [69,99 RON](https://www.optimusdigital.ro/en/wifi-boards/3053-placa-de-dezvoltare-esp32-cu-wifi-si-bluetooth.html?search_query=esp32&results=39) |
| Breadboard 750 points + 300 points | Project boards | [8,98 RON](https://www.optimusdigital.ro/en/breadboards/13245-breadboard-750-points.html?search_query=breadboard&results=361) and [3,49RON](https://www.optimusdigital.ro/en/breadboards/13249-breadboard-300-puncte.html?search_query=breadboard&results=361)|
| Female-Female Wires| Connecting components | [6,99 RON](https://www.optimusdigital.ro/en/wires-with-connectors/652-10-cm-40p-female-female-wire.html?search_query=male+male&results=806&HTTP_REFERER=https%3A%2F%2Fwww.optimusdigital.ro%2Fen%2Fsearch%3Fcontroller%3Dsearch%26orderby%3Dposition%26orderway%3Ddesc%26search_query%3Dmale%2Bmale%26submit_search%3D) |
| Male-Female Wires| Connecting components | [5,99 RON](https://www.optimusdigital.ro/en/wires-with-connectors/653-10-cm-40p-male-to-female-wire.html?search_query=male+male+40p&results=38) |
| Male-Male Wires| Connecting components | [7,98 RON](https://www.optimusdigital.ro/en/wires-with-connectors/890-set-fire-tata-tata-40p-30-cm.html?search_query=male+male+40p&results=38) |
| SparkFun Pro nRF52840 Mini cu Bluetooth | Board | [229,14 RON](https://www.robofun.ro/wireless/placa-de-dezvoltare-sparkfun-pro-nrf52840-mini-cu-bluetooth.html) |

### Libraries

<!-- This is just an example, fill in the table with your actual components -->

| Library | Description | Usage |
|---------|-------------|-------|
| [lib-name1](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |
| [lib-name2](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |

## Log

<!-- write every week your progress here -->

### Week 6 - 12 May

### Week 7 - 19 May

### Week 20 - 26 May


## Reference links

<!-- Fill in with appropriate links and link titles -->

[Tutorial 1](https://www.youtube.com/watch?v=wdgULBpRoXk&t=1s&ab_channel=BenEater)

[Article 1](https://www.explainthatstuff.com/induction-motors.html)

[Link title](https://projecthub.arduino.cc/)
