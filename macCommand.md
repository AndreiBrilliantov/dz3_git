# Основные команды Терминала
Просмотр файлов и папок в директории
~~~
ls
ls -a //show all files including hidden ones
~~~
Перейти на директорию выше
~~~
cd ..
~~~
Перейти в корневую директорию
~~~
cd ~
~~~
Перейти в директорию по пути
~~~
cd [directoryName/]
~~~
Создать файл
~~~
touch [fileName.fileType]
~~~
Записать строчку в файл (+ создает файл)
~~~
echo "Text" > fileName.txt
~~~
Просмотреть файл
~~~
cat fileName.txt
~~~
Переместить/переименовать файл
~~~
mv fileName.txt newFileName.py // can specify the directory
~~~
Скопировать файл
~~~
cp [newFileName.txt]
~~~
Удалить файл
~~~
rm fileName.txt
~~~
Удалить рекурсивно содержимое директории (Если в ней есть другие файлы)
~~~
rm -R dirName
~~~

Посмотреть историю введенных команд
~~~
history
~~~
Отчистить консоль
~~~
clear
~~~