# lab8echo "hello" > a.txt
git add a.txt
git commit -m "first commit"
git switch -c feature
echo "feature work" > b.txt
git add b.txt
git commit -m "add feature"
git switch main
echo "main work" >> a.txt
git commit -am "update main"
git merge feature -m "merge feature"
git branch -d feature
git push origin main
clear
git log --oneline --decorate --graph --all
