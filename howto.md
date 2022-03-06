git clone https://github.com/KrolTryCode/KotlinAsFirst2020.git -- сохраняем репозиторий  
cd KotlinAsFirst2020 -- переходим в него
git remote add upstream-my https://github.com/sql3/KotlinAsFirst2021.git -- добавляем свой репозиторий в KotlinAsFirst2020  
git fetch upstream-my -- подгружаем KotlinAsFirst2021  
git branch backport -- создаем новую ветку - backport  
git checkout backport -- переходим в созданную ветку
git cherry-pick d535f359...FETCH_HEAD -- загружаем историю коммитов 
git remote add upstream-theirs https://github.com/Ken4ikS/KotlinAsFirst2021.git -- добавляем репозиторий товарища 
git fetch upstream-theirs -- подгружаем репозиторий товарища  
git add . -- добавляем измененные файлы, в которых возникли ошибки при merge  
git commit -m  -- коммитим  
git checkout master -- переходим в master  
git merge backport upstream-theirs/master -- объединяем  
Исправляем возникшие конфликты в vs code  
git add . -- добавляем измененные файлы, в которых возникли ошибки при merge  
git merge --continue  
git remote -v > remotes -- создаем файл remotes  
git add .  
git commit -m "check" -- коммитим  
git push -- пушим  
touch howto.md -- создаем файл  
git add .  
git commit -m "newFile" -- коммитим  
git push -- пушим  
редактируем файл на гитхабе  
сдаем работу и радуемся жизни  
