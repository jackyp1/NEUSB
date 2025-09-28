# NEUSB
## Summary
This project is to solve a particular problem I have. Third party controllers for old consoles are naff. At work, on my lunch I'll often play emulated NES games on a Raspberry Pi, but third party controllers feel awful to play with. I'm an embedded software engineer by trade, so I figured I could whip something up with a microcontroller in my own time to make a USB adapter for an original NES controller.

This project uses an STM32G431KBT6U microcontroller on the NUCLEO-G431KB.

## Pinout

### CN3
2 -> GND 

4 -> +5V

15 -> PB3 -> AF5 (SPI1_CLK) -> NES_CLK

### CN4
5 -> PA12 -> USB_DP

13 -> PA11 -> USB_DM

14 -> PB5 -> AF2 (TIM3_CH2) -> NES_LATCH

15 -> PB4 -> AF5 (SPI1_MISO) -> NES_DATA
