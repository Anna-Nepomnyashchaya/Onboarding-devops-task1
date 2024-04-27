#  Лист баш-команд для выполнения домашки
## Вносим изменения в конфиг
 - git config --global user.name "nepomnyaschaya.a2"
 - git config --global user.email nepomnyaschaya.a2@wb.ru

## Cоздаем локальный проект
> 1. git init "home_work"
> 2. cd home_work
> 3. touch README.md nginx.conf
4. git add .
5. git commit -m "initial commit"
6. git log
7. git status

## Пушим репу на 2 удаленных репозитория
* git remote add origin git@gitlab.wildberries.ru:nepomnyaschaya.a2/onboarding-devops-task1.git
    - git remote -v
    - git push -u origin main
* git remote add origin-github git@github.com:Anna-Nepomnyashchaya/Onboarding-devops-task1.git
    - git remote -v
    - git push -u origin-github main
 ## Клонируем репу и смотрим 6-ой комит
```bash
 git clone git@gitlab.wildberries.ru:ilin-leonid/git-checkout.git
 git checkout dfbdad
 git show
```
### Полезные ресурсы
| Ресурс | Ссылка |
| ------ | ------ |
| Основы гит | https://git-scm.com/book/ru/v2/Основы-Git-Работа-с-удалёнными-репозиториями |
| Ветвление | https://git-scm.com/book/ru/v2/Ветвление-в-Git-О-ветвлении-в-двух-словах |
## Добавляем файл гитигнор в нем прописываем директорию tmp/
```
vim .gitignore
touch ignored_file file_for_ignore another-ignored-file
git add -A
git log
git status
git show
git push origin
```

![Картиночка](https://as2.ftcdn.net/v2/jpg/03/37/00/59/1000_F_337005995_hRjUA4xXUTbTgeJ0FchilPBITj3FxVHU.jpg "Картинка для просмотра при проверке")
