You have to set the correct memory layout for your device in the linker script.
Please check the FLASH and SRAM length.

e.g.

MEMORY
{
  FLASH (rx) : ORIGIN = 0x08000000, LENGTH = 0x08000   /* 32k */
  RAM (rwx)  : ORIGIN = 0x20000000, LENGTH = 0x01000   /*  4k */
}

HOW TO USE: 

PRESS BOTH BUTTONS SIMULTANEOUSLY TO CHANGE MODES:

MODE 0: Press the buttons to turn ON or OFF the LED's
MODE 1: Automatic Heartbeat with PWM
MODE 2: PWM with buttons (press the buttons to change the brightness)
