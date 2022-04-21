**1) Посмотреть где я.**  
`pwd`

**2) Создать папку.**  
`mkdir task2`

**3) Зайти в папку.**  
`cd task2Cancel changes`

**4) Создать 3 папки.**  
`mkdir task4_0 task4_1 task4_2`  
   или  
`mkdir task{1..3}`  

**5) Зайти в любоую папку.**  
`cd /e/qa/hw_1_29free/task2/task4_0`

**6) Создать 5 файлов (3 txt, 2 json).**  
`touch 1.txt 2.txt 3.txt 1.json 2.json`  
   или  
`touch file{1..3}.txt file{1..2).json`

**7) Создать 3 папки.**  
`mkdir task{4..6}`  

**8. Вывести список содержимого папки.**  
`ls`  

**9) Открыть любой txt файл.**  
`vi file1.txt`  

**10) Написать туда что-нибудь, любой текст.**  
`isn + text (ввести текст тут)`  

**11) Сохранить и выйти.**  
`esc+ :wq`  

**12) Выйти из папки на уровень выше.**  
`cd ..`  

**13) Переместить любые 2 файла, которые вы создали, в любую другую папку.**  
`mv file1.json file2.json ./task4`  

**14) Скопировать любые 2 файла, которые вы создали, в любую другую папку.**  
`cp 1.json 2.json ./task2`  

**15) Найти файл по имени.**  
`find 1.txt`   
  или  
`find *txt, где * равно имени файла`

**16) Просмотреть содержимое в реальном времени (команда grep).**  
`grep text 1.txt  
ls | grep task1  
tail -f 1.txt | grep 2`  

**17) Вывести несколько первых строк из текстового файла.**  
`head -n2 1.txt`  

**18) Вывести несколько последних строк из текстового файла.**  
`tail -n3 1.txt`  

**19) Просмотреть содержимое длинного файла (команда less) изучите как она работает.**  
`less 1.txt`  

**20) Вывести дату и время.**  
`date +%x" "%X`  

-----

2) **Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13.**  
   *(3) Зайти в папку  
     4) Создать 3 папки  
     5) Зайти в любоую папку  
     6) Создать 5 файлов (3 txt, 2 json)  
     7) Создать 3 папки  
     8) Вывести список содержимого папки  
     13) Переместить любые 2 файла, которые вы создали, в любую другую папку.)*  

```css
touch script.txt	
vi script.txt	#!/bin/bash
                mkdir dt1_2
		cd dt1_2
		mkdir a1 a2 a3
		cd a1
		touch t{1..3}.txt j{1..2}.json
		mkdir st{1..3}
		ls
		mv {t1.txt,j2.json} ./st3
chmod +x ./script.txt	
./script.txt
```
	
