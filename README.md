# image-processing-tool-25948
Инструмент для обработки изображений
# Image Processing Tool

Программа для обработки изображений

## Студент

- Имя: Голубев Артем
- Группа: 25948

## Возможности

- Медианный фильтр (удаление шума)
- Фильтр Гаусса (размытие)
- Детекция границ (алгоритм Собеля)
- Изменение яркости

## Сборка
gcc main.c image_processing.c -o imgproc -lm -O2


## Использование

Медианный фильтр:
./imgproc input.jpg -median 3 output.jpg


Фильтр Гаусса:
./imgproc input.jpg -gauss 5 1.5 output.jpg


Детекция границ:
./imgproc input.jpg -edges 50 output.jpg


Изменение яркости:
./imgproc input.jpg -bright 30 output.jpg

## Форматы

Поддерживаются PNG, JPEG, BMP, TGA.

## Файлы проекта

- main.c - главный модуль
- image_processing.c - реализация фильтров
- image_processing.h - заголовочный файл
- stb_image_read.h - библиотека для чтения
- stb_image_write.h - библиотека для записи
