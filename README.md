# STM32 ARM Cortex-M3 Basic I
Mempelajari penggunaan STM32F103 dengan CubeMX pada sistem operasi linux. Pada kali ini akan mencoba menyambungkan dengan Ublox-M8N. Fitur yang digunakan adalah **UART, RTC**

### Setup
Jangan lupa memastikan bahwa cmake, libusb, dan stlink sudah terinstall.
Selain itu pastikan juga CubeMX sudah mengkonfigurasi code generator untuk membuat **makefile**
Command yang perlu ditambahkan pada makefile:
```bash

#######################################
# flash
#######################################
flash:
	cd build && st-flash write STM32F103_061220.bin 0x8000000
```
