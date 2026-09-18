```
 ⡇ ⡇⢹⠁⢹⠁⡇ ⣏⡉ ⢎⡑⡎⢱⡇⢸⣏⡉⣎⣱⣇⠜⢇⢸ ⡷⢾⣎⣱⡎⠑⣇⣸⡇⡷⣸⣏⡉
 ⠧⠤⠇⠸ ⠸ ⠧⠤⠧⠤ ⠢⠜⠣⠪⠣⠜⠧⠤⠇⠸⠇⠱ ⠇ ⠇⠸⠇⠸⠣⠔⠇⠸⠇⠇⠹⠧⠤
```

The Little Squeaky Machine is a hardware reference platform for the [Little Weirdo Software Synthesizer](https://github.com/hi-squeaky-things/little-weirdo).

## Little Squeaky Machine Hardware

### ESP32-S3 processing pinout

This section reflects the board-level net names as they are labeled in the processing schematic, rather than a stale hand-transcribed table. The most reliable source is the actual net names on the schematic: `EN`, `CHIP_BOOT`, `TXD0`, `RXD0`, `USB_D+`, `USB_D-`, `I2C_SDA`, `I2C_SCL`, `I2S_*`, `TOUCH_*`, `MIDI_*`, and the encoder/LED nets.

#### Core power, reset and debug

| ESP32-S3 pin | Net name | Board function |
| --- | --- | --- |
| 3 | `EN` | Chip reset / enable |
| 0 | `CHIP_BOOT` | Boot strap / boot mode |
| 1 | `RESET` | Board reset net |
| 45 | `IO45` | Unused / no board net on the current schematic |
| 46 | `IO46` | Unused / no board net on the current schematic |

#### USB and MIDI

| ESP32-S3 pin | Net name | Board function |
| --- | --- | --- |
| 19 | `USB_D-` | USB-C data minus |
| 20 | `USB_D+` | USB-C data plus |
| 17 | `MIDI_OUT` | MIDI TRS-A output |
| 18 | `MIDI_IN` | MIDI TRS-A input |

#### I2C and OLED / codec bus

| ESP32-S3 pin | Net name | Board function |
| --- | --- | --- |
| 47 | `I2C_SDA` | I2C data to OLED and codec |
| 48 | `I2C_SCL` | I2C clock to OLED and codec |

#### Audio codec I2S bus

| ESP32-S3 pin | Net name | Board function |
| --- | --- | --- |
| 42 | `I2S_MLCK` | Audio codec master clock |
| 41 | `I2S_WS` | Audio codec LRCLK / word select |
| 40 | `I2S_BCLK` | Audio codec bit clock |
| 39 | `I2S_DOUT` | Audio data out |
| 38 | `I2S_DIN` | Audio data in |

#### Touch, key matrix and controls

| ESP32-S3 pin | Net name | Board function |
| --- | --- | --- |
| 4,5,6,7,15 | `TOUCH_ROW_1` ... `TOUCH_ROW_5` | Keys rows |
| 40 | `TOUCH_COL_1` ... `TOUCH_COL_5` | Keys columns |
| 40 | `KEY_SW_25` | Key matrix switch sense for the 25-key board |
| 40 | `LED_CTRL` | LED drive signal |
| 16,8 | `ENCO0_A/B` | Encoder 0 A/B channels |
| 3,9 | `ENCO1_A/B` | Encoder 1 A/B channels |
| 1,2 | `ENCO2_A/B` | Encoder 2 A/B channels |
| 43,44 | `ENCO3_A/B` | Encoder 3 A/B channels |
| 21 | `H_OLED` | OLED header net |

#### Notes

- The schematic labels the board nets as names like `TOUCH_ROW_1`, `TOUCH_COL_1`, `I2S_WS`, `MIDI_OUT`, etc. Those net names are the most trustworthy mapping source for the actual board.
- Some ESP32-S3 GPIOs are intentionally unused in the current board design and are left as no-connects on the processing sheet.
- The design uses the ESP32-S3's native USB pins for USB-C connectivity and the UART pins for debug/boot-related lines.




