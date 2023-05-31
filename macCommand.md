# Основные команды Терминала
Просмотр файлов и папок в директории
~~~bash
ls
ls -a #show all files including hidden ones
~~~
Перейти на директорию выше
~~~bash
cd ..
~~~
Перейти в корневую директорию
~~~bash
cd ~
~~~
Перейти в директорию по пути
~~~bash
cd [directoryName/]
~~~
Создать файл
~~~bash
touch [fileName.fileType]
~~~
Записать строчку в файл (+ создает файл)
~~~bash
echo "Text" > fileName.txt
~~~
Просмотреть файл
~~~bash
cat fileName.txt
~~~
Переместить/переименовать файл
~~~bash
mv fileName.txt newFileName.py # can specify the directory
~~~
Скопировать файл
~~~bash
cp [newFileName.txt]
~~~
Удалить файл
~~~bash
rm fileName.txt
~~~
Удалить рекурсивно содержимое директории (Если в ней есть другие файлы)
~~~bash
rm -R dirName
~~~

Посмотреть историю введенных команд
~~~bash
history
~~~
Отчистить консоль
~~~bash
clear
~~~