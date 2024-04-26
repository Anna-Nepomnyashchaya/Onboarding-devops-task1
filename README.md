git init "home_work"
cd home_work
git remote add origin git@gitlab.wildberries.ru:nepomnyaschaya.a2/onboarding-devops-task1.git
git add .
git commit -m "Initial commit"
#git push --set-upstream origin master
#git remote rename origin old-origin
git remote add origin-github git@github.com:Anna-Nepomnyashchaya/Onboarding-devops-task1.git
git push -u origin-github main
git clone git@gitlab.wildberries.ru:ilin-leonid/git-checkout.git
git checkout dfbdad
git show
