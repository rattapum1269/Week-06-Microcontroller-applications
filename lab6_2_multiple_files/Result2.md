### lab6-2

# sensor.c+sensor.h
```c
rst:0x1 (POWERON_RESET),boot:0x12 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6372
load:0x40078000,len:15928
load:0x40080400,len:3880
entry 0x40080638
I (1599) boot: ESP-IDF v6.0-dev-1002-gbfe5caf58f 2nd stage bootloader
I (1604) boot: compile time Aug  6 2025 03:55:30
I (1605) boot: Multicore bootloader
I (2608) boot: chip revision: v3.0
I (2614) boot.esp32: SPI Speed      : 40MHz
I (2615) boot.esp32: SPI Mode       : DIO
I (2616) boot.esp32: SPI Flash Size : 2MB
I (2757) boot: Enabling RNG early entropy source...
I (2894) boot: Partition Table:
I (2896) boot: ## Label            Usage          Type ST Offset   Length
I (2897) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (2900) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (2902) boot:  2 factory          factory app      00 00 00010000 00100000
I (3024) boot: End of partition table
I (4016) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=09634h ( 38452) map
I (4501) esp_image: segment 1: paddr=0001965c vaddr=3ff80000 size=00024h (    36) load
I (4956) esp_image: segment 2: paddr=00019688 vaddr=3ffb0000 size=025e0h (  9696) load
I (5454) esp_image: segment 3: paddr=0001bc70 vaddr=40080000 size=043a8h ( 17320) load
I (5981) esp_image: segment 4: paddr=00020020 vaddr=400d0020 size=0f0ach ( 61612) map
I (6448) esp_image: segment 5: paddr=0002f0d4 vaddr=400843a8 size=08c58h ( 35928) load
I (7757) boot: Loaded app from partition at offset 0x10000
I (7759) boot: Disabling RNG early entropy source...
I (7922) cpu_start: Multicore app
I (15123) cpu_start: Pro cpu start user code
I (15127) cpu_start: cpu freq: 160000000 Hz
I (15128) app_init: Application information:
I (15129) app_init: Project name:     lab6_2_multiple_files
I (15133) app_init: App version:      1
I (15136) app_init: Compile time:     Aug  6 2025 03:54:37
I (15138) app_init: ELF file SHA256:  4c9147caf...
I (15140) app_init: ESP-IDF:          v6.0-dev-1002-gbfe5caf58f
I (15141) efuse_init: Min chip rev:     v0.0
I (15142) efuse_init: Max chip rev:     v3.99
I (15144) efuse_init: Chip rev:         v3.0
I (15151) heap_init: Initializing. RAM available for dynamic allocation:
I (15154) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (15155) heap_init: At 3FFB2EA8 len 0002D158 (180 KiB): DRAM
I (15156) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (15156) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (15157) heap_init: At 4008D000 len 00013000 (76 KiB): IRAM
I (15275) spi_flash: detected chip: winbond
I (15290) spi_flash: flash io: dio
I (15328) main_task: Started on CPU0
I (15348) main_task: Calling app_main()
I (15348) MAIN: 🚀 Lab 6.2: Multiple Source Files Demo
I (15348) MAIN: 📍 Main function from file: ./main/lab6_2_multiple_files.c, line: 13
I (15348) MAIN: ESP-IDF Version: v6.0-dev-1002-gbfe5caf58f
I (15358) SENSOR: 🔧 Sensor initialized from file: ./main/sensor.c, line: 12
I (15358) SENSOR: 📡 Sensor module ready for operation
I (15358) MAIN: === Loop 0 ===
I (15358) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (15368) SENSOR: 🌡️  Temperature: 27.4°C
I (15398) SENSOR: 💧 Humidity: 63.8%
I (17398) MAIN: === Loop 1 ===
I (17398) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (17398) SENSOR: 🌡️  Temperature: 33.1°C
I (17398) SENSOR: 💧 Humidity: 96.2%
I (19398) MAIN: === Loop 2 ===
I (19398) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (19398) SENSOR: 🌡️  Temperature: 35.4°C
I (19398) SENSOR: 💧 Humidity: 67.6%
I (19398) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (19398) SENSOR: 📈 All sensors operating normally
I (21408) MAIN: === Loop 3 ===
I (21408) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (21408) SENSOR: 🌡️  Temperature: 31.5°C
I (21408) SENSOR: 💧 Humidity: 83.6%
I (23408) MAIN: === Loop 4 ===
I (23408) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (23408) SENSOR: 🌡️  Temperature: 28.9°C
I (23408) SENSOR: 💧 Humidity: 79.1%
I (25408) MAIN: === Loop 5 ===
I (25408) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (25408) SENSOR: 🌡️  Temperature: 35.4°C
I (25408) SENSOR: 💧 Humidity: 92.0%
I (25408) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (25408) SENSOR: 📈 All sensors operating normally
```
# display

