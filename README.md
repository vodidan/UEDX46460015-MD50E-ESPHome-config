# ESPHome Config for UEDX46460015-MD50ESP32 1.5" SH8601 Display

This repository contains a working ESPHome configuration for the **UEDX46460015-MD50ESP32** round touch knob display, which features:
https://www.aliexpress.com/item/1005008352920046.html
- 1.5" 466x466 round AMOLED panel  
- SH8601 display driver over QSPI  
- CST816 touch controller over I²C  
- Rotary encoder + button  

The config uses:
- `qspi_dbi` custom display driver from ESPHome
- LVGL for rendering UI
- Init sequence for SH8601


## 🛠️ Hardware Pins

| Function        | GPIO |
|----------------|------|
| QSPI CLK       | 10   |
| QSPI D0-D3     | 13, 11, 14, 9 |
| CS             | 12   |
| Reset          | 8    |
| I2C SDA/SCL    | 1, 3 |
| Touch INT/RST  | 4, 2 |
| Rotary A/B     | 5, 6 |
| Button         | 0    |
| Power Enable   | 17   |

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
