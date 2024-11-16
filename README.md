# LR6
Лабораторная работа №6
### __GitHUB__
_Цель лабораторной работы_: изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.

# Ход выполнения лабораторной работы
> Скриншоты лабораторной работы находятся в папке screenshots, каждый из них имеет название, соответствующее номеру пункта, выполнение которого необходимо подкрепить этим самым скриншотом. Например, скриншот для пункта 1 соответственно имеет название _1.png_
## Пункт 1
Необходимо создать аккаунт на сайте GitHub (_см. [рис. 1](https://github.com/mishaanyaa/LR6/tree/report/screenshots/1.png)_). 
## Пункт 2
Далее при помощи Fork создается копия [репозитория лабораторной работы](https://github.com/Kurtyanik/LR6/) в личное хранилище (_см. [рис. 2](https://github.com/mishaanyaa/LR6/tree/report/screenshots/2.png)_).
## Пункт 3
Соглано лабораторной работе, необходимо установить Git (_см. [рис. 3](https://github.com/mishaanyaa/LR6/tree/report/screenshots/3.png)_).
## Пункт 4
Далее с помощью _git config --global user_name_ и _git config --global user_email_ был настроен клиент git (_см. [рис. 4](https://github.com/mishaanyaa/LR6/tree/report/screenshots/4.png)_).
## Пункт 5
Затем на диске С в папке infa была создана копия своего личного удалённого репозитория на компьютер (_см. [рис. 5](https://github.com/mishaanyaa/LR6/tree/report/screenshots/5.png)_).
## Пункт 6
Теперь нужно добавить файл через интерфейс GitHub и подтянуть изменения в локальный репозиторий. На скриншоте 6 (_см. [рис. 6](https://github.com/mishaanyaa/LR6/tree/report/screenshots/6.png)_) представлены файлы, находящиеся в локальном репозитории, до обновленния данных и после. Их поиск осуществляется командой _ls -1_, а обновление информации - _git pull_.
## Пункты 7, 8
Далее необходимо получить историю операций для веток и просмотреть последние изменения. Первое осуществлялось с помощью команды _git reflog branch_name_, а второе - с помощью _log_ (_см. [рис. 7, 8](https://github.com/mishaanyaa/LR6/tree/report/screenshots/7-8.png)_).
## Пункт 9
Затем нужно выполнить слияние в ветку master. С помощью команды _git merge branch_name_ ветки _master_ и _new_file_ были объединены (содержимое new_file появилось в ветке master, _см. [рис. 9](https://github.com/mishaanyaa/LR6/tree/report/screenshots/9.png)_).
## Пункт 10
Теперь необходимо удалить побочную ветку. Для этого была использована команда _git branch -d branch_name_ (_см. [рис. 10](https://github.com/mishaanyaa/LR6/tree/report/Report/screenshots/10.png)_).
## Пункт 11
Для наглядной работы с репозиторием необходимо сделать изменения и зафиксировать их, оставляя комментарии. Поочередно в репозиторий были добавлены три текстовых файла: minecraft.txt, fnaf.txt, fnaf2.txt, созданные командой _echo "text" >> name.txt_. Извенения фиксировались командой _git add_, для создания коммита - _git commit -m "text"_, для обновления информации в репозитории - _git push_ (_см. [рис. 11.1](https://github.com/mishaanyaa/LR6/tree/report/screenshots/11_1.png); [рис. 11.2](https://github.com/mishaanyaa/LR6/tree/report/screenshots/11_2.png); [рис. 11.3](https://github.com/mishaanyaa/LR6/tree/report/screenshots/11_3.png)_).
## Пункт 12
С помощью _git revert HEAD --no-edit_ был осуществлен откат коммита (_см. [рис. 12](https://github.com/mishaanyaa/LR6/tree/report/screenshots/12.png)_).

# Лог команд
git config --global user.name "4315 Бондарев М. А."

git config --global user.email "mishabond005@mail.ru"

cd /C:/Users/Misha/Documents/OP_GUAP

git clone https://github.com/mishaanyaa/LR6

ls -1

git pull

ls -1

git reflog

git log

git checkout branch1

ls -1

git checkout master

ls -1

git merge branch1

ls -1

git push --delete origin branch1

echo "LA LA LA" >> bavaria.txt

git status

git add bavaria.txt

git status

git commit -m "1 файл"

echo "penalty a favor del real madrid" >> real.txt

git status

git add real.txt

git commit -m "2 файл"

echo "марко ройс, мой любимый марко ройс снова не чемпион" >> bor.txt

git add bor.txt

git commit -m "3 файл"

git status

git push

git revert HEAD --no-edit

git push

# История операций
С помощью команды _git log --pretty=format:"%h - %ad - %an: %s" --date=short_ была получена история операций в укороченном виде.

f3c6778 - 2024-11-16 - 4315 Бондарев М. А.: Revert "3 файл"

7fe93d7 - 2024-11-16 - 4315 Бондарев М. А.: 3 файл

eec5379 - 2024-11-16 - 4315 Бондарев М. А.: 2 файл

9a4308e - 2024-11-16 - 4315 Бондарев М. А.: 1 файл

fdf515a - 2024-11-16 - 4315 Бондарев М. А.: Порешал конфликт

718fb1f - 2024-11-16 - Misha: Create neymar.txt

ae45c56 - 2024-11-16 - Misha: Create messi

921f53b - 2020-11-21 - Kurtyanik: Обновление информации

0f9f50d - 2020-11-21 - Kurtyanik: Заполнил файл

c08a654 - 2020-11-21 - Kurtyanik: Файл создан пустым

3c6e913 - 2020-11-21 - Kurtyanik: Initial commit
