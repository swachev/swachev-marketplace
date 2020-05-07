# swachev-marketplace
Online marketplace

## Steps to Setup the Spring Boot Back end app (evliion-app-server)

1. **Clone the application**

	```bash
	git clone git@github.com:swachev/swachev-api.git
	cd evliion-app-server
	```

2. **Create MySQL database**

	```bash
	create database evliion_app
	```

3. **Change MySQL username and password as per your MySQL installation**

	+ open `src/main/resources/application.properties` file.

	+ change `spring.datasource.username` and `spring.datasource.password` properties as per your mysql installation

4. **Run the app**

	You can run the spring boot app by typing the following command -

	```bash
	mvn spring-boot:run
	```

	The server will start on port 8080.

	You can also package the application in the form of a `jar` file and then run it like so -

	```bash
	mvn package
	java -jar target/ev-0.0.1-SNAPSHOT.jar
	```


Fork a repo
A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.

On GitHub, navigate to the octocat/Spoon-Knife repository.
In the top-right corner of the page, click Fork. 

Step 2: Create a local clone of your fork
Right now, you have a fork of the Spoon-Knife repository, but you don't have the files in that repository on your computer. Let's create a clone of your fork locally on your computer.
On GitHub, navigate to your fork of the Spoon-Knife repository.
Under the repository name, click Clone or download. 


To clone the repository using HTTPS, under "Clone with HTTPS", click . To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click . 


Open Git Bash.
Type git clone, and then paste the URL you copied earlier. It will look like this, with your GitHub username instead of YOUR-USERNAME:
$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
Press Enter. Your local clone will be created.
$ git clone https://github.com/YOUR-USERNAME/Spoon-Knife
> Cloning into `Spoon-Knife`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.

Open Git Bash.
Change directories to the location of the fork you cloned in Step 2: Create a local clone of your fork.
To go to your home directory, type just cd with no other text.
To list the files and folders in your current directory, type ls.
To go into one of your listed directories, type cd your_listed_directory.
To go up one directory, type cd ...
Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.
$ git remote -v
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
Type git remote add upstream, and then paste the URL you copied in Step 2 and press Enter. It will look like this:
$ git remote add upstream https://github.com/octocat/Spoon-Knife.git
To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.
$ git remote -v
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
> origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
> upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)

Syncing a fork
Sync a fork of a repository to keep it up-to-date with the upstream repository.

Open Git Bash.
Change the current working directory to your local project.
Fetch the branches and their respective commits from the upstream repository. Commits to master will be stored in a local branch, upstream/master.
$ git fetch upstream
> remote: Counting objects: 75, done.
> remote: Compressing objects: 100% (53/53), done.
> remote: Total 62 (delta 27), reused 44 (delta 9)
> Unpacking objects: 100% (62/62), done.
> From https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY
>  * [new branch]      master     -> upstream/master
Check out your fork's local master branch.
$ git checkout master
> Switched to branch 'master'
