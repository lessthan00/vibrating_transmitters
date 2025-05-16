# vibrating_transmitters

依赖的项目:
https://github.com/lessthan00/ADXL345BCCZ-RL7_a
https://github.com/lessthan00/current-to-voltage-loop
https://github.com/lessthan00/HT7333
https://github.com/lessthan00/nucleo-stm32-pin32-kicad-b
https://github.com/lessthan00/TLV70450DBVR

## 主意事项

控制电流损耗

SMF3.3CA 反向漏电流Ir 500uA
SMAJ5.0CA Ir 800uA
SMAJ36CA Ir 1uA

慎重选择

LED 都去掉,驱动LED 要消耗大约1mA

## MCU选择

STM32L432KCBU6
PIN31->GND
PIN16->GND
PIN33->GND

## 通讯引脚选择

PA3->GPIO_down
PA4->DAC1_OUT1
PA5->SPI1_SCK
PA6->SPI1_MISO
PA7->SPI1_MOSI
PA8->INT2
PA9->INT1

## 底板绘制

引入接口
PCB引入模块的SVG图片,以对准位置

## 最后Gerber文件生成

所有模块加底板画成一个大板子->转嘉立创打板.