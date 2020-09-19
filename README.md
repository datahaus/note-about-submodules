# Use of submodules

https://stackoverflow.com/questions/8212800/how-do-submodules-behave-in-github-pages

The "Site" repo is NOT currently using submodules. 
(It's easier to pull external repos into Site and add to .gitignore)

Later we may use the following:

To add as a submodule to your existing project, run the following command in your local project folder.
When you deploy, only the submodule reference will reside in your GitHub repo.

git submodule add https://github.com/[your site]/site.git site

Avoid editing a submodule inside another repo. Otherwise conflicts will occur when commiting.

Try running:

git submodule init
git submodule update - to get data

https://git-scm.com/book/en/v2/Git-Tools-Submodules

To update your submodules to the latest version, run:
git submodule foreach git pull origin master
