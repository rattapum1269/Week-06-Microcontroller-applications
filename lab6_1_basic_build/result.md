
### ขั้นตอนการทำ
# lab6-1
```c
rst:0x1 (POWERON_RESET),boot:0x12 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6372
load:0x40078000,len:15928
load:0x40080400,len:3880
entry 0x40080638
I (1675) boot: ESP-IDF v6.0-dev-1002-gbfe5caf58f 2nd stage bootloader
I (1679) boot: compile time Aug  6 2025 02:48:42
I (1680) boot: Multicore bootloader
I (2778) boot: chip revision: v3.0
I (2786) boot.esp32: SPI Speed      : 40MHz
I (2787) boot.esp32: SPI Mode       : DIO
I (2788) boot.esp32: SPI Flash Size : 2MB
I (2930) boot: Enabling RNG early entropy source...
I (3072) boot: Partition Table:
I (3072) boot: ## Label            Usage          Type ST Offset   Length
I (3073) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (3078) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (3079) boot:  2 factory          factory app      00 00 00010000 00100000
I (3213) boot: End of partition table
I (4298) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=09484h ( 38020) map
I (4818) esp_image: segment 1: paddr=000194ac vaddr=3ff80000 size=00024h (    36) load
I (5305) esp_image: segment 2: paddr=000194d8 vaddr=3ffb0000 size=025e0h (  9696) load
I (5811) esp_image: segment 3: paddr=0001bac0 vaddr=40080000 size=04558h ( 17752) load
I (6297) esp_image: segment 4: paddr=00020020 vaddr=400d0020 size=0ef10h ( 61200) map
I (6825) esp_image: segment 5: paddr=0002ef38 vaddr=40084558 size=08a60h ( 35424) load
I (8314) boot: Loaded app from partition at offset 0x10000
I (8315) boot: Disabling RNG early entropy source...
I (8482) cpu_start: Multicore app
I (16197) cpu_start: Pro cpu start user code
I (16200) cpu_start: cpu freq: 160000000 Hz
I (16201) app_init: Application information:
I (16202) app_init: Project name:     lab6_1_basic_build
I (16202) app_init: App version:      1
I (16203) app_init: Compile time:     Aug  6 2025 02:48:16
I (16205) app_init: ELF file SHA256:  f9a263d59...
I (16207) app_init: ESP-IDF:          v6.0-dev-1002-gbfe5caf58f
I (16211) efuse_init: Min chip rev:     v0.0
I (16213) efuse_init: Max chip rev:     v3.99
I (16215) efuse_init: Chip rev:         v3.0
I (16219) heap_init: Initializing. RAM available for dynamic allocation:
I (16222) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (16227) heap_init: At 3FFB2EA8 len 0002D158 (180 KiB): DRAM
I (16233) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (16235) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (16236) heap_init: At 4008CFB8 len 00013048 (76 KiB): IRAM
I (16340) spi_flash: detected chip: winbond
I (16357) spi_flash: flash io: dio
I (16386) main_task: Started on CPU0
I (16396) main_task: Calling app_main()
I (16406) LAB6_1: Lab 6.1: Basic ESP32 Project Structure
I (16406) LAB6_1: ESP-IDF Version: v6.0-dev-1002-gbfe5caf58f
I (16406) LAB6_1: Free heap size: 304636 bytes
I (16416) LAB6_1: Build system test - Counter: 0
I (18416) LAB6_1: Build system test - Counter: 1
I (20416) LAB6_1: Build system test - Counter: 2
I (22416) LAB6_1: Build system test - Counter: 3
I (24416) LAB6_1: Build system test - Counter: 4
I (26416) LAB6_1: Build system test - Counter: 5
I (28416) LAB6_1: Build system test - Counter: 6
I (30416) LAB6_1: Build system test - Counter: 7
I (32416) LAB6_1: Build system test - Counter: 8
I (34416) LAB6_1: Build system test - Counter: 9
I (36416) LAB6_1: Build system test - Counter: 10
I (38416) LAB6_1: Build system test - Counter: 11
I (40416) LAB6_1: Build system test - Counter: 12
I (42416) LAB6_1: Build system test - Counter: 13
I (44416) LAB6_1: Build system test - Counter: 14
I (46416) LAB6_1: Build system test - Counter: 15
I (48416) LAB6_1: Build system test - Counter: 16
I (50416) LAB6_1: Build system test - Counter: 17
I (52416) LAB6_1: Build system test - Counter: 18
I (54416) LAB6_1: Build system test - Counter: 19
I (56416) LAB6_1: Build system test - Counter: 20
```

