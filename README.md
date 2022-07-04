# Esp32 Dev Module Hardware Boards
This repository contains hardware and circuit board designs to simplify esp32 Dev Module peripheral device connectivity

I think that I have about average circuit board design and soldering skills for an (older) mechanical engineer. As currently, mostly a hobbiest developer, I tend to develop reusable functionality focused circuit boards as opposed to project specific circuit boards. My soldering skills are OK for 0.1 inch center parts. 0805 surface mount parts are at or beyond my limit.

I am sharing these eagle board designs that I have found to be useful; mostly as a sort of tidy bridge between a breadboard and a project specific design. Unless otherwise specified, they are for (30 pin) esp32 Dev Module boards.

## Esp32 Dev Module Pins
This design consists of two 15 pin pin headers; ESP32-LEFT and ESP32-RIGHT, with wires and labels corresponding to pin functionality. They are not 'connected' to one-another and are generally intended to be used as a quick start in laying out a board for one or the other side of an esp32 Dev Module. 

## ESP32 Lcd 3.5 Connectors
This design connects one side of an esp32 Dev Module (ESP32-LEFT) to a LCD touch screen display. The display uses all of the GPIOs on that side except two. A four pin connector supports connecting the display mounted SD socket using a shared SPI. The two unused ports are routed to a four pin I2C connector. 

Used with display http://www.lcdwiki.com/3.5inch_SPI_Module_ILI9488_SKU:MSP3520

## ESP32 I/O Adapter
This design connects the right side of an esp32 Dev Module to JST ZH 1.5mm keyed connectors. The connectors include
1. 1 each 2 pin GS connector (switch)
2. 3 each 3 pin GVS connectors (potentiomer, servo motor, etc)
3. 1 each 4 pin GVSS connector (serial port)
4. 2 each 5 pin GVSSS connectors (thumb joystick)

## ESP32 Audio / Relay Adapter
This design connects the right side of an esp32 Dev Module to a three channel relay board and a CD4066 based analog switch. Two channels of the CD4066 are connected to 3.5mm TRS (input / output) audio connectors, and the other two are available on a pair of 0.1 in center 3 pin headers.
