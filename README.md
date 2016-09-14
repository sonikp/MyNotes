# MyNotes

Git + Homework

1. Create project in GitHub
2. Create project in eclipse
3. Within the eclipse workspace, in the project folder, initialize git:
$ git init

4. Register new project
$ git remote add origin https://github.com/sonikp/[reponame].git

5. Pull down project and info file from server
$ git pull origin master

6. Add all existing local files to the commit:
$ git add .      # this adds all the files

7. Make the initial commit, this stages all the files locally for the commit
$ git commit -a -m “Initial commit"

8. Move locally committed files to the remote project repo:
$ git push -u origin --all