# lab6-1-test
```c
rst:0x1 (POWERON_RESET),boot:0x12 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6372
load:0x40078000,len:15928
load:0x40080400,len:3880
entry 0x40080638
I (1594) boot: ESP-IDF v6.0-dev-1002-gbfe5caf58f 2nd stage bootloader
I (1598) boot: compile time Aug  6 2025 02:48:42
I (1599) boot: Multicore bootloader
I (2620) boot: chip revision: v3.0
I (2626) boot.esp32: SPI Speed      : 40MHz
I (2633) boot.esp32: SPI Mode       : DIO
I (2634) boot.esp32: SPI Flash Size : 2MB
I (2758) boot: Enabling RNG early entropy source...
I (2880) boot: Partition Table:
I (2881) boot: ## Label            Usage          Type ST Offset   Length
I (2883) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (2886) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (2891) boot:  2 factory          factory app      00 00 00010000 00100000
I (3014) boot: End of partition table
I (4013) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=09534h ( 38196) map
I (4518) esp_image: segment 1: paddr=0001955c vaddr=3ff80000 size=00024h (    36) load
I (4994) esp_image: segment 2: paddr=00019588 vaddr=3ffb0000 size=025e0h (  9696) load
I (5530) esp_image: segment 3: paddr=0001bb70 vaddr=40080000 size=044a8h ( 17576) load
I (6047) esp_image: segment 4: paddr=00020020 vaddr=400d0020 size=0efb8h ( 61368) map
I (6566) esp_image: segment 5: paddr=0002efe0 vaddr=400844a8 size=08b10h ( 35600) load
I (8273) boot: Loaded app from partition at offset 0x10000
I (8274) boot: Disabling RNG early entropy source...
I (8434) cpu_start: Multicore app
I (16136) cpu_start: Pro cpu start user code
I (16140) cpu_start: cpu freq: 160000000 Hz
I (16141) app_init: Application information:
I (16147) app_init: Project name:     lab6_1_basic_build
I (16151) app_init: App version:      1
I (16153) app_init: Compile time:     Aug  6 2025 02:48:16
I (16154) app_init: ELF file SHA256:  d1812da5f...
I (16156) app_init: ESP-IDF:          v6.0-dev-1002-gbfe5caf58f
I (16157) efuse_init: Min chip rev:     v0.0
I (16158) efuse_init: Max chip rev:     v3.99
I (16160) efuse_init: Chip rev:         v3.0
I (16163) heap_init: Initializing. RAM available for dynamic allocation:
I (16169) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (16172) heap_init: At 3FFB2EA8 len 0002D158 (180 KiB): DRAM
I (16173) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (16174) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (16174) heap_init: At 4008CFB8 len 00013048 (76 KiB): IRAM
I (16274) spi_flash: detected chip: winbond
I (16288) spi_flash: flash io: dio
I (16315) main_task: Started on CPU0
I (16325) main_task: Calling app_main()
I (16335) LAB1: === Build Information ===
I (16335) LAB1: Project Name: lab6_1_basic_build
I (16335) LAB1: ESP-IDF Version: v6.0-dev-1002-gbfe5caf58f
I (16345) LAB1: Compile Date: Aug  6 2025
I (16345) LAB1: Compile Time: 03:05:26
I (16345) LAB1: Chip Model: esp32
I (16345) LAB1: Free Heap: 304636 bytes
I (16345) LAB1: Running... Counter: 0
I (17355) LAB1: Running... Counter: 1
I (18355) LAB1: Running... Counter: 2
I (19355) LAB1: Running... Counter: 3
I (20355) LAB1: Running... Counter: 4
I (21355) LAB1: Running... Counter: 5
I (22355) LAB1: Running... Counter: 6
I (23355) LAB1: Running... Counter: 7
I (24355) LAB1: Running... Counter: 8
I (25355) LAB1: Running... Counter: 9
I (25355) LAB1: Current free heap: 304636 bytes
I (26355) LAB1: Running... Counter: 10
I (27355) LAB1: Running... Counter: 11
I (28355) LAB1: Running... Counter: 12
I (29355) LAB1: Running... Counter: 13
I (30355) LAB1: Running... Counter: 14
I (31355) LAB1: Running... Counter: 15
I (32355) LAB1: Running... Counter: 16
I (33355) LAB1: Running... Counter: 17
I (34355) LAB1: Running... Counter: 18
I (35355) LAB1: Running... Counter: 19
I (35355) LAB1: Current free heap: 304636 bytes
I (36355) LAB1: Running... Counter: 20
I (37355) LAB1: Running... Counter: 21
I (38355) LAB1: Running... Counter: 22
I (39355) LAB1: Running... Counter: 23
I (40355) LAB1: Running... Counter: 24
I (41355) LAB1: Running... Counter: 25
I (42355) LAB1: Running... Counter: 26
I (43355) LAB1: Running... Counter: 27
I (44355) LAB1: Running... Counter: 28
I (45355) LAB1: Running... Counter: 29
I (45355) LAB1: Current free heap: 304636 bytes
```
## 🔍 คำถามทบทวน

