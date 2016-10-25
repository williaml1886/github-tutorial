# GitHub Tutorial

_by William Law_

---
## Git vs. GitHub

  * Git is basically like a version control that keeps snapshots of "code". Git also runs in the command line, and makes a basic workflow.
  
  * Github stores code in the cloud, and can visually track changes you've made. Github can also easily collaborate on files, but must require Git.
  
---
## Initial Setup
  * Before you initialize, you must make sure [you are logged into your account](hstat.org/sep11). In order to initialize, you must make a new folder, typing `mkdir <directory-name>`. However, you're not done yet! You need to run the code, by using and typing `git init` into a directory or repository. After you initialize in the directory or repository using the input `git init`, 
you'll notice that more Git commands, such as `git status`, `git add`, `git commit`, `git push`, and `git pull` are acceptable commands to use.

---
## One-Time Setup
  * To create a Github account, make sure you are using your _school account_. You can create a Github account using your school account [<first-and-last-name-and-last-4-digit-numbers-of-your-ID>](hstat.org/first-name-last-name-initial-last-4-digit-numbers-of-your-ID) However, if you are new to Github and don't utilize the school account, you are free to choose a username for your own desire, but PLEASE, ensure it is appropriate. After entering your username, you must then enter your e-mail that you use daily, as _Github will occasionally, or seldomly, e-mail you notifications_ you don't want to miss. After entering your e-mail, now create a password. You must enter a password that you can remember. It must be more than, or at least, seven characters, with 1 letter being _lowercase_ and the rest being uppercase, and don't forget to add a number next to your last name. It's your choice how you want to configure your password, but please, when entering a password when signing up, make sure to write it down so you don't forget.
  * Now, before you're a few steps away to set up a repository, you're on step 2. Select "Unlimited public repositories for free".
  * Now that you're a step away, you may answer your "Tailor your experience" answer; however, it is not required. You may also skip this step if you wish. After that, you're all  **SET UP!!!** You are now ready to make and set up a repository for the first time.
  
  * ---
  
## Repository Setup  
  * Now that you've successfully set up your account, you'll want to get started on creating a new repository. Go to Github. Click on the top right, which is the icon of your profile, then click on **Settings**.
    * _Command syntax_
        * Insert Snapshot
  * Now that you're on Settings, go to the left sidebar, and click _SSH and GPG keys_. After you click on _SSH and GPG Keys_, look for the **New SSH key** and click on it. Always type "Cloud9" as the title.
    * _Command syntax_
        * Insert Snapshot
  * Next, for the key, navigate to your cloud 9 tab. Navigate to the top-right, where you will see the gear icon.
    * _Command syntax_
        * Insert snapshot
  *Now that you're in Settings, go to the left sidebar and click on SSH keys tab. This is when you'll copy and paste your SSH key from your Cloud9 into your Github repository. ** Please note that **every SSH keys** begin with `ssh-rsa`. After you copy and paste your entire ssh-rsa key code from cloud9 to Github, click on  
**Add SSH Key**. After that, navigate back to Cloud 9 and open your "github learning" IDE. Note: To set up a new repository or edit, ensure you're logged into Github. If not, log in now.
    * _Command syntax_
        * Insert snapshot
  * Click on the green button that states `New Repository`.
    * _Command syntax_
        * Insert snapshot
  * Name your repository something that **associates with what you'll be working on in your repository.** _Always leave your repositories public and leave `Initialize this repository with a README unchecked._
    * _Command syntax_
        * Insert snapshot
  * _ALWAYS_ **make sure you have SSH key selected**. You may want to save your repository and clone it to your Cloud9 by copying and pasting the texts from the "...or push an existing repository from the command line" column. This is when you'll paste and enter your Github info. This includes your e-mail and password you used to sign in to Github.
    * _Command syntax_
        * Insert snapshot
  * After you enter your Github e-mail and password, you will receive a text statement, saying, "Hi <username>! You've successfully authenticated, but Github does not provide shell access." This is when you hit `git init`, then you `git add .` before you enter `git commit -m "message"`. For the message, try thinking of something appropriate and/or meaningful to put for your message. Don't enter messages like, "Complete" or "Brooklyn down". This will cause confusion and errors to take place in your repository. The best messages to use are such, but unlimited to: "Create empty file structure", "Remove extra whitespace", "Change dark reds to navy blues", "Refactor to use hashes instead of arrays", etc.
    * _Command syntax_
  * After you commit, refresh your Github page. Notice that there will be a new change, with a new Github repository with a new name.

---

## Workflow & Commands
  * The command `status` checks the status of a file. By way of example, untracked files would be shown in **RED**, while the tracked ones are represented in **GREEN**. This is done by entering `git status`, which then enters and shows tracked and untracked file(s).
    * Command syntax
        * Insert snapshot
  * The command `add` adds changes to the file to be committed. As an illustration, if you were to perform a file commit using `git add`, you would enter `git add file`. This is similar to how you would add people into a photo.
  * The command `git commit -m "message"` takes snapshots of the stage and adds it to the timeline. This is done by simply typing `git commit -m "message"` before entering it. Now, pay ***CLOSE ATTENTION*** to the `"message"`part. This is where you need to pause and think of a meaningful and specific message to put in `"message"`. As mentioned earlier before, don't put things like, "Change stuff", "Work on code", etc. The most meaningful messages are, but not limited to, such things as "Removed extra comma", "Removed file fork-practice", etc.
  * Using command `git push`, it pushes the information you changed from cloud9 to Github. For example, after you initialize, you push your Cloud9 project to Github. Therefore, Github now has your remote repository that you pushed your Cloud9 project from. However, you may receive an error, stating "git push -u origin master
Warning: Permanently added 'github.com,207.97.227.239' (RSA) to the list of known hosts.
Permission denied (publickey).
fatal: The remote end hung up unexpectedly".

---

## _Extra Credit_

* Error handling
    * If there is this one moment you do `git init` in a wrong directory, you'll see a code displaying, "initialized empty Git repository in /path/to/folder/.git/". However, don't despise yourself for it and give up! The only reason why this happens is because there's a hidden .git folder. We can fix it. We just simply need to type in `rm -rf .git` to remove the hidden .git folder.
        * Command syntax
            * Insert snapshot
* Collaboration
    * To fork and clone, click on `Explore Github`. Browse on any topics, and when you want to find more, click on `More Showcases >`. Just continue browsing and when you come into a topic that most interests you, click on the username/topic file. There, you will find a README file, and click on it to read. Then after that, click on `Fork`. It should only take a few seconds. After that, you'll find the `_"Clone & Download"_` icon. Click on it, and there, you will find the SSH key to the file you selected. The URL text, stating "git@github.com:,<first-name-and-initial-of-last-name-and-last-4-digits-of-your-ID-number>/<topic>.git" is the exact SSH key to the original creator's file, so click on that text, and copy. Then, navigate back to your Cloud9 tab, and paste at once, using only the `Ctrl + V` keys by pressing at the same time.
    * Make sure that in Cloud9, you are in the directory where you want the Github repository you are cloning to go in.
