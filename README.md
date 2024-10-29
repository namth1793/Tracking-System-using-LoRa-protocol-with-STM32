## Welcome to my project about using LoRa technique with STM32F103C8T6.
### 1. System Diagram
![System Diagram](https://github.com/user-attachments/assets/3b5479b7-bd71-481a-8bb9-c6b3bdf52dfe)
- There are others 2 branch in my repository, they are MASTER and SLAVE.
- For the MASTER branch, I set up and develope for the transmit node, It will receive GPS signal from GPS module(Quectel L80-M39) and transmit via LoRa.
- Next, for the SLAVE branch, that also my set up but use for receive signal from MASTER node and display it in the LCD 16x2 (with i2c module).
- I using LORA library from:
  https://github.com/SMotlaq/LoRa/tree/master?fbclid=IwZXh0bgNhZW0CMTAAAR07GdoOCyXt8_d9Y_I7p44Sc2CIL0V0PH8Cm7YJXKeXMlnBAQmdb_MHYNM_aem_AY2NSFanzzq9Fuo8-GP09s07NCwS7mxoUd9qy1OV1a30vqOwYpQMlh7vMkdglJf1YBNWLOrk8lejAV5p1PG8x0Fa
- And for processing GPS signal, I using this driver:
  https://github.com/sztvka/stm32-nmea-gps-hal
- And the last one, I follow a lot of step from this page to using LCD for my project:
  https://deepbluembedded.com/stm32-i2c-lcd-library-example-16x2-20x4-multiple-lcds/
### 2. Result
### ![451491303_506287805414361_3575618958314909936_n](https://github.com/user-attachments/assets/331aae95-1e15-49c9-b3dc-a2f1c7672c9f)

### 3. PCB Design
![2bfd8527-585f-440c-946b-e17004a13dbb-removebg-preview](https://github.com/user-attachments/assets/9d25eceb-a37e-4365-b408-b2bcb5c62a9b)

## -> My project will have some update in the future, maybe I wil send data to the server and build a LoRaWan network.
  Thanks for reviewing!

