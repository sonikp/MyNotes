# MyNotes

# Git + Homework

1. Create project in GitHub
2. Create project in eclipse
3. Within the eclipse workspace, in the project folder, initialize git:
$ git init

4. Register new project
$ git remote add origin https://github.com/sonikp/[reponame].git

 4a. Instead of removing and re-adding, you can do this:
 $ git remote set-url origin git://new.url.here

 4b. Check Origin and remove
 $ git remote -v
 $ git remote rm origin

5. Pull down project and info file from server
$ git pull origin master

6. Add all existing local files to the commit:
$ git add .      # this adds all the files

7. Make the initial commit, this stages all the files locally for the commit
$ git commit -a -m “Initial commit"

8. Move locally committed files to the remote project repo:
$ git push -u origin --all

# Alternate Git Options
Pull from repo while ingoring local changes:

1. Fetch all changes:
$ git fetch --all

2. Register the master:
$ git reset --hard origin/master

3. Pull update:
$ git pull origin master

4. Remove repository:
$ git rm -f -r *
$ rm -rf .git*

# Eclipes import the additional class files for the projects:

I've had a play with Eclipse to work this one out. Give the following a go:

1. Create the following directory structure (your desktop will do) classes/lec/utils
2. Place the InputReader class file in the utils directory.
3. Remove any references you have to InputReader you currently have in your build path.
4. Using (right click on project) Properties->Java Build Path->Libraries select the 'Add external class folder' and select the 'classes' folder you created on your desktop and click OK.
5. Now in the 'Referenced Libraries' in the project folder you should have one called 'classes' and a package path under that called 'lec.utils' which contains the InputReader class.
6. You can use that class using 'import lec.utils.InputReader' in you own class.

From:
http://stackoverflow.com/questions/2172916/how-to-use-external-class-files-in-an-eclipse-project

# Eclipse
Run
L: F11
M: crtl + shift + mac + F11

Menu:
ctrl + space

# Java for MAC
There are two Java source, the MAC one and the Oracle one. It is recommended to use the Oracle one.
Updating Java version(Oracle):

1. Download Oracle Java for MAC "jdk-XXX-macosx-x64.dmg"

2. Execute and install file. Installs to /Library/Java/JavaVirtualMachines

3. Check java -version on command line

4. Check java version using:# echo $JAVA_HOME 

5. Update path for java in user's home directory ~/.bash_profile 

	export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_111.jdk/Contents/Home

6. Update path for java in user's home directory ~/.profile

	export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_111.jdk/Contents/Home

