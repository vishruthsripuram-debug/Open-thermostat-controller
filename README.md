# Open-thermostat-controller
A small thermostat controller for split units and zones with adaptable temperatures able to be used within home assistant.

## About
The open thermostat controller is a project designed to replace my old air conditioner remote, my old air conditioner remote was extremely large, clunky and ultimately a large wastof space in my bedroom, not to mention it looked incredibly ugly. I designed my device to be small, compact and useful featuring a simple 3 button layout that simplifies the old large remote into a smaller much more elegant design that can be placed on a desk or sat next to my pillow on my bed without any worries. The actual remote itself is a low power device simply communicating over thread with home assistant, using esphome, it controls the aircon using the integration built in with home assistant. 

## Instructions
### Assembly
1. Fabricate the PCB and 3D print the case.
2. Assemble the PCB by following the instructions printed onto the silkscreen, placing the selected components on their respective pads. Or order the PCB with assembly, for self assembly, an SMD stencil is preffered.
3. Place the buttons covers onto the buttons of the PCB, and insert the PCB into the case, use the screw holes from the display and screw the PCB into place.
4. Place down the top cover and press it into place, you should hear a faint click here.
5. You're finished, now its time to flash
### Flashing
1. Plug the device into your computer using a usb c cable and download the ESPhome yaml from the repository.
2. upload the YAML and press the flash button on your screen, once the flash is completed a message will show up on the display as 'done flashing' and then configure the device in home assistant.
3. You're finished, you are now ready to use your device.

## CAD rendering
<img width="763" height="482" alt="Screenshot 2026-09-22 at 2 34 57 PM" src="https://github.com/user-attachments/assets/f13ffddb-badc-4b09-97a0-d34e35d09102" />

## PCB and schematic
<img width="413" height="666" alt="Screenshot 2026-10-01 at 11 23 04 AM" src="https://github.com/user-attachments/assets/5e1d9e9e-7e37-4928-8864-73ece27966bf" />
<img width="477" height="376" alt="Screenshot 2026-10-01 at 11 22 33 AM" src="https://github.com/user-attachments/assets/0eee29c8-80bf-4a50-8374-12141e2ce1c2" />

## Design
<img width="484" height="247" alt="Screenshot 2026-09-10 at 7 07 42 PM" src="https://github.com/user-attachments/assets/f431cad8-e1a9-41da-b487-7cef4b5ed2fa" />
<img width="497" height="251" alt="Screenshot 2026-09-10 at 7 07 46 PM" src="https://github.com/user-attachments/assets/1c24ee94-0e99-4ef4-b4e3-601def47e7bf" />

## BOM
| Ref | Qty | Value | MPN | Supplier | Unit Price (USD) | Line Total (USD) | Buy Link |
|---|---|---|---|---|---|---|---|
| J1 | 1 | Conn_01x02_Socket (JST PH 2-pin, SMD side entry) | S2B-PH-SM4-TB(LF)(SN) | Digi-Key | $0.49 | $0.49 | [Buy](https://www.digikey.com/en/products/detail/jst-sales-america-inc/S2B-PH-SM4-TB/926655) |
| SW1, SW2, SW3 | 3 | SW_Push (SMD tactile) | PTS645SM43SMTR92 LFS | Digi-Key | $0.36 | $1.08 | [Buy](https://www.digikey.com/en/products/detail/c-k/PTS645SM43SMTR92-LFS/1146840) |
| U1 | 1 | XIAO-ESP32-C6-SMD | 113991254 | Digi-Key | $5.38 | $5.38 | [Buy](https://www.digikey.com/en/products/base-product/seeed-technology-co-ltd/1597/ESP32-C6/678377) |
| U2 | 1 | ER_OLEDM0.91_1x-I2C | ER-OLEDM0.91-1W-I2C | BuyDisplay | $2.80 | $2.80 | [Buy](https://www.buydisplay.com/i2c-white-0-91-inch-oled-display-module-128x32-arduino-raspberry-pi) |
| PCB | 1 | Custom PCB | - | - | $1.80 | $1.80 | - |
| | | | | | **Total** | **$11.55** | |

## Credits
Made entirely By vishruth
AI disclosure: The code for this project was written mostly by AI but nothing else was, all cad, PCB design and research was done by me.
