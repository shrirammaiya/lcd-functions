Note:

In CubeMX pin editor window:
- DS pin should be named as TFT_DC
- Reset pin should be named as TFT_RST
- Chip Select pin should be named as TFT_CS
- LED backlight pin to be connected to GPIO named TFT_LED

It then works like a modular unit without requirement of manual pin editing.

The .h files should be included in Core/Inc
The .c files should be included in Core/Src

Current files are configured to use SPI2
