# git_assignment_HeroVired

1. Created a repository named "git_assignment_HeroVired" on GitHub
2. Then, clone the repository to your local machine and create a new branch named 'dev':
git clone https://github.com/karthicknath11205/git_assignment_HeroVired.git
cd git_assignment_HeroVired
git checkout -b dev
3. Added the provided code to the calculator.py file in your project directory.
4. Implemented the square root feature within calculator class
5. After implementing the feature, commit the changes and push the dev branch to the remote repository:(steps as shown below)
git add calculator.py
git commit -m 'Implemented sqrt feature'
git push origin dev
6. Then modified the divide function as given
7. Commit the changes and push them to the dev branch:
git add calculator.py
git commit -m 'Fixed divide bug'
git push origin dev
8. Create a new branch for sqrt feature
git checkout -b feature/sqrt
git add calculator.py
git commit -m 'Added sqrt'
9. Then critical bug is reported in the main branch, switched back to the dev branch, fixed the bug, and applied the changes to keep the feature branch up-to-date
git checkout dev
git pull origin dev
git add calculator.py
git commit -m'fixed bug'
git push origin dev
git merge --no-ff feature/sqrt
git push origin dev
git checkout main
git merge --no-ff dev
git tag -a v2.0 -m "merge V2 branch"
git push origin main --tags