1. **Docker vs Native Setup**: อธิบายข้อดีของการใช้ Docker เปรียบเทียบกับการติดตั้ง ESP-IDF บน host system
- ANS
| ด้าน | Docker | Native |
|------|--------|--------|
| ความสะดวกในการติดตั้ง | ✅ สูง | ❌ ต้อง config เอง |
| ความยืดหยุ่นและพกพา | ✅ สูง | ❌ ต่ำ |
| ความเร็วและประสิทธิภาพ | ⚠ อาจช้ากว่า | ✅ เร็วกว่า |
| เข้าถึง hardware/serial | ❌ ต้อง map พอร์ต | ✅ เข้าถึงตรง |
| ใช้งานร่วมกับ IDE | ⚠ ต้อง config เพิ่ม | ✅ ง่ายกว่า |
| เหมาะกับผู้ใช้ | ผู้เริ่มต้น, DevOps | ผู้ใช้ขั้นสูง, Debug |

2. **Build Process**: อธิบายขั้นตอนการ build ของ ESP-IDF ใน Docker container ตั้งแต่ source code จนได้ binary
flowchart TD
    A[Source Code on Host] --> B[Mount to Container]
    B --> C[เข้าสู่ Container]
    C --> D[Environment Setup]
    D --> E[Set Target & Menuconfig]
    E --> F[Run idf.py build]
    F --> G[Binary Files Created (.bin, .elf)]
    G --> H{เชื่อมต่ออุปกรณ์?}
    H -- Yes --> I[Flash ผ่าน USB]
    H -- No --> J[Copy binary กลับ host เพื่อ flash ภายหลัง]

3. **CMake Files**: บทบาทของไฟล์ CMakeLists.txt แต่ละไฟล์คืออะไร และทำงานอย่างไรใน Docker environment?
| ไฟล์ | ที่อยู่ | หน้าที่ |
|------|--------|---------|
| `CMakeLists.txt` | โฟลเดอร์ root | เรียก `project.cmake` เพื่อสร้างระบบ build |
| `main/CMakeLists.txt` | โฟลเดอร์ main/ | ระบุ source files และ header files สำหรับ component |
| `project.cmake` | (ESP-IDF) | เตรียมระบบ build ทั้งหมด ใช้ร่วมกับ ESP-IDF |
4. **Git Ignore**: ไฟล์ .gitignore มีความสำคัญอย่างไรสำหรับ ESP32 project development?
- .gitignore คือเครื่องมือสำคัญในการจัดการโค้ดให้สะอาดและเป็นระเบียบ
- ช่วยลดปัญหาที่เกิดจากไฟล์ build ชั่วคราว และไฟล์เฉพาะเครื่องในโปรเจกต์ ESP32
- ทำให้ทีมงานทำงานร่วมกันได้ราบรื่นและลดข้อผิดพลาดจากไฟล์ไม่จำเป็น
5. **Container Persistence**: ข้อมูลใดบ้างที่จะหายไปเมื่อ restart container และข้อมูลใดที่จะอยู่ต่อ?
| ประเภทข้อมูล              | อยู่หรือหายเมื่อ Restart Container? |
|--------------------------|-------------------------------------|
| ไฟล์ใน container layer   | ❌ หาย (ถ้าไม่ได้ mount)             |
| ไฟล์ในโฟลเดอร์ mount จาก host | ✅ อยู่ต่อ                         |
| Docker volume            | ✅ อยู่ต่อ                         |
| Environment variables    | ❌ หาย (ต้องกำหนดใหม่ทุกครั้ง)       |

6. **Development Workflow**: เปรียบเทียบ workflow การพัฒนาระหว่างการใช้ Docker กับการทำงานบน native system


| ขั้นตอน / ด้าน            | Docker                              | Native System                      |
|--------------------------|-----------------------------------|----------------------------------|
| การติดตั้ง                | ง่าย, พร้อมใช้, ไม่ยุ่งยาก        | ต้องติดตั้งเอง, อาจซับซ้อน      |
| ความเสถียรของ environment | สม่ำเสมอ, เหมือนกันทุกเครื่อง    | ขึ้นกับเครื่อง, อาจไม่เหมือนกัน |
| การแก้ไขโค้ด              | แก้ไขบน host, build ใน container  | แก้ไขและ build บนเครื่องตรง ๆ   |
| ความเร็ว build            | อาจช้ากว่าเล็กน้อย (due to container overhead) | เร็วกว่าปกติ                   |
| ความสะดวกในการอัพเดต     | เปลี่ยน image ง่าย               | ต้องจัดการ dependencies เอง      |
| การ debug ขั้นสูง        | ยากกว่า                         | ง่ายกว่า, เข้าถึง hardware ได้เต็มที่ |