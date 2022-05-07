# RadioFrog
Simple arduino-based RF transmitter and receiver using 433 MHz modules

# Plan

- Switch to 8 MHz and 3.3 v power
- Add antenna 13 cm
- 

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

# Characteristic

## Receiver
    Напряжение питания: 5 В
    Несущая частота: 433 МГц
    Максимальная пропускная способность: 5 кб/сек
    Потребляемый ток: 4,5 мА
    Чувствительность: −106…-110 дБм
    Диапазон рабочих температур: −20…+80 °C

## Transmitter
    Напряжение питания: 3–12 В
    Несущая частота: 433 МГц
    Максимальная пропускная способность: 8 кб/сек
    Потребляемый ток: 8 мА
    Выходная мощность: 32 мВт
    Диапазон рабочих температур: −20…+80 °C

## Digispark Attiny85 (both)
    https://iarduino.ru/lib/eef404f668a0834ace20ad691c09fcba.pdf
    
    ATtiny25/45/85: 0 – 10 MHz @ 2.7 - 5.5V, 0 - 20 MHz @ 4.5 - 5.5V

# Troobleshooting

sudo apt-get install libusb-0.1-4
sudo apt install libusb-dev

Compile micronucleus (to resolve v2.2 of the board) and replace the original one located in
/home/$USER/.arduino15/packages/digistump/tools/micronucleus/2.0a4

https://startingelectronics.org/tutorials/arduino/digispark/digispark-linux-setup/
https://digistump.com/wiki/digispark/tutorials/connecting
https://digistump.com/wiki/digispark/tutorials/linuxtroubleshooting