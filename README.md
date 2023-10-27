# Marlin 2.0.x (BigTreeTech SKR 1.4 and FLSun SR)
## Features
This fork of Marlin is built off of firmware provided by FLSun for the SKR 1.3 mainboard, reconfigured for the SKR 1.4 board.

Base Marlin features are maintained, as well as features such as the factory display.

## Build
As the firmware is based on Marlin2.0.x which is built on the core of PlatformIO, the buid compiling steps are the same as Marlin2.0.x. You can directly using [PlatformIO Shell Commands](https://docs.platformio.org/en/latest/core/installation.html#piocore-install-shell-commands), or using IDEs contain built-in PlatformIO Core(CLI), for example, [VSCode](https://docs.platformio.org/en/latest/integration/ide/vscode.html#ide-vscode) and [Atom](https://docs.platformio.org/en/latest/integration/ide/atom.html). VSCode is recommended.

If the initial build fails, replace the `.pio/build/LPC1768/src/src/HAL/LPC1768/MarlinSerial.cpp.o` file with the file located at `/FirmwarePatches/MarlinSerial.cpp.o` and attempt to build again.