esp32_can
==========

Implements a CAN driver for the built-in CAN hardware on an ESP32. 
The builtin CAN is called CAN0, and also CAN1 if there is a second CAN port on the ESP32 chip in use.
This library is specifically meant to be used with the EVTV ESP32-Due board. 
Primarily, one should check TX and RX pins if using a different board.

This library requires the can_common library. That library is a common base that 
other libraries can be built off of to allow a more universal API for CAN.

The needed can_common library is found here: https://github.com/collin80/can_common

ESP32 C6
Can0 - RX 10, TX 11
Can1 - RX 15, TX 23
tested with TJA1051T/3 and TJA1042T/3 on 500 kbit/s
![esp32_c6_connection](https://github.com/user-attachments/assets/6ba087ff-68de-4f4c-8bb7-06cab5833249)
