# stlink_v2_iso
🔌 ST-Link V2 ISO (Type-C, Dual Isolation, External Power)

This project is an isolated version of the ST-Link V2 based on the STM32F103CBT6 microcontroller, designed for safe programming and debugging of STM32 and other ARM-compatible MCUs.

Its main feature is the use of two galvanic isolation barriers and the ability to power the target device directly from the programmer via USB Type-C.

<img width="1487" height="535" alt="image" src="https://github.com/user-attachments/assets/81999217-abae-48c7-a4ad-bbc69a818d5d" />

⚙️ Key Features

MCU: STM32F103CBT6 (ST-Link core)
Connector: USB Type-C
Isolation:
  MAX14850AEE+ – digital isolation of SWD signals (T_SWCLK, T_SWDIO, T_NRST, T_SWO)
  ADUM3160 – USB 2.0 Full-Speed isolation between PC and programmer
Protection:
  SRV05-4 – ESD/TVS protection for USB lines
  Short-circuit and overload protection
Power Supply:
  Ability to power the target board directly from the programmer
  Output voltage for target: 3.3V (up to 200–300 mA)
  
🚀 Highlights
  Full USB isolation → the PC is completely protected from possible voltage spikes on the target side
  SWD/UART isolation → safe debugging even in high-voltage or industrial environments
  Target power supply directly from the programmer (convenient for small boards)
  Supported interfaces: SWD, SWO, UART (via isolated channels)
  Full compatibility with STM32CubeProgrammer, OpenOCD, Keil, IAR

📦 Applications
Safe debugging of STM32 microcontrollers
Use in circuits with different voltage domains
Protected connection to industrial devices
Powering and programming small target boards through a single USB Type-C cable
