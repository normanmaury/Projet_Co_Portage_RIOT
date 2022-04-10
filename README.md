### STM32@Fablab

* <https://github.com/normanmaury/Projet_Co_Portage_RIOT>


## How to flash Wyres board
make all BOARD=wyres_proto
make flash BOARD=wyres_proto

##Using ST-Link
Run ST's software : STM32CubeProgrammer
Connect the board and choose ST-Link
Select Hardware reset in the configuration panel 
Transfer the .elf/.bin that has been created
Start Programming

##Troubleshooting
- If your using a standalone ST-Link with the wyres and the 
  board won't connect after you flashed it with CubeProgrammer:
  You want to reset (by removing the batteries e.g.) the board between your flashes
- The usage of a Discovery Board allows to reset directly without hardware manipulation
- Don't forget to remove the short-circuit module on the ST-Link Pin before flashing
