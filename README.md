Note:

In CubeMX pin editor window:
- DS pin should be named as TFT_DC
- Reset pin should be named as TFT_RST
- Chip Select pin should be named as TFT_CS
- LED backlight pin to be connected to GPIO named TFT_LED

It then works like a modular unit without requirement of manual pin editing.
Check the .h files to see the list of available functions to use. Then call them from main.c.

**IMPORTANT**: you must include the .h files in main.c -
```c
/* USER CODE BEGIN Includes */

#include "lcd.h"
#include "GUI.h"
#include "test.h"  // If you want to use inbuilt test functions

/* USER CODE END Includes */
```

The .h files should be included in Core/Inc
The .c files should be included in Core/Src

Current files are configured to use SPI2
