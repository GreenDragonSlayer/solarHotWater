# solarHotWater
This project is a solar hot water control system for Raspberry Pi with a "hat" for interfacing sensors. 

The project contains a 2-layer PCB design, containing 

- 1 x ATMega328P-AU MCU clocked at 8 MHz
- 4 x RTD ICs - Max31865
- 1 x RTC DS3231
- 1 x 16 but ADC for NTC, Pressure and solar power input
- 2 x Valve control outputs, 5V/230V (Fused)
- 2 x Interrupt inputs for pulse flow meter inputs
- 1 x 0-10V output for pump control
- 1 x PWM output, 3.3V for pump control
- 1 x Battery for RTC
- 2 x NTC inputs (ADC
- 1 x pressure sensor input
- 1 x Solar radiation power measurement input (Soldata pyranometer)
- 1 x 5V output for screen power (7" RPi touchscreen)
- 1 x 8 port IO expander

Communication between ATMega328P and RPi is via uart0.

The firmware is written in the Arduino framework in C/C++.

The GUI is written in Python3.x and PyQt5 and runs on the Raspberry pi
