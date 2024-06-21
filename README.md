# Проект обробки відео з Raspberry Pi

## Опис

Цей проект захоплює відео з камери, підключеної до Raspberry Pi, обробляє його за допомогою OpenCV, а потім керує аналоговим виходом через PWM на основі середнього значення яскравості обробленого кадру.

## Вимоги

- Raspberry Pi (з Raspbian OS або іншою сумісною ОС)
- Камера, сумісна з Raspberry Pi (наприклад, камера Raspberry Pi)
- Підключення до Інтернету
- Доступ до GPIO пінів

## Інсталяція

### 1. Оновлення системи

Перед початком, оновіть вашу систему:

sudo apt-get update
sudo apt-get upgrade

2. Встановлення OpenCV
Щоб встановити OpenCV на Raspberry Pi, виконайте наступну команду:

sudo apt-get install python3-opencv

3. Встановлення RPi.GPIO
RPi.GPIO зазвичай встановлено за замовчуванням на Raspberry Pi. Якщо його немає, встановіть його за допомогою:

sudo apt-get install python3-rpi.gpio

4. Встановлення інших залежностей
Щоб встановити інші залежності, створіть файл requirements.txt з наступним вмістом:

numpy
opencv-python
RPi.GPIO
Потім виконайте наступну команду для встановлення залежностей:

pip3 install -r requirements.txt
