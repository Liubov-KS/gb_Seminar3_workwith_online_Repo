## My remote repository tutorial

### Команды по работе с новым онлайн репозиторием на github:

git push - отправляем изменения из локального репозитория

**git push -u origin main** / команда отправить инфо в оригинальный файл (на Гитхаб) 
 
git pull - получение изменений с сервера (из удаленного репозитория Гитхаб)

### *Расшифровка команд (что и куда отправляется):*

* git push origin HEAD  - Удобный способ отправить текущую ветку с тем же именем на сервере.
HEAD указывает на текущую ветку (current branch). Тем самым, не надо запоминать имя ветки, на которой вы находитесь.

* Отправка изменений:

Перед пушем надо зафиксировать текущие изменения, то есть сделать **git commit**.

* для отправки в терминале пишем:
**git push origin branch** 
Вместо branch — *__имя ветки, которую надо отправить__*. Чаще всего используется master или main: 

* git push origin master 
Такое каждый раз писать слишком громоздко, для этого придумали git push по умолчанию. Для этого единожды набираем предыдущую команду с флагом -u:  git push -u origin branch

* git push -u origin master
После этого можно писать более коротко, так как git запомнил, что пушить надо на сервер origin, ветку под именем master:

* git push
Таким образом, git позволяет запушить ветку в удаленный репозиторий. Чтобы через git добавить ветку в удаленный репозиторий, надо запушить существующую локальную ветку.


## Регистрация аккаунта и порядок действий: 
1. Создаем аккаунт на Github.com
2. Создаем локальный репозиторий у себя
3. "Подружить" ваш локальный и удаленный репозитории (Github подскажет как:)   ^**git remote add origin**  ссылка
4. Отправить (push) ваш локальный репозиторий на удаленный (на Github). При этом,вам, возможно нужно будет авторизоваться на удаленном репозитории
5. Провести изменения с "другого компьютера" (с Github к примеру)
6. Выкачать (pull) актуальное состояние из удаленного репозитория - в свою локальную версию

## Регистрируемся на гитхаб и создаем свой репозиторий:

(1) …or create a new repository on the command line (в терминале задать команды:)
echo "..." >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/Liubov-KS/Test_VvCtrlversii_Lesson3.git

git push -u origin main

(2) …or push an existing repository from the command line

__git remote add origin__ https://github.com/ ссылка на ваш онлайн репозиторий

__git branch -M main__    /основная ветка будет ветка "main"

__git push -u origin main__ /направить инфо отсюда в оригинальную (удаленную ветку на Github) - ветку "main"
