# Отчёт по лабораторной работе: `Команда grep`
**Выполнил:** Левахин Лев Александрович 343730

## Ход работы:

1. Создание файла `data.txt`:  
Файл `data.txt` был создан и заполнен данными, как описано в задании
![data.png](screenshots%2Fdata.png)

2. Поиск строк, содержащих line:  
```bash
grep "line" data.txt
````
Результат
```
This is the first line of data.
Second Line with some UPPER case.
third line with 123 numbers.
Another line with punctuation,!.
a line that includes start too
special  special line.
```
![1.png](screenshots%2F1.png)

3. Поиск строк, содержащих special, игнорируя регистр: 
```bash
grep -i "special" data.txt
```
Результат
```
a special line.
special  special line.
```
![2.png](screenshots%2F2.png)

4. Поиск строк, содержащих цифры:  
```bash
grep "[0-9]" data.txt
```
Результат
```
third line with 123 numbers.
```
![3.png](screenshots%2F3.png)

5. Поиск строк, начинающихся со слова This:   
```bash
grep "^This" data.txt
```
Результат
```
This is the first line of data.
This line contains START.
This line is started.
```
![4.png](screenshots%2F4.png)

6. Подсчет строк, содержащих слово start: 
```bash
grep -c "start" data.txt
```
Результат
```2```
![5.png](screenshots%2F5.png)

7. Вывод строк, не содержащих line: 
```bash
grep -v "line" data.txt
```
Результат
```
...
```
![6.png](screenshots%2F6.png)

7. Сохранение строк с цифрами в файл numbers.txt:
```bash
grep "[0-9]" data.txt > numbers.txt
```
Результат: сохранение строк с цифрами в файл numbers.txt. В терминал ничего выведено не было.
![7.png](screenshots%2F7.png)
![7_numbers.png](screenshots%2F7_numbers.png)

8. Проверка содержимого numbers.txt:
```bash
cat numbers.txt
```
Содержимое файла numbers.txt.
```
third line with 123 numbers.
```
![8.png](screenshots%2F8.png)

## Вывод:
В ходе выполнения лабораторной работы я успешно познакомился с командой grep и её основными возможностями. 
Я научился искать строки по шаблону, игнорировать регистр, искать строки по началу слова, считать количество совпадений, 
выводить строки не содержащие определённое слово и сохранять результаты поиска в файл.   
Команда grep показала себя как очень полезный инструмент для работы с текстовыми данными.