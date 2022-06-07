# Bash-1
1) Посмотреть где я       -  `pwd`

2) Создать папку          -   `mkdir happiness`

3) Зайти в папку          -   `cd happiness`

4) Создать 3 папки        -   `mkdir money time work` 

5) Зайти в любоую папку   -   `cd time`

6) Создать 5 файлов 
      (3 txt, 2 json)     -   `touch second.txt minute.txt hour.txt week.json month.json`

7) Создать 3 папки        -   `mkdir breakfast lunch dinner`

8) Вывести список
 содержимого папки        -   `ls -la` 

9) + Открыть любой txt 
файл                      -   `cat hour.txt`

10) + написать туда 
что-нибудь, любой текст   -   `cat >> hour.txt`

11) + сохранить и выйти.  -   `Enter,  ctrl + C`

12) Выйти из папки на 
уровень выше              -   `cd ..`

13) переместить любые 
2 файла, которые вы 
создали, в любую 
другую папку              -    `mv time/second.txt time/minute.txt work/`
    

14) скопировать любые 
2 файла, которые вы 
создали, в любую другую
 папку.                   -    `cp time/month.json time/week.json money/`


15) Найти файл по имени   -    `find . -name "minute.txt"` 

16) просмотреть содержимое
 в реальном времени 
(команда grep) 
изучите как она работает. -    `tail -f time/hour.txt`     

17) вывести несколько
 первых строк из
 текстового файла         -     `head time/hour.txt`
ы

18)вывести несколько 
последних строк из 
текстового файла          -     `tail -5 time/hour.txt`

19) просмотреть содержимое
 длинного файла           -     `less time/hour.txt`

20) вывести дату и время  -     `date`






ЗАДАНИЕ 
1) Отправить http запрос
  на сервер               -      `curl "http://162.55.220.72:5005/get_method?name=Andy&age=34"`



2)  Написать скрипт который
 выполнит автоматически 
пункты 3, 4, 5, 6, 7, 8, 13  - 


вход в редактор  -   `nano bash_script.sh`


#!/bin/bash\n
cd happiness
mkdir money time work
cd time
touch second.txt minute.txt hour.txt week.json month.json
mkdir breakfast lunch dinner
ls -la
mv -t dinner/ minute.txt second.txt

echo "готово!"

запустить скрипт - bash bash_script.sh
