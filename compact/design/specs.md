```
 ⡇ ⡇⢹⠁⢹⠁⡇ ⣏⡉ ⢎⡑⡎⢱⡇⢸⣏⡉⣎⣱⣇⠜⢇⢸ ⡷⢾⣎⣱⡎⠑⣇⣸⡇⡷⣸⣏⡉
 ⠧⠤⠇⠸ ⠸ ⠧⠤⠧⠤ ⠢⠜⠣⠪⠣⠜⠧⠤⠇⠸⠇⠱ ⠇ ⠇⠸⠇⠸⠣⠔⠇⠸⠇⠇⠹⠧⠤
```

The Little Squeaky Machine is a hardware reference platform for the [Little Weirdo Software Synthesizer](https://github.com/hi-squeaky-things/little-weirdo). 

## LttL Squeaky Machine Hardware

### Specification and capabilities

| Name | Component | Function | 
| --- | --- | --- |
| MCU | ESP32-S3-WROOM-1 |  Running the LttL Weirdo Firmware and controlling the LttL Squeaky Machine, enabling sound generation and control through firmware. |
| CODEC | SPGL5000 | Providing advanced audio processing, including stereo line input, microphone input with bias, stereo line output, and a capless stereo headphone amplifier with mixing and filtering capabilities.|
| TOUCH | ESP32-S3-WROOM-1  | Enabling capacitive touch functionality for user interaction, suitable for applications like musical instrument controls. (matrix of 4x4 (16) + 2 = 18 touch points) |
| MIDI | ESP32-S3-WROOM-1 | Facilitating MIDI data transfer through TRS-A connections, enabling communication between devices like synthesizers and controllers. |
| USB-MIDI | ESP32-S3-WROOM-1 | Providing MIDI data transfer over USB-C connections, offering flexibility in connecting devices with USB-based interfaces. |
| POT-METER | ESP32-S3-WROOM-1 | Enabling analog-to-digital conversion functionality for user interaction using potential meters. | 

