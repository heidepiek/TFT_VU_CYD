


# TFT VU Meter for ESP32 CYD

Hey there! This is a port of the awesome TFT VU Meter by Manny Miller (CineLights), brought over to the popular ESP32 Cheap Yellow Display (CYD).

> **Note on the source code:** Out of respect for the original creator's work, I'm not sharing the source code here. However, you'll find the ready-to-use `firmware.bin` and a simple web installer so you can easily flash it to your own CYD. All credits for the original project and idea go entirely to Manny Miller / CineLights!

## Hardware & Pinout
- **Display:** 2.8 inch ESP32 CYD (Cheap Yellow Display) with ST7789 driver and dual USB ports (USB-C & Micro USB).
- **Microphone (MAX9814):** 
  - Powered by 3.3V from the `CN1` connector.
  - Data pin hooked up to `P3` (GPIO35).
- **LED Strip (WS2812):**
  - Powered by an external 5V supply (make sure to tie the grounds together!).
  - Data pin hooked up to `CN1` (GPIO27).

## First Boot & Setup ⚠️
1. **Touch Calibration:** On the very first boot, you will see 4 arrows appear on the screen. Touch them one by one to calibrate the touch panel.
2. **Gain/Volume Adjustment:** Once booted into the menu, head over to **Settings** and turn the volume/input down a bit. It defaults to full volume, which can easily cause over-modulation and make the LEDs go haywire!

## Menu & Layout
- **Boot Screen:** Shows "Cine-Lights" at the top. Clicking it will take you straight to the credits menu.
- **Main Menu:** 
  - VU Meters
  - Standby Patterns
  - Settings
