"# Banking App" 
mkdir banking-app
cd banking-app
git init
git remote add origin https://github.com/shahdsamir19/BankingApp
echo "# Banking App" > README.md
git checkout -b main
git checkout -b develop
git checkout main
echo "This is file f1 on main" > f1.txt
git add f1.txt
git commit -m "Add f1 file on main branch"
git checkout develop
echo "This is file f1 on develop" > f1.txt
git add f1.txt
git commit -m "Add f1 file on develop branch"
git checkout -b login-feature
echo "Implement the login functionality" >> f1.txt
git add f1
git commit -m "Implement login functionality"
git push -u origin login-feature
git checkout development
git add f1.txt
git commit -m "Update f1.txt in development branch"
git merge login-feature
git add f1.txt
git commit -m "Resolve merge conflict between login-feature and development"
git push
git checkout development
git merge login-feature
git push
git branch -d login-feature
git push origin --delete login-feature
git checkout development
git pull
git checkout -b release-v1.0
git push -u origin release-v1.0
git checkout login-feature
echo "Case 1" >> f1.txt
git add f1.txt
git commit -m "Add Case 1 to f1"
echo "Case 2" >> f1.txt
git add f1.txt
git commit -m "Add Case 2 to f1"
echo "Case 3" >> f1.txt
git add f1.txt
git commit -m "Add Case 3 to f1"
git push
git checkout release-v1.0
git log login-feature-case --oneline
git cherry-pick b7ad085
notepad f1.txt
git add f1.txt
git commit -m "Resolve merge conflict"
git cherry-pick cac6559
notepad f1.txt
git add f1.txt
git commit -m "Resolve merge conflict"
git push
git checkout main
git merge release-V1.0
notepad f1.txt
git add f1.txt
git commit -m "Resolve merge conflict"
git checkout development
git merge release-V1.0
notepad f1.txt
git add f1.txt
git commit -m "solving merge conflict"
git branch -D release-V1.0
git checkout main
git checkout -b hotfix/login-security
git add f1.txt
git commit -m "fix(security): patch login vulnerability with input validation"
git checkout main
git merge hotfix/login-security
git checkout development
git merge hotfix/login-security
git branch -d hotfix/login-security
git push origin main
git push origin development
git checkout development
git log --oneline --graph --all
git rebase -i b7ad085