```c

rst:0x1 (POWERON_RESET),boot:0x12 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6372
load:0x40078000,len:15928
load:0x40080400,len:3880
entry 0x40080638
I (1601) boot: ESP-IDF v6.0-dev-1002-gbfe5caf58f 2nd stage bootloader
I (1613) boot: compile time Aug  6 2025 03:55:30
I (1614) boot: Multicore bootloader
I (2640) boot: chip revision: v3.0
I (2645) boot.esp32: SPI Speed      : 40MHz
I (2647) boot.esp32: SPI Mode       : DIO
I (2649) boot.esp32: SPI Flash Size : 2MB
I (2776) boot: Enabling RNG early entropy source...
I (2905) boot: Partition Table:
I (2906) boot: ## Label            Usage          Type ST Offset   Length
I (2908) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (2914) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (2918) boot:  2 factory          factory app      00 00 00010000 00100000
I (3045) boot: End of partition table
I (4121) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=09824h ( 38948) map
I (4641) esp_image: segment 1: paddr=0001984c vaddr=3ff80000 size=00024h (    36) load
I (5148) esp_image: segment 2: paddr=00019878 vaddr=3ffb0000 size=025e0h (  9696) load
I (5672) esp_image: segment 3: paddr=0001be60 vaddr=40080000 size=041b8h ( 16824) load
I (6173) esp_image: segment 4: paddr=00020020 vaddr=400d0020 size=0f230h ( 62000) map
I (6724) esp_image: segment 5: paddr=0002f258 vaddr=400841b8 size=08e48h ( 36424) load
I (8462) boot: Loaded app from partition at offset 0x10000
I (8463) boot: Disabling RNG early entropy source...
I (8639) cpu_start: Multicore app
I (16543) cpu_start: Pro cpu start user code
I (16549) cpu_start: cpu freq: 160000000 Hz
I (16553) app_init: Application information:
I (16555) app_init: Project name:     lab6_2_multiple_files
I (16556) app_init: App version:      1
I (16557) app_init: Compile time:     Aug  6 2025 03:54:37
I (16558) app_init: ELF file SHA256:  ec571c1bf...
I (16559) app_init: ESP-IDF:          v6.0-dev-1002-gbfe5caf58f
I (16559) efuse_init: Min chip rev:     v0.0
I (16560) efuse_init: Max chip rev:     v3.99
I (16561) efuse_init: Chip rev:         v3.0
I (16565) heap_init: Initializing. RAM available for dynamic allocation:
I (16570) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (16574) heap_init: At 3FFB2EA8 len 0002D158 (180 KiB): DRAM
I (16576) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (16577) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (16579) heap_init: At 4008D000 len 00013000 (76 KiB): IRAM
I (16692) spi_flash: detected chip: winbond
I (16709) spi_flash: flash io: dio
I (16736) main_task: Started on CPU0
I (16746) main_task: Calling app_main()
I (16746) MAIN: 🚀 Lab 6.2: Multiple Source Files Demo
I (16756) MAIN: 📍 Main function from file: ./main/lab6_2_multiple_files.c, line: 14
I (16756) MAIN: ESP-IDF Version: v6.0-dev-1002-gbfe5caf58f
I (16756) SENSOR: 🔧 Sensor initialized from file: ./main/sensor.c, line: 12
I (16766) SENSOR: 📡 Sensor module ready for operation
I (16766) DISPLAY: 🖥️  Display initialized from file: ./main/display.c, line: 9
I (16766) DISPLAY: 💡 Display module ready
I (16766) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (16776) DISPLAY: 📺 Message: System Starting...
I (16776) MAIN: === Loop 0 ===
I (16776) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (16776) DISPLAY: ✨ Display ready for new content
I (16786) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (16786) SENSOR: 🌡️  Temperature: 33.7°C
I (16806) SENSOR: 💧 Humidity: 71.5%
I (16806) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (16806) DISPLAY: 📈 Value 1: 26.50
I (16806) DISPLAY: 📉 Value 2: 61.00
I (18816) MAIN: === Loop 1 ===
I (18816) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (18816) DISPLAY: ✨ Display ready for new content
I (18816) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (18816) SENSOR: 🌡️  Temperature: 34.4°C
I (18816) SENSOR: 💧 Humidity: 69.9%
I (18816) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (18826) DISPLAY: 📈 Value 1: 27.50
I (18826) DISPLAY: 📉 Value 2: 62.00
I (20826) MAIN: === Loop 2 ===
I (20826) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (20826) DISPLAY: ✨ Display ready for new content
I (20826) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (20826) SENSOR: 🌡️  Temperature: 32.4°C
I (20826) SENSOR: 💧 Humidity: 67.6%
I (20826) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (20826) DISPLAY: 📈 Value 1: 28.50
I (20836) DISPLAY: 📉 Value 2: 63.00
I (20836) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (20846) SENSOR: 📈 All sensors operating normally
I (20846) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (20846) DISPLAY: 📺 Message: Status Check Complete
I (22846) MAIN: === Loop 3 ===
I (22846) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (22846) DISPLAY: ✨ Display ready for new content
I (22846) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (22846) SENSOR: 🌡️  Temperature: 32.7°C
I (22846) SENSOR: 💧 Humidity: 71.0%
I (22846) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (22846) DISPLAY: 📈 Value 1: 29.50
I (22846) DISPLAY: 📉 Value 2: 64.00
I (24856) MAIN: === Loop 4 ===
I (24856) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (24856) DISPLAY: ✨ Display ready for new content
I (24856) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (24856) SENSOR: 🌡️  Temperature: 34.8°C
I (24856) SENSOR: 💧 Humidity: 69.8%
I (24866) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (24866) DISPLAY: 📈 Value 1: 30.50
I (24866) DISPLAY: 📉 Value 2: 65.00
I (26866) MAIN: === Loop 5 ===
I (26866) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (26866) DISPLAY: ✨ Display ready for new content
I (26866) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (26866) SENSOR: 🌡️  Temperature: 29.3°C
I (26866) SENSOR: 💧 Humidity: 95.3%
I (26866) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (26866) DISPLAY: 📈 Value 1: 31.50
I (26876) DISPLAY: 📉 Value 2: 66.00
I (26876) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (26876) SENSOR: 📈 All sensors operating normally
I (26876) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (26886) DISPLAY: 📺 Message: Status Check Complete
```
# ทดลองเพิ่ทเติม
```c
rst:0x1 (POWERON_RESET),boot:0x12 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6372
load:0x40078000,len:15928
load:0x40080400,len:3880
entry 0x40080638
I (1325) boot: ESP-IDF v6.0-dev-1002-gbfe5caf58f 2nd stage bootloader
I (1327) boot: compile time Aug  6 2025 03:55:30
I (1328) boot: Multicore bootloader
I (2073) boot: chip revision: v3.0
I (2078) boot.esp32: SPI Speed      : 40MHz
I (2079) boot.esp32: SPI Mode       : DIO
I (2080) boot.esp32: SPI Flash Size : 2MB
I (2182) boot: Enabling RNG early entropy source...
I (2288) boot: Partition Table:
I (2288) boot: ## Label            Usage          Type ST Offset   Length
I (2289) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (2291) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (2293) boot:  2 factory          factory app      00 00 00010000 00100000
I (2389) boot: End of partition table
I (3144) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=09a24h ( 39460) map
I (3525) esp_image: segment 1: paddr=00019a4c vaddr=3ff80000 size=00024h (    36) load
I (3884) esp_image: segment 2: paddr=00019a78 vaddr=3ffb0000 size=025e0h (  9696) load
I (4249) esp_image: segment 3: paddr=0001c060 vaddr=40080000 size=03fb8h ( 16312) load
I (4629) esp_image: segment 4: paddr=00020020 vaddr=400d0020 size=0f3e4h ( 62436) map
I (5019) esp_image: segment 5: paddr=0002f40c vaddr=40083fb8 size=09048h ( 36936) load
I (6287) boot: Loaded app from partition at offset 0x10000
I (6288) boot: Disabling RNG early entropy source...
I (6411) cpu_start: Multicore app
I (12217) cpu_start: Pro cpu start user code
I (12221) cpu_start: cpu freq: 160000000 Hz
I (12222) app_init: Application information:
I (12222) app_init: Project name:     lab6_2_multiple_files
I (12223) app_init: App version:      1
I (12223) app_init: Compile time:     Aug  6 2025 03:54:37
I (12225) app_init: ELF file SHA256:  bfaba04af...
I (12225) app_init: ESP-IDF:          v6.0-dev-1002-gbfe5caf58f
I (12226) efuse_init: Min chip rev:     v0.0
I (12227) efuse_init: Max chip rev:     v3.99
I (12228) efuse_init: Chip rev:         v3.0
I (12230) heap_init: Initializing. RAM available for dynamic allocation:
I (12233) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (12235) heap_init: At 3FFB2EB0 len 0002D150 (180 KiB): DRAM
I (12236) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (12237) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (12239) heap_init: At 4008D000 len 00013000 (76 KiB): IRAM
I (12323) spi_flash: detected chip: winbond
I (12336) spi_flash: flash io: dio
I (12357) main_task: Started on CPU0
I (12367) main_task: Calling app_main()
I (12367) MAIN: 🚀 Lab 6.2: Multiple Source Files Demo
I (12367) MAIN: 📍 Main function from file: ./main/lab6_2_multiple_files.c, line: 15
I (12377) MAIN: ESP-IDF Version: v6.0-dev-1002-gbfe5caf58f
I (12377) SENSOR: 🔧 Sensor initialized from file: ./main/sensor.c, line: 12
I (12377) SENSOR: 📡 Sensor module ready for operation
I (12377) DISPLAY: 🖥️  Display initialized from file: ./main/display.c, line: 9
I (12377) DISPLAY: 💡 Display module ready
I (12377) LED: 💡 LED initialized from file: ./main/led.c, line: 12
I (12387) LED: 🔧 LED module ready
I (12387) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (12387) DISPLAY: 📺 Message: System Starting...
I (12387) LED: 🚀 Starting LED blink task from file: ./main/led.c, line: 59
I (12387) LED: ✨ LED blink task started from file: ./main/led.c, line: 49
I (12397) LED: ✅ LED ON from file: ./main/led.c, line: 20
I (12397) LED: 🟢 LED is now ON
I (12397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
I (12397) MAIN: === Loop 0 ===
I (12397) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (12397) DISPLAY: ✨ Display ready for new content
I (12407) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (12407) SENSOR: 🌡️  Temperature: 35.4°C
I (12417) SENSOR: 💧 Humidity: 94.9%
I (12417) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (12417) DISPLAY: 📈 Value 1: 26.50
I (12427) DISPLAY: 📉 Value 2: 61.00
I (12427) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (12427) DISPLAY: 📺 Message: LED Status: ON
I (14427) MAIN: === Loop 1 ===
I (14427) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (14427) DISPLAY: ✨ Display ready for new content
I (14427) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (14427) SENSOR: 🌡️  Temperature: 27.8°C
I (14427) SENSOR: 💧 Humidity: 74.8%
I (14427) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (14427) DISPLAY: 📈 Value 1: 27.50
I (14427) DISPLAY: 📉 Value 2: 62.00
I (14437) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (14437) DISPLAY: 📺 Message: LED Status: ON
I (15397) LED: ❌ LED OFF from file: ./main/led.c, line: 27
I (15397) LED: 🔴 LED is now OFF
I (15397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
I (16437) MAIN: === Loop 2 ===
I (16437) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (16437) DISPLAY: ✨ Display ready for new content
I (16437) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (16437) SENSOR: 🌡️  Temperature: 34.9°C
I (16437) SENSOR: 💧 Humidity: 76.9%
I (16437) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (16437) DISPLAY: 📈 Value 1: 28.50
I (16437) DISPLAY: 📉 Value 2: 63.00
I (16437) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (16447) DISPLAY: 📺 Message: LED Status: OFF
I (16447) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (16447) SENSOR: 📈 All sensors operating normally
I (16447) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (16447) DISPLAY: 📺 Message: Status Check Complete
I (18397) LED: ✅ LED ON from file: ./main/led.c, line: 20
I (18397) LED: 🟢 LED is now ON
I (18397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
I (18447) MAIN: === Loop 3 ===
I (18447) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (18447) DISPLAY: ✨ Display ready for new content
I (18447) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (18447) SENSOR: 🌡️  Temperature: 25.9°C
I (18447) SENSOR: 💧 Humidity: 83.6%
I (18447) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (18447) DISPLAY: 📈 Value 1: 29.50
I (18447) DISPLAY: 📉 Value 2: 64.00
I (18457) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (18457) DISPLAY: 📺 Message: LED Status: ON
I (20457) MAIN: === Loop 4 ===
I (20457) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (20457) DISPLAY: ✨ Display ready for new content
I (20457) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (20457) SENSOR: 🌡️  Temperature: 26.7°C
I (20457) SENSOR: 💧 Humidity: 66.9%
I (20457) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (20457) DISPLAY: 📈 Value 1: 30.50
I (20467) DISPLAY: 📉 Value 2: 65.00
I (20467) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (20467) DISPLAY: 📺 Message: LED Status: ON
I (21397) LED: ❌ LED OFF from file: ./main/led.c, line: 27
I (21397) LED: 🔴 LED is now OFF
I (21397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
I (22467) MAIN: === Loop 5 ===
I (22467) DISPLAY: 🧹 Screen cleared from file: ./main/display.c, line: 28
I (22467) DISPLAY: ✨ Display ready for new content
I (22467) SENSOR: 📊 Reading sensor data from file: ./main/sensor.c, line: 18
I (22467) SENSOR: 🌡️  Temperature: 33.3°C
I (22467) SENSOR: 💧 Humidity: 76.7%
I (22467) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (22467) DISPLAY: 📈 Value 1: 31.50
I (22477) DISPLAY: 📉 Value 2: 66.00
I (22477) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (22477) DISPLAY: 📺 Message: LED Status: OFF
I (22477) SENSOR: ✅ Sensor status check from file: ./main/sensor.c, line: 30
I (22477) SENSOR: 📈 All sensors operating normally
I (22477) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (22477) DISPLAY: 📺 Message: Status Check Complete
I (24397) LED: ✅ LED ON from file: ./main/led.c, line: 20
I (24397) LED: 🟢 LED is now ON
I (24397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
```
## 🔍 คำถามทบทวน

