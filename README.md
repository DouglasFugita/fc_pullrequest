## Full Cycle - Pull Requests

```
echo "# fc_pullrequest" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/DouglasFugita/fc_pullrequest.git
git push -u origin main
git checkout -b develop
git push origin develop
```

* Settings > Branches > 
    * Default - develop
    * Branch protection rules

```
git checkout -b feature/contact
touch contact.html
git add .
git commit -m 'add contact'
git push origin feature/contact
```

* Compare & pull request
* Merge
* Delete branch

```
git checkout develop
git pull origin develop
git branch -d feature/contact
```

```
git checkout -b feature/pr
mkdir .github
cd .github
touch PULL_REQUEST_TEMPLATE.md >> Conteudo: https://embeddedartistry.com/blog/2017/08/04/a-github-pull-request-template-for-your-projects/
git add .
git commit -m 'Add PULL_REQUEST_TEMPLATE'
git push origin feature/pr
git checkout develop
git pull origin develop
git branch -d feature/pr
```

