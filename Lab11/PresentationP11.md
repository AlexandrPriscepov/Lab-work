### 11 Лабораторная работа
   Прищепов Александр
# Цель работы
Изучить основы программирования в оболочке ОС UNIX. Научится писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

## Выполнение лабораторной работы

1. Создадим командный файл pr1.sh, далее откроем его в emacs (рис.1)
рис 1:

![изображение](https://user-images.githubusercontent.com/104249657/170490851-ef7ac7fc-c097-4e45-97b0-79e436f50d04.png)

 - Используя команды getopts grep, запишем в файл программу (рис.2), которая анализирует командную строку с ключами: – -iinputfile — прочитать данные из указанного файла; – -ooutputfile — вывести данные в указанный файл; – -pшаблон — указать шаблон для поиска; – -C — различать большие и малые буквы; – -n — выдавать номера строк; а затем ищет в указанном файле нужные строки, определяемые ключом -p.

рис 2:

![изображение](https://user-images.githubusercontent.com/104249657/170491159-37125a00-4772-4f7f-9573-d31d22141a61.png)


 - Проверим работу файла, предварительно дав ему права на выполнение (chmod +x *.sh), и создадим два файла для проверки работы (touch one.txt two.txt) (рис.3,4). Запускаем файл

рис 3:

![изображение](https://user-images.githubusercontent.com/104249657/170491310-2a5ca617-0179-43ac-83f7-eaee372ccf84.png)

рис 4:

![изображение](https://user-images.githubusercontent.com/104249657/170491542-12f0cf10-1eb3-42f9-904b-704338075509.png)

## 2. Создадим два файла для третьего задания (команда touch pr2.c pr2.sh) и откроем в emacs.
Затем напишем на языке Си программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю. Затем программа завершается с помощью функции exit(n), передавая информацию в о коде завершения в оболочку. Командный файл должен вызывать эту программу и, проанализировав с помощью команды $?, выдать сообщение о том, какое число было введено

![изображение](https://user-images.githubusercontent.com/104249657/170492235-60ac954f-b06c-4737-9a39-11f99a7eadb2.png)

![изображение](https://user-images.githubusercontent.com/104249657/170492380-ec9199b0-0689-4b82-952e-5584998e915e.png)

 - Проверим работу командного файла, передав ему права на выполнения и запустив его 

![изображение](https://user-images.githubusercontent.com/104249657/170492616-b6d653a9-4735-40c0-b223-3f4b5d839d94.png)

![изображение](https://user-images.githubusercontent.com/104249657/170492689-80c53510-f582-4286-b028-b3b6d0a53f82.png)

## 3. Создадим командный файл files.sh и откроем его в emacs.Напишем командный файл, создающий указанное число файлов, пронумерованных последовательно от 1 до 𝑁 (например 1.tmp, 2.tmp и т.д.). Число файлов, которые необходимо создать, передаётся в аргументы командной строки. Этот же командный файл должен уметь удалять все созданные им файлы (если они существуют).

![изображение](https://user-images.githubusercontent.com/104249657/170492798-e1a209d0-c4d3-4a54-88d9-2a55b2c291b3.png)

 - Проверим его работу, передав ему права на выполнения и запустив его (команда ./files.sh)


## 4. Создадим командный файл pr4.sh и откроем его в emacs. Напишем командный файл, который с помощью команды tar запаковывает в архив все файлы в указанной директории. Модифицируем его так, чтобы запаковывались только те файлы, которые были изменены менее недели тому назад (использовать команду find).

![изображение](https://user-images.githubusercontent.com/104249657/170492859-c4c01c2d-f560-42d9-a186-7484c2d960f9.png)

 - Создадим в домашнем каталоге каталог catalog и перенесем туда некоторые файлы, измененные в разное время. Дадим командному файлу право на выполнение (chmod +x pr4.sh) и запустим его в этом каталоге. Файл работает исправно.

![изображение](https://user-images.githubusercontent.com/104249657/170493087-b5448c71-197e-4bc9-971e-28de79866764.png)


## Выводы

Я научился писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.
