```
 ⡇ ⡇⢹⠁⢹⠁⡇ ⣏⡉ ⢎⡑⡎⢱⡇⢸⣏⡉⣎⣱⣇⠜⢇⢸ ⡷⢾⣎⣱⡎⠑⣇⣸⡇⡷⣸⣏⡉
 ⠧⠤⠇⠸ ⠸ ⠧⠤⠧⠤ ⠢⠜⠣⠪⠣⠜⠧⠤⠇⠸⠇⠱ ⠇ ⠇⠸⠇⠸⠣⠔⠇⠸⠇⠇⠹⠧⠤
```

The Little Squeaky Machine is a hardware reference platform for the [Little Weirdo Software Synthesizer](https://github.com/hi-squeaky-things/little-weirdo). 

## Little Squeaky Machine Hardware

### Pin layout of the MCU

| Pin ESP32-S3-WROOM-1 | Pin ESP32S3 | Function ESP32S3 | Function |
| --- | --- | --- | --- |
| 03 | 03 | EN | Chip Reset |
| 04 | 04 | GPIO | 🫳 Keypad row 1 |
| 05 | 05 | GPIO | 🫳 Keypad row 2 |
| 06 | 06 | GPIO | 🫳 Keypad row 3 |
| 07 | 07 | GPIO | 🫳 Keypad row 4 |
| 08 | 15 | GPIO | 🫳 Keypad row 4 |
| 09 | 16 |  ADC2_CH5 | 🎛️ Potmeter 2 |
| 10 | 17 |  U1TXD  | 🎹 MIDI out |
| 11 | 18 |  U1RXD | 🎹 MIDI in |
| 12 | 08 |  NC | Not connected |
| 13 | 19 |  USB_D- | 💻 USB-OTG / 🎹 USB-MIDI |
| 14 | 20 |  USB_D+ | 💻 USB-OTG / 🎹 USB-MIDI |
|  |
| 15 | 03 | ADC1_CH2 | 🎛️ Potmeter 1 |
| 16 | 47 | NC | Not connected |
| 17 | 09 | NC | Not connected |
| 18 | 10 | GPIO | 🫳 Keypad column 5 |
| 19 | 11 | GPIO | 🫳 Keypad column 4 |
| 20 | 12 | GPIO | 🫳 Keypad column 3 |
| 21 | 13 | GPIO | 🫳 Keypad column 2 |
| 22 | 14 | GPIO | 🫳 Keypad column 1 |
| 23 | 21 | RMT | 💡 Led controller |
| 24 | 47 | I2C_0_SDA | I2C controller data / 📺 OLED / 🔈 CODEC  |
| 25 | 48 | I2C_1_SDL | I2C controller clock / 📺 OLED / 🔈 CODEC |
| 26 | 45 |  NC | Not connected |
|  | 
| 27 | 0 | GPIO | Chip Boot |
| 28 | 35 | NC | Not connected |
| 29 | 36 | NC | Not connected |
| 30 | 37 | NC | Not connected |
| 31 | 38 | I2S_0_DIN | 🔈 I2S controller, data IN (DIN) / 🔈 CODEC |
| 32 | 39 | I2S_0_DOUT | 🎤 I2S controller, data OUT (DOUT) / 🔈 CODEC |
| 33 | 40 | I2S_0_BLCK | I2S controller, block select (BLCK) / 🔈 CODEC |
| 34 | 41 | I2S_0_WS | I2S controller, word select (LRCLK) / 🔈 CODEC |
| 35 | 42 | I2S_0_MLCK | I2S controller, master clock (MLCK) / 🔈 CODEC|
| 36 | 44 | U0RXD | Firmware TX / Serial Debug |
| 37 | 43 | U0TXD| Firmware RX / Serial Debug |
| 38 | 02 |  ADC1_CH1  | 🎛️ Potmeter 4 |
| 39 | 01 |  ADC1_CH0 | 🎛️ Potmeter 3 |
| |






