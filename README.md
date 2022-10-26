1. Создаем аккаунт на Github.com
2. Создаем локальный репозиторий у себя
3. "Подружить" ваш локальный и удаленный репозитории (Github подскажет как:)   ^**git remote add origin**  ссылка
4. Отправить (push) ваш локальный репозиторий на удаленный (на Github). При этом,вам, возможно нужно будет авторизоваться на удаленном репозитории
5. Провести изменения с "другого компьютера" (с Github к примеру)
6. Выкачать (pull) актуальное состояние из удаленного репозитория - в свою локальную версию


Регистрируемся на гитхаб и создаем свой репозиторий:

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
