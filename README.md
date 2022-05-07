# RadioFrog
Simple arduino-based RF transmitter and receiver using 433 MHz modules

# Plan

## Transmitter

- MX-RM-5v
- Digispark attiny85 (USB Type B - MicroUsb)


## Receiver

- FS1000A
- Button
- Digispark attiny85 (USB Type A)

# Installation

Digispark – плата на базе ATtiny85, загрузка в которую может производиться через бортовой USB. Для работы с Digispark нужно добавить поддержку плат в Arduino IDE:

    Запустить Arduino IDE, перейти в Файл/Настройки/
    В окошко “Дополнительные ссылки…” Вставить
        http://digistump.com/package_digistump_index.json
        или https://raw.githubusercontent.com/digistump/arduino-boards-index/master/package_digistump_index.json
    Нажать ОК
    Перейти в Инструменты/Плата/Менеджер плат… Начать вводить в поиске “Digispark”. Выбрать и установить Digistump AVR Boards
    Теперь в списке плат Инструменты/Плата/ появится семейство плат Digispark! Выбираем первую Digispark (Default – 16.5mhz)

https://digistump.com/wiki/digispark/tutorials/connecting

# Troobleshooting

sudo apt-get install libusb-0.1-4
sudo apt install libusb-dev

Compile micronucleus (to resolve v2.2 of the board) and replace the original one located in
/home/$USER/.arduino15/packages/digistump/tools/micronucleus/2.0a4

https://startingelectronics.org/tutorials/arduino/digispark/digispark-linux-setup/


https://digistump.com/wiki/digispark/tutorials/linuxtroubleshooting

