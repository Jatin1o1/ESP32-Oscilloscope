# ESP32-Oscilloscope
ESP32 Oscilloscope with ST7789 display - 320 X  240 
Jobit Joseph published his work here https://circuitdigest.com/microcontroller-projects/diy-esp32-oscilloscope

## Changes from the Original Source Code:
1. Changes the wiring of TFT( #define TFT_D3  33 -> #define TFT_D3  18   ) , Please do check the *User_Setup.h in TFT_eSPI library*  while connecting the TFT ( Arduino TFT 2.4 inch ST7789 320*240 )
2. Changes in the frequency function (in data_analysis.h file), it needed to be multiplied by a factor of 2
3. Fixed ADC_Sampling function in i2s.ino file.  (i2s_read funtion is updated)
4. Change the Pins of input Buttons
5. Reduced Buffer Size to 49000 from 50000, else DMA ERROR were occuring  (#define BUFF_SIZE 50000 -> #define BUFF_SIZE 49000)
   
