# Hardware Overview

CJAM is built around an ESP32 DevKit V1 and three NRF24L01+ modules connected through a shared SPI bus.

## Main Features

- ESP32 DevKit V1
- Triple NRF24L01+
- OLED
- Status LED
- User Button

## Power

Each NRF24L01 has:

- 100µF Bulk Capacitor
- 0.1µF Ceramic Decoupling Capacitor

to improve stability during transmit bursts.

## PCB

- 2 Layer
- FR4
- Black Soldermask
- White Silkscreen