1. **Multiple Source Files**: เหตุใดต้องแยก source code เป็นหลายไฟล์?

- การแยกซอร์สโค้ดเป็นหลายไฟล์เป็นการทำให้โค้ดมีความเป็นระเบียบ มีโครงสร้างที่ชัดเจน และช่วยให้การทำงานร่วมกันเป็นทีมมีประสิทธิภาพมากขึ้น ซึ่งเป็นสิ่งสำคัญสำหรับโปรเจกต์ซอฟต์แวร์ทุกขนาด โดยเฉพาะโปรเจกต์ขนาดใหญ่

2. **CMakeLists.txt Management**: การเพิ่มไฟล์ source ใหม่ต้องแก้ไขอะไรบ้าง?

- การแยก Source Code และ CMakeLists.txt
การแยกซอร์สโค้ดออกเป็นหลายไฟล์ในโปรเจกต์ขนาดใหญ่มีประโยชน์หลายอย่าง เช่น:

 จัดระเบียบ: ทำให้โค้ดเป็นระเบียบและง่ายต่อการอ่าน
 นำกลับมาใช้ใหม่: สามารถนำโค้ดในไฟล์อื่นมาใช้ซ้ำได้
 ทำงานเป็นทีม: ลดปัญหาการแก้ไขไฟล์ซ้ำซ้อนเมื่อทำงานเป็นทีม
 บำรุงรักษา: แก้ไขหรือเพิ่มฟีเจอร์ได้ง่ายขึ้น
 คอมไพล์เร็วขึ้น: ประหยัดเวลาในการคอมไพล์
