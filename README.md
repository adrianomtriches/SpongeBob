# SpongeBob


**Git commands**

- To work in other projects: -> click in fork, add the project to your account. Get the link of the repo. then on the terminal use the command "git clone <repolink>"
- Git status "red === changes were made but not added" - "green === changes were added"
- Git add <name of the file> or just, git add . “With a space and a dot to select all files that you made changes to it”
- Git Status “status should’ve changed to green”
- Git commit -m “add your msg here, changes you made”
- Git push “pushes the code into GitHub”
- Git push origin <name of the branch> "pushes to your fork and to the original repo that you are contribuiting as well".
- Git pull “updates to the most current changes on the document”

- Git checkout -b <name of the branch> “Creates a new Branch and switches to the branch”
- Git branch <name of the branch> “creates a new branch but doesn’t switches to it”.
- Git checkout <name of the branch> “switches to the branch”
- Git diff “shows the changes you made”

Good practice:
- Before merging code from a branch into the master branch it’s good to switch to the master branch and do a pull after you have added and committed, just to make sure you don’t get any conflicts on the code.
- Than switching back to the branch and “git merge master” into the branch to visually see any conflicts in the code, in the text editor.

****Keeping Your Fork Up To Date****
You may have noticed something while watching the previous videos...Do you have to always fork the Open Source project every time master get's updated? What happens if somebody makes an update to the original project and now your forked project is out of sync and outdated? Luckily for you, there is an easy way to always make sure your fork has the most up to date version of the original project. Here is how:

Once you are in your forked project directory in your command prompt....


Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.

git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
Type git remote add upstream, and then paste the URL you would copy from the original repository if you were to do a git clone. Press Enter. It will look like this:

git remote add upstream https://github.com/zero-to-mastery/PROJECT_NAME.git
To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.

git remote -v
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
Now, you can keep your fork synced with the upstream repository with a few Git commands.

One simple way is to do the below command from the master of your forked repository: 

git pull upstream master
Or you can follow along another method here: "Syncing a fork."

Source: https://www.udemy.com/course/the-complete-web-developer-zero-to-mastery/learn/lecture/16539458#overview
