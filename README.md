# Frypi-LED

STM32CubeMX and Keil MDK project for the FryPi board.

## Hardware

- MCU: STM32F411RET6
- User LED: PC13 (`LED_T`)
- User key: PA0 (`KEY1`, active low)

## Current behavior

The LED turns on while KEY1 is pressed and turns off when the key is released.

## Workflow

1. Change peripheral configuration in `Frypi-LED.ioc` with STM32CubeMX.
2. Keep custom code inside `USER CODE BEGIN/END` sections.
3. Edit code in VS Code.
4. Run the default build task with `Ctrl+Shift+B`.
5. Run `Tasks: Run Task` → `Keil: Download` to build and flash through ST-Link.

