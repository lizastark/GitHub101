# GitHub 101
**A place to teach and learn GitHub**

*A place for personal reminders and instructions to use GitHub. 'Cause we all forget sometimes.*

It is my intention to keep these instructions in very plain language for beginners. 

## Creating a Repo
### Overview
- What is the deal with all this language?! What is a repository? What is a directory? What is a project? What is a folder?
- What components and properties does it have?
- Is there anything I need to do before I create a repo?

### Steps
**1. Create a new repository on GitHub**

**2. Add files before saving**
- .readMe
- .gitignore
- license (MIT?)
    
**3. Click "Clone/Download"**
- Use SSH (only if password is already set up) and copy link.

**4. Copy link**

**5. Open terminal and cd into folder/directory where you want to store it**
- I store all my repositories in a folder called 'GitHub' to keep them tidy, so my terminal command would look like `cd GitHub`
- *Remember: Directories can be anywhere AND do not put repos inside repos.*

**6. Type git clone command in terminal and copy link**
- It will look something like this: `git clone git@github.com:username/repoName.git`

### Other Links
- [Start a new github repository](https://kbroman.org/github_tutorial/pages/init.html)

## Pushing to a Repo
### Overview
- Why do I want to push to a repo? 
- How do you connect a local and remote repository?
- What is actually happening in these steps?

### Steps
**1. Add files to a directory**
**2. Open terminal and cd into the local directory of the repository you want to push to** 
- For example, if I wanted to update files I had added into my shiny new GitHub101 repo, my commands would look like this:
    - `cd` - Get back into my main home directory (i.e. the very top of the file tree)
    - `cd GitHub` - change directories into the folder where I store all my GitHub repos. If you store them in a folder that is directly in your home directory, then you don't need to do this. Basically, you have to work your way down the file tree until you're in the folder that contains the repo you want to push to.
    - `cd GitHub101` - change directories into the folder where the project is stored.
**3. Type the following commands:**
- `git status` - check the status of the repo
- `git add -A` - add *all* changes in directory to commit
- `git commit -m "Type your message here"` - commit changes with a message
- To push the changes, you have two options: *(Note - add another section on branches later)*
    - `git push` - assumes that you already have a remote repository defined for that branch
    - `git push origin master` - indicates that you are pushing to a specific remote repo - in this case `origin`
    - If you're only committing to one GitHub repository, then it doesn't really matter which one you use.
- `git status` - check status again to make sure all changes went through
    
### Other Links
- [Git Gud: The Working Tree, Staging Area, and Local Repo](https://medium.com/@lucasmaurer/git-gud-the-working-tree-staging-area-and-local-repo-a1f0f4822018)

## Terminal Command Cheatsheet
- **pwd** - full path to working directory
- **cd** - home directory
- **cd foldername** - change directory into that folder
- **cd /** - root of drive
- **cd ..** - move *one* level up
- **cd ../../** - move *two* levels up
- **ls** - list files in that directory
- **ls -l** - long list
- **ls -a** - list with invisible files
- **clear** - clear screen
