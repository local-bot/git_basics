
# Setting shh enviroment

download repo
<pre>
git clone git@github.com:local-bot/git_basics
</pre>

setting user
<pre>
git config --global user.name "user"
git config --global user.emai "email@example.com"
</pre>

edit or add some files
<pre>
nano README.md
</pre>

include files to git in order to make changes to repo
<pre>
git add filename # or git add -A for all files
</pre>

undo includes
<pre>
git reset
git reset filename
</pre>

check changes made
<pre>
git status
</pre>

commit
<pre>
git commit -m "some infos about your changes"
</pre>

show available branches
<pre>
git branch
</pre>

make changes definitive to the default master branch
<pre>
git push origin master
</pre>

remove files from repository
<pre>
git rm file
git commit -m "Deleted the file from the git repository"
git push
</pre>

# for multiple repositories with diferent ssh keys

create file ~/.ssh/config 

it should look like this:

<pre>
Host repo_user_1.github.com  
    HostName github.com  
    IdentityFile ~/.ssh/key_repo1  
    IdentitiesOnly yes  

Host repo_user_2.github.com  
    HostName github.com  
    IdentityFile ~/.ssh/key_repo2  
    IdentitiesOnly yes  
</pre>

clone repos like this
<pre>
git clone git@repo_user_1.github.com:local-bot/repo1
git clone git@repo_user_2.github.com:local-bot/repo2
</pre>