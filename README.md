# Custom 87 key Mechanical Keybord
This is a custom-designed 80% mechanical keyboard built around the Raspberry Pi Pico RP2040 microcontroller. The project combines a custom PCB, individually soldered mechanical switches, an OLED display, and a rotary encoder into a compact keyboard designed for everyday typing and customization. 

# Features 
- **87 key layout**: A compact layout that retains the function row, arrow keys, and navigation clusters.
- **Custom PCB**: A purpose-designed printed circuit board for the keyboard matrix and peripherals.
- **Direct-solder switches**: MX-compatible mechanical switches soldered directly to the PCB, without hot-swap pockets.
- **RP2040 controller**: A raspberry Pi Pico handles keyboard input and peripheral communication.
- **OLED Display**: A small I2C display for keyboard status and custom information.
- **Rotary encoder**: Provides rotary input and a push-button control.
- **Custom enclosure**: A case and plate designed to support and protect the assembly.

# Hardware architecture 
The Raspberry Pi Pico RP2040 scans a keyboard switch matrix. Each key uses a mechanical switch and a 1N418 diode to help prevent unintended electrical interactions when multiple keys are pressed. 

The OLED communications with a controller over I2C. The rotary encoder provides rotational input and a push-button signal. Firmware interprets these inputs and translates key presses into keyboard reports sent to the host computer over USB. 

# Firmware
The firmware will run on the Raspberry Pi Pico RP2040 and provide: 
- Keyboard matrix scanning.
- USB keyboard input reporting.
- OLED communication over I2C.
- Rotary encoder and push-button handling.

The firmware framework and keymap will be documented here once finalized. 

# Assembly
1. Inspect the fabricated PCB for manufacturing defects.
2. Solder the diodes in the correct orientation.
3. Solder the mechanical switches directly to the PCB.
4. Install the Raspberry Pi Pico and peripheral connections according to the finalized design.
5. Connect the OLED and rotary encoder.
6. Fit the stabilizers, keycaps, plate, and case.
7. Flash the firmware and test every key and peripheral.
8. Verify USB connectivity and check for unintended key presses.

# Project pictures
**PCB design** 

A photo will be added here 

**Schematic** 

A photo will be added here 

**3D case**

A photo will be added here 

**Complete physical build** 

A photo will be added here
