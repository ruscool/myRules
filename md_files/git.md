# Мини справочник по Git
***
### Устанавливаем в командной строке
***
### **Первоначальная настройка GIT**
#### Установить/изменить имя пользователя
    git config --global user.name "<Ваше_имя>"
#### Установить/изменить email пользователя
    git config --global user.mail Ваша@почта.com

***
#### Просмотр настроек
    git config --list

***
#### Превратить каталог, который не находится под
#### версионным контролем, в репозиторий Git
    git init

***
#### Индексировать измененный файл
    git add
#### Индексировать измененные файлы
    git add .

***
#### Удаление индексации файла
    git rm -cashed имя_файла
#### Удаление из индекса и из проекта
    git rm -f имя_файла

***
***
### Просмотр изменений
    git status
***
***
#### Фиксация изменения в локальное хранилище
#### В коммит попадут (будут сохранены) только файлы, 
#### которые были проиндексированы командой git add
    git commit -m "комментарии к коду"
***
#### Просмотр истории коммитов
    git log

***
### Связываение локального репозитория с GitHub 
    git remote add origin git@github.com:my_name/my_repo.git
#### Где my_name – имя пользователя на GitHub 
####my_repo – название созданного репозитория
#### Проверка свызывания  
    git remote get-url origin 
#### Удаление свызывания  
    git remote remove origin

***
#### Отправка изменений в удаленный 
#### репозиторий origin ветки master
    git push origin master

#### Отправка изменений c текущей ветки
    git push
#### Получение изменений
    git pull
***
#### Клонировать существующий репозиторий
    git clone ссылка-на-репозиторий
***
***
#### Добавление удаленного репозитория
    git remote add 'имя' - ,имя будет псевдонимом + сам репозиторий
#### Получить изменения без полного пути 
    git fetch 'имя' 'новое имя'
#### Просмотр удаленных репозитариев
    git remote -v
***
####Отмена индексации файла
    git restore --staged <file>
***
####Откат измененного файла с помощью git restore
    git restore <file>
***
#### Отмена недавно сделанные незакомиченные изменения в файле
    git checkout --<file>
#### Изменить последний коммит, добавить и изменить коментарий 
    git commit --amend
#### Позволяет отменить конкретный коммит
    git revert <commit>
#### "Жестко" срезаем все до указанного коммита 
    git reset --hard
#### Изменния после коммита которого указали - отправляем в индекс 
    git reset --soft
#### Отменяется все что было после этого коммита
    git reset --mixed


#### Литература:
1. Git book <https://git-scm.com/book/ru/v2>
2. Интерактивный тур по Git <https://githowto.com/ru>
3. "Бог в помощь" - поисковики :)

***