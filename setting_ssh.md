
# Setting shh enviroment

download repo
> git clone git@github.com:local-bot/git_basics

setting user
> git config --global user.name "user"
> git config --global user.emai "email@example.com"


edit or add some files
>nano README.md

include files to git in order to make changes to repo
> git add filename # or git add -A for all files

undo includes
> git reset

check changes made
> git status

commit
> git commit -m "some infos about your changes"

show available branches
> git branch

make changes definitive to the default master branch
> git push origin master

# for multiple repositories with diferent ssh keys

create file ~/.ssh/config 

it should look like this

> Host repo_user_1.github.com  
>>  HostName github.com  
>>  IdentityFile ~/.ssh/key_repo1  
>>  IdentitiesOnly yes  

> Host repo_user_2.github.com  
>>  HostName github.com  
>>  IdentityFile ~/.ssh/key_repo2  
>>  IdentitiesOnly yes  

clone repos like this
> git clone git@repo_user_1.github.com:local-bot/repo1
> git clone git@repo_user_2.github.com:local-bot/repo2