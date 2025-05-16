# Universal IoT Hub: Microprocessor for Protocol Convergence in Smart Networks


| | |
|-|-|
|`Author` | Barbier Ileana Geneviève & Brișan Andrei-Sebastian 

## Description
 ### Purpose:

Development of a hardware-software system based on a microprocessor (ESP32 + extensions) that functions as a universal IoT gateway, capable of interconnecting and translating between various protocols: Matter, Zigbee, Z-Wave, BLE, Wi-Fi, Thread, etc.

### Objectives:
1. Design of a modular microprocessor/microcontroller architecture with support for protocol extension modules.
2. Hardware integration of modules: Zigbee (e.g., CC2652), Z-Wave (ZGM130S), Wi-Fi/BLE (ESP32), Thread (nRF52840).
3. Implementation of a software interface that:
Detects IoT devices in the network regardless of protocol, displays them in a web dashboard (hosted on the ESP), allows the creation of automation scenarios between devices across different protocols.
5. Development of a real-time monitoring WebUI or mobile app.


## Motivation
The smart home ecosystem suffers from fragmentation due to multiple communication standards (Zigbee, Z-Wave, BLE, Thread, etc.), which limits interoperability between devices. This project aims to create a single hardware hub capable of bridging these technologies through a unified interface, enabling seamless integration and smarter automation scenarios.

## Architecture

### Block diagram

<!-- Make sure the path to the picture is correct -->
![Block Diagram](https://github.com/user-attachments/assets/8cd24071-292e-4331-8f5c-5a35147cda7c)

### Schematic

![Schematic](https://github.com/user-attachments/assets/bb103c5d-e36a-4fa5-b51f-d41bafd511e8)

### Components


<!-- This is just an example, fill in with your actual components -->

| Device | Usage | Price |
|--------|--------|-------|
| ESP32-WROOM32D | Development board | [69,99 RON](https://www.optimusdigital.ro/en/wifi-boards/3053-placa-de-dezvoltare-esp32-cu-wifi-si-bluetooth.html?search_query=esp32&results=39) |
| Breadboard 750 points + 300 points + 300 points | Project boards | [8,98 RON](https://www.optimusdigital.ro/en/breadboards/13245-breadboard-750-points.html?search_query=breadboard&results=361) and 2 * [3,49RON](https://www.optimusdigital.ro/en/breadboards/13249-breadboard-300-puncte.html?search_query=breadboard&results=361)|
| Female-Female Wires| Connecting components | [6,99 RON](https://www.optimusdigital.ro/en/wires-with-connectors/652-10-cm-40p-female-female-wire.html?search_query=male+male&results=806&HTTP_REFERER=https%3A%2F%2Fwww.optimusdigital.ro%2Fen%2Fsearch%3Fcontroller%3Dsearch%26orderby%3Dposition%26orderway%3Ddesc%26search_query%3Dmale%2Bmale%26submit_search%3D) |
| Male-Female Wires| Connecting components | [5,99 RON](https://www.optimusdigital.ro/en/wires-with-connectors/653-10-cm-40p-male-to-female-wire.html?search_query=male+male+40p&results=38) |
| Male-Male Wires| Connecting components | [7,98 RON](https://www.optimusdigital.ro/en/wires-with-connectors/890-set-fire-tata-tata-40p-30-cm.html?search_query=male+male+40p&results=38) |
| 2 Pitch Male Pin Header| Soldering on nRF52840 | [1,98 RON](https://www.optimusdigital.ro/en/pin-headers/464-colored-40p-254-mm-pitch-male-pin-header-red.html?search_query=Colored+40p+2.54+mm+Pitch+Male+Pin+Header+-+Red&results=4) |
| SparkFun Pro nRF52840| Thread/BLE/Matter| [229,14 RON](https://www.robofun.ro/wireless/placa-de-dezvoltare-sparkfun-pro-nrf52840-mini-cu-bluetooth.html) |

### Libraries

<!-- This is just an example, fill in the table with your actual components -->

| Library | Description | Usage |
|---------|-------------|-------|
| [libCoAP](https://github.com/obgm/libcoap) | A CoAP (RFC 7252) implementation in C | Used in ESP-IDF on ESP32 to implement a CoAP server for communication with Thread/BLE devices (e.g., nRF52840)  |
| [ESP-IDF](https://github.com/espressif/esp-idf) | Espressif IoT Development Framework. Official development framework for Espressif SoCs. | Provides hardware abstraction, drivers, FreeRTOS, and networking support including Wi-Fi  |
| [OpenThread](https://github.com/openthread/openthread) | OpenThread released by Google is an open-source implementation of the Thread networking protocol | Enables Thread protocol support on the nRF52840  |



## Log

<!-- write every week your progress here -->

### Week 6 - 12 May
1. Finalized the component list and began sourcing hardware.
2. Planned project architecture and started block diagram design.

### Week 7 - 19 May
1. Initial testing of ESP32 dev board and Wi-Fi web server setup.
2. Breadboard layout and wiring test for ESP32 and nRF52840.

### Week 20 - 26 May


## Reference links

<!-- Fill in with appropriate links and link titles -->

[Matter over Thread with nRF52840](https://docs.nordicsemi.com/bundle/ncs-latest/page/nrf/protocols/matter/index.html)

[OpenThread by Google](https://openthread.io)

[UART, SPI, I2C Protocol basics](https://learn.sparkfun.com/tutorials/serial-communication/all)
