# download repo
git clone git@github.com:local-bot/git_basics

- setting user

git config --global user.name "user"
git config --global user.emai "email@example.com"


- edit or add some files
nano README.md

- include files to git in order to make changes to repo
git add filename # or git add . for all files
- undo includes
git reset

- check changes made
git status

- commit
git commit -m "some infos about your changes"

- make changes definitive to the default master branch
git push origin master