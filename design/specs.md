```
 ⡇ ⡇⢹⠁⢹⠁⡇ ⣏⡉ ⢎⡑⡎⢱⡇⢸⣏⡉⣎⣱⣇⠜⢇⢸ ⡷⢾⣎⣱⡎⠑⣇⣸⡇⡷⣸⣏⡉
 ⠧⠤⠇⠸ ⠸ ⠧⠤⠧⠤ ⠢⠜⠣⠪⠣⠜⠧⠤⠇⠸⠇⠱ ⠇ ⠇⠸⠇⠸⠣⠔⠇⠸⠇⠇⠹⠧⠤
```

The Little Squeaky Machine is a hardware reference platform for the [Little Weirdo Software Synthesizer](https://github.com/hi-squeaky-things/little-weirdo). 

## LttL Squeaky Machine Hardware

### Specification and capabilities

| Name | Component | Function | 
| --- | --- | --- |
| Name        | Component           | Function                                                                                                                |
|-------------|---------------------|------------------------------------------------------------------------------------------------------------------------|
| MCU         | ESP32-S3-WROOM-1    | Running the LttL Weirdo Firmware and controlling the LttL Squeaky Machine, enabling sound generation and control through firmware.      |
| CODEC       | SGTL5000            | Providing advanced audio processing, including stereo line input, microphone input with bias, stereo line output, and a capless stereo headphone amplifier with mixing and filtering capabilities.  |
| TOUCH       | CY8CMBR3108         | Enabling capacitive touch functionality (interface through I2C) for user interaction, suitable for applications like musical instrument controls. Includes 6 touchpoints and 2 proximity sensors.     |
| MIDI        | ESP32-S3-WROOM-1    | Facilitating MIDI data transfer through TRS-A connections, enabling communication between devices such as synthesizers and controllers.                    |
| USB-MIDI    | ESP32-S3-WROOM-1    | Providing MIDI data transfer over USB-C connections, offering flexibility in connecting devices with USB-based interfaces.                   |
| POT-METER   | ESP32-S3-WROOM-1    | Enabling analog-to-digital conversion functionality for user interaction using potentiometers (4x).                                     |
| GYRO        | STK8321             | 3D gyroscope and x-y-z speed sensor (interface through I2C).                                                          |
| KEYS        | CPG151101S11    | Hotswappable tactile switches (25x).                                                                                             |
