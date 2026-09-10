

# Достаточно выполнить один раз, настройка запомнится для всех новых репозиториев название ветки main
git config --global init.defaultBranch main

cd proect
git init     создает инициализирует репозитарий

git status

echo 'Hello, Hexlet!' > README.md      новый текст в файл
echo 'Haskell Curry' >> PEOPLE.md        добавляем тект к уже существующему тексту в файле

git add README.md    добавляем файл в репозитарий

git commit -m 'add README.md'   добавляем коммит

git ls-files  список отслеживаемых файлов
ls -a         список файлов в проекте

создаем репозитарий на GitHub
обьединяем его с локальным репозитарием на компьютере
 Вам нужна ссылка для работы с репозиторием по SSH
git remote add origin git@github.com: НА ГИТХАБЕ < ИМЯ > /hexlet-git.git
git branch -M main
git push -u origin main
Клонировать репозиторий можно с помощью команды git clone. Полную команду для клонирования можно получить на странице репозитория. Для этого нажмите большую кнопку Code, перейдите на вкладку SSH и скопируйте содержимое:
git clone git@github.com:<ИМЯ НА ГИТХАБЕ>/hexlet-git.git
git pull –rebase   проверить новые коммиты нв GitHub


rm PEOPLE.md   удалить файл

git restore PEOPLE.md  восстановить файл из локального репозитария

полное удаление

rm PEOPLE.md
# Любое изменение нужно добавлять в индекс
git add PEOPLE.md
git commit -m 'remove PEOPLE.md'
git rm PEOPLE.md
# Равносильно rm + git add

изменить проект на GitHub

git add .
git commit -m "Сохранение текущей работы перед pull"

git pull origin main     Скачайте изменения с GitHub:


git push origin main     Отправьте всё на GitHub:

git diff                   общие изменения перед коммитом

git diff –stages      изменеия после индекса до коммита  выхол q

git lod –oneline

git mv файл1 файл2  переименование файла

git log                                   		        список всех коммитов
git log -p         			       список всех diff коммитов
git show fnsdlfkjhlkdfjhkkjghfjh;м         diff конкретного коммита по хешу
git blame INFO.md                                  кто последним менял конкретную строчку в файле?

git grep                                                    поиск совпадений
git grep -i                                                  поиск без учета реистра