3. **Header Files**: บทบาทของไฟล์ `.h` คืออะไร และทำไมต้องมี?
- กล่าวโดยสรุป ไฟล์ `.h` ทำหน้าที่เป็นเหมือน สัญญา (contract) ที่บอกว่ามีอะไรให้ใช้งานได้บ้าง โดยเก็บรายละเอียดการทำงานไว้ในไฟล์ .cpp ซึ่งช่วยให้โค้ดเป็นระเบียบ ทำงานเป็นทีมได้ง่าย และช่วยลดเวลาในการคอมไพล์

4. **Include Directories**: เหตุใด CMakeLists.txt ต้องระบุ INCLUDE_DIRS?
- ไฟล์ `.h`เป็นส่วนสำคัญที่ช่วยให้การเขียนโปรแกรมมีโครงสร้างที่ชัดเจน ส่วนคำสั่ง include_directories() ใน CMakeLists.txt เป็นเครื่องมือที่ช่วยให้การจัดการไฟล์ .h ในโปรเจกต์เป็นไปอย่างราบรื่น
5. **Git Ignore**: ไฟล์ .gitignore ช่วยอะไรในการจัดการ ESP32 project?
- การไม่ดึงไฟล์ที่ไม่ต้องการ ให้ขึ้น  git
6. **Task Management**: การใช้ FreeRTOS task ในโมดูล LED ช่วยอะไร?
- การใช้ FreeRTOS task ในโมดูล LED ช่วยให้การจัดการพฤติกรรมของ LED เป็นอิสระจากโค้ดหลัก,  ทำให้โปรแกรมโดยรวมทำงานได้อย่างมีประสิทธิภาพ, ไม่เกิดปัญหา blocking, และสามารถจัดลำดับความสำคัญของงานได้ ซึ่งเป็นแนวทางปฏิบัติที่ดีสำหรับการพัฒนาโปรแกรมบนระบบปฏิบัติการแบบ Real-Time (RTOS)

