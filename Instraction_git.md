# инструкция по работе с git

Git- это круто
![log_git](git.png)

## Создание нового репозитория

ЧТо бы создать репозиторий (инициализировать) нужно веести команду эту надпись

    git initq
  
## Команда git status 
показывает состояния файлов в рабочем каталоге и индексе: какие файлы изменены, но не добавлены в индекс; какие ожидают коммита в индексе. Вдобавок к этому выводятся подсказки о том, как изменить состояние файлов.

    git status
## Команда git diff 
используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между вашей рабочей копией и индексом (собственно git diff), разница между индексом и последним коммитом (git diff --staged), или между любыми двумя коммитами (git diff master branchB).

    git diff  (можноввести значения, между которыми нужно получить разницу)

## Команда git commit 
берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.

    git commit
    git commit -m "имя комита"   задает имя
    git commit -am "имя комита"   задает имя и выполняет команду add
## Команда git add 
добавляет содержимое рабочего каталога в индекс (staging area) для последующего коммита

    git add    (имя файла)

## перейти к нужной точке, к нужному комиту
    git checkout   (вводим номер комита, или мастер)
## список комитов 
    git log   
    git log --oneline  (коротким списком)   
    git log --oneline --all   все комиты коротким списком

# **_семинар2_**
## ветвление

### Отображения всех веток
нужно написать

    git branch
### Добаления новой ветки
нужно написать

    git branch (имя ветки)
### Удаление ветки
нужно написать

    git branch -d (имя ветки)
### Перееключение на другую ветку
команда
    git checkout (имя ветки)
### Отслеживание комитов с графиком ветвления
1. вариант
        
        git log --gpaph

2. вариант
        
        git log -all --oneline --graph
### Слияние веток
нужно выполнить команду в менно той ветке, в которую нужно добавить что то новое из другой какой нибудь ветки

    git merge
### Конфликты слияния
Для решения конфликтов сушествуют инструменты  VSCod предлогается на выбор 4 решения 
1. оставить первоначальный вариант
2. первоначальный вариант заменить на новый, из "новой ветки" той что сливаем с текушей!!!
3. Добавить оба варианта
4. отредактировать вручную
## Семинар оконцен, всем спасибо
# Семинар №3
## Работа с удаленными репозиториями

