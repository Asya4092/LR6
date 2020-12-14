##ОТЧЁТ О ЛАБОРАТОРНОЙ РАБОТЕ №6 
## ПО ОСНОВАМ ПРОГРАММИРОВАНИЯ



###Ход работы:
Cделала копию на сайте GitHubhttps://github.com/Kurtyanik/LR6/

![Копированный репозиторий](screen/2.png)

В консоли Git Bash перешла в созданную на рабочем столе папку oplr6

Далее использовала команду _git init_, чтобы инициализировать гит в данной папке

![Git init](screen/5.png)

С помощью команды _git remote add origin_ связала папку с удалённым репозиторием на сайте GitHub

![Git remote add origin](screen/6.png)

Затем через графический интерфейс GitHub добавила новый файл op.txt в удалённый репозиторий и добавила его в ветку __master__

![Новый файл](screen/3.png)

![Новый файл](screen/4.png)

Пользуясь командой _git pull origin master_ , загрузила изменения из удалённого репозитория в локальный

![Git pull](screen/7.png)

Командой _git log_ получила список операций/коммитов

![git log](screen/8.png)

Используя _git show *commit SHA-1*_ , получила более подробную информацию по последнему изменению

![git show](screen/9.png)

Командой _git checkout -t branch1_ попыталась переключится на другую ветку **branch1**, но выдало ошибку. Поэтому с помощью команды _git remote update_ обновила подключение к сайту GitHub и заново выполнила переключение на ветку **branch1**

![git checkout](screen/10.png)

Попыталась выполнить слияние веток **master** и **branch1** командой _git merge branch1_ , попросило авторизоваться

![Merge error](screen/11.png)

Заново попыталась выполнить слияние и получила ошибку 

![Merge error](screen/12.png)

Вручную изменила файл mergefile.txt, вызвавший ошибку слияния и выполнила коммит

![Fix](screen/13.png)

Выполнила слияние веток **master** и **branch1** а затем удалила ветку **branch1** командой _git branch -d branch1_

![Merge and branch delete](screen/14.png)

Запушила всё в удалённый репозиторий командой _git push origin master_ 

![Push1](screen/15.png)

Затем сделала несколько изменений, добавив новые файлы text2.txt и text3.txt

![New files](screen/16.png)

![New files](screen/17.png)

Командой _git reset --hard HEAD~1_ выполнила откат последнего коммита - добавления файла **text3.txt**

![Hard reset](screen/18.png)

Запушила изменённую ветку _git push -f origin master_

![Push2](screen/19.png)

![Push2 result](screen/20.png)

Пользуясь командой _git checkout -b otchet_ , создала новую ветку **otchet**

![New branch](screen/21.png)

С помощью команды _git add ._ подготовила все новые файлы в папке **oplr6** к пушу

![Git add .](screen/22.png)

Запушила файлы скриншотов в удалённый репозиторий

![Git add .](screen/23.png)

Оформляю отчёт в файле **README.md** , используя блокнот

![Readme](screen/24.png)



Лог команд из папки **.git/logs**

![Logs](screen/25.png)

Финальный результат команды _git log_

![Git log3](screens/26.png)

Все файлы скриншотов лежат в папке **screen**