7. **Code Organization**: ข้อดีของการแยกโมดูล sensor, display, led เป็นไฟล์แยกคืออะไร?
- การแยกโค้ดเป็นโมดูลต่าง ๆ มีข้อดีหลักคือช่วยให้โค้ดเป็นระเบียบ, เข้าใจง่าย, สามารถนำไปใช้ซ้ำได้, และง่ายต่อการแก้ไขและบำรุงรักษา ซึ่งเป็นแนวทางปฏิบัติที่ดีที่สุดสำหรับการเขียนโปรแกรม โดยเฉพาะในโปรเจกต์ขนาดใหญ่

## 💡 บันทึกผลการทดลอง

**ขั้นตอนที่ 1 (เฉพาะ sensor.c):**
- จำนวนไฟล์ source: 4
- ขนาด binary: 163041 bytes
- การทำงาน: ตัวจับอุณภูมิและความชื้น EX.
```c
I (18447) SENSOR: 🌡️  Temperature: 25.9°C
I (18447) SENSOR: 💧 Humidity: 83.6%
```
**ขั้นตอนที่ 2 (เพิ่ม display.c):**
- จำนวนไฟล์ source: 6
- ขนาด binary: 163925 bytes
- การทำงาน: แสดงผลสรุป EX.
```c
I (22467) DISPLAY: 📊 Data display from file: ./main/display.c, line: 21
I (22467) DISPLAY: 📈 Value 1: 31.50
I (22477) DISPLAY: 📉 Value 2: 66.00
I (22477) DISPLAY: 📢 Displaying from file: ./main/display.c, line: 15
I (22477) DISPLAY: 📺 Message: LED Status: OFF
```
**ขั้นตอนที่ 3 (เพิ่ม led.c):**
- จำนวนไฟล์ source: 8
- ขนาด binary: 164873 bytes
- การทำงาน: EX.
```c
I (21397) LED: ❌ LED OFF from file: ./main/led.c, line: 27
I (21397) LED: 🔴 LED is now OFF
I (21397) LED: 🔄 LED toggled from file: ./main/led.c, line: 38
```