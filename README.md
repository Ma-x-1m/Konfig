Разработать эмулятор для языка оболочки ОС. Необходимо сделать работу 
эмулятора как можно более похожей на сеанс shell в UNIX-подобной ОС. 
Эмулятор должен запускаться из реальной командной строки, а файл с 
виртуальной файловой системой не нужно распаковывать у пользователя. 
Эмулятор принимает образ виртуальной файловой системы в виде файла формата 
tar. Эмулятор должен работать в режиме CLI. 

Ключами командной строки задаются: 

• Путь к архиву виртуальной файловой системы. 

• Путь к лог-файлу. 

Лог-файл имеет формат json и содержит все действия во время последнего 
сеанса работы с эмулятором. 

Необходимо поддержать в эмуляторе команды ls, cd и exit, а также 
следующие команды: 
1. cp. 
2. tree. 

Все функции эмулятора должны быть покрыты тестами, а для каждой из 
поддерживаемых команд необходимо написать 2 теста.

---

# Virtual File System Emulator

Это проект эмуляции виртуальной файловой системы, который поддерживает базовые операции над файлами и каталогами, такие как просмотр содержимого директории, переход между папками, копирование файлов, отображение структуры файлов и другие.

## Основные возможности
- Эмуляция структуры файловой системы с помощью словаря (без использования библиотеки `os`).
- Поддержка команд:
  - `ls` — выводит содержимое текущей директории.
  - `cd` — смена текущей директории.
  - `cp` — копирование файлов.
  - `tree` — отображение дерева каталогов.
  - `exit` — завершение работы с эмулятором.
- Работа с `.tar` архивами для имитации исходной структуры файлов.
- Обработка ошибок, например, если файл или директория не существует.

---

## Как использовать

1. Убедитесь, что у вас установлен Python версии 3.8 и выше.
2. Скачайте проект на локальный компьютер.
3. Запустите главный файл `main.py`:
   ```bash
   python main.py

---

## Пример

![image](https://github.com/user-attachments/assets/ec3f82c9-934d-4f95-a9ac-29a6ebde78f2)


