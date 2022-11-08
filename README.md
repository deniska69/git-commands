## Разработка в отдельной ветке:
```
git checkout master
```
```
git pull
```
```
git checkout -b new-name-branch
```
## Ребейз своей ветки от master-ветки:
```
git checkout master
```
```
git pull
```
```
git checkout name-branch
```
```
git rebase origin/master
```
```
yarn start
```
- Проверить свою ветку на баги и затем:
```
git push --force
```
# Убрать во временное хранилище текущие наработки:
- Добавить все файлы и убрать в стэш:
```
git add .
```
```
git stash
```
- Уходим на какую-то ветку, что-то делаем
- Возвращаемся на ветку, в которой шла основная разработка:
git checkout branch-current
-Возвращаем наработки из стэша:
```
git stash pop
```
# Переименование последнего коммита:
```
git commit --amend -m new-name-commit
```
```
git push --force
```
# Отменить фиксацию последнего незапушенного коммита:
```
git reset HEAD~1 --soft
```
