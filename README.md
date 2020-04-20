# Covid19







* HELP ON git
choose a folder in the terminal and do 
git clone https://github.com/JoaoCanhoto/Covid19.git

(1) and do:
git config --global user.name "Arnaud blabla"
git config --global user.email arnaud@example.com
to set your name...
(with the global, your pc git will remember you for others gits you may create in the future,
so you don't need to set your name again)

(1.1) then do:
git status
to see the status of the git

(2) do 
git pull
to be sure you have everything, which is there

(3) than create you branch, which is the place where you work:
git branch arnaud_branch

(4) to enter in your branch do:
git checkout arnaud_branch
now the changes will be made in your branch 
the top one, or the original if called master, 
but working in your branch, git does a copy of everything and makes the original files in master invisilbe

if you want to go back to master you can do 
checkout master
and the files in your branch become invisible and you see the files in master
(so a new file you have add in the branch, you cannot see it anymore )

(5) create a file arnaud.txt and write something
(6) do 
git status
you sill see in red that you change or created a new file which was not in the branch or master (it should be written there)

(7) after you are happy with the changes do the steps until 10
git add arnaud.txt [OTHER FILES]
git don't know if the change you made or the new file is suppose to go online
so you have to add that files or files

(8) to see if you add all files you need, do:
git status
the files you change/add, that git considers to send online will be in green

(9) you need to say something about what you changed, and say you are ok with the current changes, (usually means the code can run), so do:
git -m commit "add file arnaud.txt"

(9) you can do git status again to check

(10) now do:
git push
this means you sent the files to the repository online


now, you only did these changes in your branch,
now you should go to the website and
cick banchs -> click your branch ->  do a pull request
the pull request will merge your changes with master


#*****************************************************
If you already did the commit and push
before you make more changes,
maybe someonelse already change thing and update them on the repository online
so change your branch tp master to copy the new things
git checkout master
git pull
(to bring to your computer the new changes in master
then go back to your branch
git checkout arnaud_branch
the do
git merge master
(this will bring the new changes in master to your branch)
(we after you can continuing doing the changes)
After you change go to number (7)

