## Fork a repo
A fork is a copy of a repository.

Forking a repository allows you to freely experiment with changes without affecting the original project.

1. On GitHub, navigate to the https://github.com/swachev/swachev-marketplace repository.
In the top-right corner of the page, click Fork.

![Screenshot](https://evliion.s3.amazonaws.com/fork-image-jpeg.jpg)

2. Create a local clone of your fork.
On GitHub, navigate to your fork of the swachev-marketplace repository.
Under the repository name, click Clone or download.

![alt tag](https://evliion.s3.amazonaws.com/clone-download-jpeg.jpg)

3. To clone the repository using HTTPS, under "Clone with HTTPS", click on Arrow sign to copy url.

![alt tag](https://evliion.s3.amazonaws.com/clone-with-https-jpeg.jpg)

4. Open Git Bash. Type git clone, and then paste the URL you copied earlier. It will look like this, with your GitHub username instead of YOUR-USERNAME:
```bash
$ git clone https://github.com/YOUR-USERNAME/swachev-marketplace
```

5. Press Enter. Your local clone will be created.
```bash
$ git clone https://github.com/YOUR-USERNAME/swachev-marketplace
> Cloning into `swachev-marketplace`...
> remote: Counting objects: 10, done.
> remote: Compressing objects: 100% (8/8), done.
> remove: Total 10 (delta 1), reused 10 (delta 1)
> Unpacking objects: 100% (10/10), done.
```
6. Open Git Bash. Change directories to the location of the fork you cloned in Step 2: Create a local clone of your fork.
Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.
```bash
$ git remote -v
> origin  https://github.com/YOUR_USERNAME/swachev-marketplace.git (fetch)
> origin  https://github.com/YOUR_USERNAME/swachev-marketplace.git (push)
```
7. Type git remote add upstream, and then paste the URL you copied in Step 3 and press Enter. It will look like this:
```bash
$ git remote add upstream https://github.com/swachev/swachev-marketplace.git
```
8. To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.
```bash
$ git remote -v
> origin    https://github.com/YOUR_USERNAME/swachev-marketplace.git (fetch)
> origin    https://github.com/YOUR_USERNAME/swachev-marketplace.git (push)
> upstream  https://github.com/swachev/swachev-marketplace.git (fetch)
> upstream  https://github.com/swachev/swachev-marketplace.git (push)
```
## Syncing a fork
Sync a fork of a repository to keep it up-to-date with the upstream repository.

Open Git Bash. 
Change the current working directory to your local project.
Fetch the branches and their respective commits from the upstream repository. Commits to master will be stored in a local branch, upstream/master.
```bash
$ git fetch upstream
> remote: Counting objects: 75, done.
> remote: Compressing objects: 100% (53/53), done.
> remote: Total 62 (delta 27), reused 44 (delta 9)
> Unpacking objects: 100% (62/62), done.
> From https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY
>  * [new branch]      master     -> upstream/master
```

## Creating Pull Request
https://jarv.is/notes/how-to-pull-request-fork-github/
