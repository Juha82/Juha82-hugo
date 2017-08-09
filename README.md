Juha82 pages

setup:

git clone http://github.com/Juha82/juha82-hugo.git
cd juha82-hugo
git subtree add -P public http://github.com/Juha82/juha82.github.io.git master --squash
git remote add juha82 http://github.com/Juha82/juha82.github.io.git
deploy:

hugo
git add .
git commit -m "update"
git push origin master
git subtree push -P public juha82 master