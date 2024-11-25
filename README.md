# 198-STM32


NEO-6M GPS Parser in CubeIDE (STM32)
UART Setup: Configure UART at 9600 baud in CubeMX, enable DMA or interrupts for data reception.

Data Reception: Use a circular/ring buffer to store incoming NMEA sentences from the GPS module.

Parsing: Detect complete NMEA sentences (e.g., $GPGGA), tokenize using strtok, and extract key fields (latitude, longitude, UTC time, etc.).

Conversion: Convert latitude/longitude from DMS to decimal format as needed.

Usage: Integrate parsed data into your application for navigation or tracking.
