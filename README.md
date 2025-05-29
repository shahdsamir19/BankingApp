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

