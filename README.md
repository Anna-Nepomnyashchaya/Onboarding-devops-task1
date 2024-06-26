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
## Задание 5, 6. Работа с ветками.
Документация не требуется, ветки на гитлабе

## Задание 7. Решение конфликтов слияния.
```
git clone git@gitlab.wildberries.ru:ilin-leonid/git-merge.git
git branch -a
git checkout origin/feature
git checkout feature
git log
git checkout origin/develop
git checkout develop
git log
git merge feature
git add .
git commit -m "Merge branch 'feature' into develop"
git switch main
git merge develop
git add .
git commit -m "Merge branch 'develop' into 'main' and resolved conflict"
git log --graph --pretty=oneline --abbrev-commit --all --decorate
```
## Задание 9. cherry-pick
```
git clone git@gitlab.wildberries.ru:ilin-leonid/git-cherry-pick.git
git branch -a
git checkout origin/develop
git switch develop
git switch master
git cherry-pick 17938b2b85023f5863e664b49c76a6b04b4c7149
```

##Задание 10. Склеить 6 комитов в 1 комит и запушить.
```
git clone git@gitlab.wildberries.ru:ilin-leonid/git-squash.git
git branch -a
git checkout origin/develop
git switch develop
git checkout origin/show
git switch show
git remote rename origin old-origin
git rebase -i HEAD~6
git push --force origin develop
git log
```

![Картиночка](https://as2.ftcdn.net/v2/jpg/03/37/00/59/1000_F_337005995_hRjUA4xXUTbTgeJ0FchilPBITj3FxVHU.jpg "Картинка для просмотра при проверке")
