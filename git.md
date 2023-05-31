# Основные команды GIT

[Все команды git](https://git-scm.com/docs)

## Настройки пользователей
>Устанавливает логин пользователя которое будет записываться при каждом изменении (видят другие разработчики)
~~~bash
git config --global user.name "[name]"
~~~
>Устанавливает почту (видят другие разработчики)
~~~bash
git config --global user.email "[email]"
~~~
>Включает подсветку при использовании терминала
~~~bash
git config --global color.ui auto
~~~
>Если хотим использовать свой тектовый редактор для git
~~~bash
git config --global core.editor "[program]"
~~~
>Показывает примененные настройки
~~~bash
git config --list
~~~


## Инициализация 
> Для работы с ГИТ необходимо перейти в папку в которой расположены файлы для отслеживания их версий

~~~bash
git init
~~~

## Статус 
> Выводит информацию по текущему коммиту
~~~bash
git status
~~~

## Отслеживание файла 
> Команда определяет какой файл в директории необходимо отслеживать 
~~~bash
git add git.md
git add --all # include all files in directory (git add . )
~~~

## История всех коммитов 
> Показывает все коммиты в ветке
~~~bash
git log
git log --oneline
git reflog //more detailed
~~~

## Разница 
> Команда выодит строки в которых есть различия. Если нет различий - ничего не выведет
~~~bash
git diff
~~~

## Коммит (Commit) 
> Создает версию (commit)
~~~bash
git commit -m "msg"
git commit -am "msg" //short recording. equal two command - git add.. + git commit 
~~~

## Переход к ветке/commit 
> Осуществляет переход к ветке или коммиту
~~~bash
git checkout [commitID]
git checkout master // get lasted(prod) version
~~~

## Соединение удаленного репозитория с локальным
Параметр origin - это название источника
~~~bash
git remote add origin url
git remote -v //make sure that the connection is established
~~~

## Отслеживания пустых папок
Перейти в директорию и создать там файл .gitkeep
~~~bash
touch dir/.gitkeep
~~~

## Правило игнорирование файлов/папок (убрать из отслеживания)
Перейти в директорию и создать там файл .gitignore
~~~bash
touch dir/.gitignore
~~~
Далее в созданный файл можно прописать файлы которые должны игнорироваться

## Возврат к определенному коммиту (сброс текущего состояния истории)
Команда позваляет вернуться к состоянию определенного коммита. при этом коммит который был сделан случайно пропадет из git log но останется в git reflog и можно откатиться
> idHash - указать кэш номер коммита к которому хотим откатиться
~~~bash
git reset idHash
~~~
отмена последствий коммита
~~~bash
git revert idHash
~~~
Сброс состояния файла на указанное
~~~bash
git restore idHash
~~~

~~~bash
git cat-file -p idHash
git cat file -t idHash
~~~

## Работа с ветками
Посмотреть существующие ветки
~~~bash
git branch
~~~

Создать новую ветку
~~~bash
git branch [name_branch]
~~~