# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов
Коммит это одно из базовых понятий в Git. Если объяснять простым языком, то коммит это огромная копия вашего проекта в момент времени, когда этот коммит был сделан. 
1. **Конфликтующий материал**
2. + Для создания коммитов git commit -m "Первый коммит"
### Git add
Для добавления измений в коммит используется команда **git add**. Чтобы использовать команду **git add** напишите **git add <имя файла>**

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда **git status**. Для этого необходимо в папке с репозиторием написать **git status**, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: **git checkout <номер коммита>**

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда **git log**. Для этого достаточно выполнить команду **git log** в папке с репозиторием

## Ветки в Git

По сути ветки в Git представляют собой указатель на снимок изменений. Если нужно добавить новую возможность или исправить ошибку (незначительную или серьезную), вы создаете новую ветку, в которой будут размещаться эти изменения.

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*
Создание ветки с переключением сразу на неё **git branch -b branch name**

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда **git merge name branch**

## Удаление веток
Для удаления ветки ввести команду **git branch -d 'name branch'**

## Переключение между ветками

Для перехода на другую ветку используется команда **"git checkout branch name"**

## Конфликты и их решение

**Не получается создать конфликт**
Создадим конфликт с веткой 2
Напечатаем тоже самое в ветке мастер, но добивам ещё немного текста, и _выделим его курсивом_. 

* Попытка
* Номер
* Два

Спиливаю ветки, создаю ветку 5, следом пробую сделать конфликт и решить его.