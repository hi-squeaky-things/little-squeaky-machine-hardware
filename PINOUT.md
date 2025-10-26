```
 __   ____  ____  __       
(  ) (_  _)(_  _)(  )    
/ (_/\ )(    )(  / (_/\ 
\____/(__)  (__) \____/ 
Squeaky Machine
```

The LttL Squaky Machine is a hardware reference platform for the LttL Weirdo Software Synthesizer. 

# LttL Squeaky Machine Hardware


## Pin layout of the MCU

| Pin ESP32-S3-WROOM-1 | Pin ESP32S3 | Function ESP32S3 | Function |
| --- | --- | --- | --- |
| 04 | 04 | TOUCH_4 | 🫳 Touchpad row 1 |
| 05 | 05 | TOUCH_5 | 🫳 Touchpad row 2 |
| 06 | 06 | TOUCH_6 | 🫳 Touchpad row 3 |
| 07 | 07 | TOUCH_7 | 🫳 Touchpad row 4 |
| 08 | 15 |  ADC2_CH4  | 🎛️ Potmeter 1 |
| 09 | 16 |  ADC2_CH5 | 🎛️ Potmeter 2 |
| 10 | 17 |  U1TXD  | 🎹 MIDI out |
| 11 | 18 |  U1RXD | 🎹 MIDI in |
| 12 | 08 |  ADC1_CH7 | 🔌 USB power management |
| 13 | 19 |  USB_D- | 💻 USB-OTG / 🎹 USB-MIDI |
| 14 | 20 |  USB_D+ | 💻 USB-OTG / 🎹 USB-MIDI |
|  |
| 15 | 03 | NC | Not connected |
| 16 | 47 | NC | Not connected |
| 17 | 09 | TOUCH_9 | 🫳 Touchpad main 1 |
| 18 | 10 | TOUCH_10 | 🫳 Touchpad main 2 |
| 19 | 11 | TOUCH_11 | 🫳 Touchpad col 4 |
| 20 | 12 | TOUCH_12 | 🫳 Touchpad col 3 |
| 21 | 13 | TOUCH_13 | 🫳 Touchpad col 2 |
| 22 | 14 | TOUCH_14 | 🫳 Touchpad col 1 |
| 23 | 21 | RMT | 💡 Led controller |
| 24 | 47 | I2C_0_SDA | I2C controller data / 📺 OLED / 🔈 CODEC  |
| 25 | 48 | I2C_1_SDL | I2C controller clock / 📺 OLED / 🔈 CODEC |
| 26 | 45 |  NC | Not connected |
|  | 
| 28 | 35 | NC | Not connected |
| 29 | 36 | NC | Not connected |
| 30 | 37 | NC | Not connected |
| 31 | 38 | I2S_0_MLCK | I2S controller, master clock (MLCK) / 🔈 CODEC|
| 32 | 39 | I2S_0_WS | I2S controller, word select (LRCLK) / 🔈 CODEC |
| 33 | 40 | I2S_0_BLCK | I2S controller, block select (BLCK) / 🔈 CODEC |
| 34 | 41 | I2S_0_DIN | 🔈 I2S controller, data IN (DIN) / 🔈 CODEC |
| 35 | 42 | I2S_0_DOUT | 🎤 I2S controller, data OUT (DOUT) / 🔈 CODEC |
| 36 | 44 | U0RXD | Firmware TX / JTAG / Serial Debug |
| 37 | 43 | U0TXD| Firmware RX / JTAG / Serial Debug |
| 38 | 02 |  ADC1_CH1  | 🎛️ Potmeter 4 |
| 39 | 01 |  ADC1_CH0 | 🎛️ Potmeter 3 |
|






