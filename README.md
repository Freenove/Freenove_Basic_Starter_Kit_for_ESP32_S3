ESP32 S3 FREENOVE RetroGo 1.45 - Freenove ESP32-S3 WROOM CAM Build Info Build Date: $(date) Build Host: macOS 13.6.0 Build Tool: rg_tool.py (ESP-IDF v4.4.6) Compiler: xtensa-esp32s3-elf-gcc 8.4.0

Target Device: Freenove ESP32-S3 WROOM CAM Chip Model: ESP32-S3 Flash Size: 16MB PSRAM Size: 8MB @ 80MHz (Octal Mode) Firmware Components:

Bootloader: 21,552 bytes (bootloader/bootloader.bin) Launcher: 923,840 bytes (launcher/launcher.bin) Retro-Core: 546,464 bytes (retro-core/retro-core.bin) Full Image: 2,031,616 bytes (firmware/RetroGo-1.45_ESP32_S3_WROOM_FREENOVE.img)

Partition Layout: Address Size Type Purpose 0x0000 - 0x8FFF Boot Bootloader 0x9000 - 0xCFFF NVS Non-volatile Storage 0xD000 - 0xEFFF OTA OTA Data 0xF000 - 0xFFFF PHY PHY Init Data 0x10000 - 0xFFFFF App Launcher App (960KB) 0x100000 - 0x1EFFFF App Retro-Core App (960KB)

Included Emulators: Game Boy / Game Boy Color (gnuboy) Game & Watch (gw-emulator) NES / Famicom (nofrendo) Hardware Configuration: CPU Frequency: 240MHz (Dual Core) Display: ILI9341 320x240 @ 40MHz SPI Audio: I2S Digital Output (MAX98357A) Buttons: 11 Game Buttons (GPIO Digital Input) Storage: Internal Flash (SD Card functionality disabled)

GPIO Mapping: Display (ILI9341): MOSI: GPIO12, CLK: GPIO48, CS: GPIO14 DC: GPIO47, RST: GPIO3, BLK: GPIO2 Audio (I2S): BCLK: GPIO5, WS: GPIO6, DIN: GPIO7

Game Buttons: UP: GPIO0, DOWN: GPIO1, LEFT: GPIO15, RIGHT: GPIO16 A: GPIO17, B: GPIO18, SELECT: GPIO8, START: GPIO9

MENU: GPIO10, OPTION: GPIO11, X: GPIO13 Build Options: RG_ENABLE_PSRAM: Enabled RG_ENABLE_CPU_240MHZ: Enabled RG_ENABLE_SPI_80MHZ: Enabled RG_ENABLE_SD_HIGHSPEED: Disabled RG_ENABLE_NETWORKING: Enabled RG_ENABLE_PROFILING: Disabled RG_BUILD_RELEASE: Disabled

Notes: This firmware is designed specifically for Freenove ESP32-S3 WROOM CAM. Camera functionality is disabled to save GPIO resources. SD Card functionality is temporarily disabled to avoid GPIO conflicts.

Audio output requires an external MAX98357A module.

Display requires an external ILI9341 module.

Please verify hardware connections are correct before flashing.

Technical Support: Hardware Setup Guide: docs/HARDWARE_SETUP.md Flashing Guide: docs/FLASHING_GUIDE.md Project Homepage: https://github.com/ducalex/retro-go
