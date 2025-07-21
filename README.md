# STM32F411 Nucleo: Button-Controlled LED

## Description
Simple GPIO demo for STM32F411RE Nucleo board:
- Press onboard user button (B1/PC13) to toggle onboard LED (LD2/PA5)

## Hardware
- **Board**: STM32F411RE Nucleo
- **MCU**: STM32F411RET6
- **Button**: PC13 (B1, active-low with external pull-down)


## Setup (STM32CubeIDE)
1. Generated with STM32CubeMX (HAL libraries)
2. Default clock config:
   - HSI 16MHz → PLL → 84MHz SYSCLK
3. GPIO:
   - PC13: Input (no pull, external pull-down on Nucleo)
   - PA5: Output push-pull, low speed

## Behavior
- Button pressed (PC13=Low) → LED ON (PA5=High)
- Button released → LED OFF

## Notes
- No debouncing implemented
- Built with STM32CubeIDE
- Refer to Nucleo schematics for pin details
