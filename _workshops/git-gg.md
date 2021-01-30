---
title:  Git Workshop with Git Gud
published: true
date:   2021-01-30
author:
- Sahan Kumarasinghe
slides:
    link: "https://docs.google.com/presentation/d/13fXG9FAndd5ZCeKH9VXZ3Gm9_lata4HrOjWbEaqmbcE/edit?usp=sharing"
objective: 
    summary: "Learn how to use Git interactively using Git Gud."
software:
    - name: Git
      homepage: https://git-scm.com
      installing: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
    - name: Python
      homepage: https://www.python.org/
      installing: https://www.python.org/downloads/
    - name: Git Gud
      homepage: https://github.com/benthayer/git-gud/
instructions:
    - Present the slides for 15 minutes, and then let members explore Git using Git Gud.
---
# Install Instructions for Linux and MacOS Users
You probably already have `python` and `git` working on your system. Run `pip install --user git-gud` to install Git Gud.

# Install Instructions for Windows Users
Windows users have a lot more setup to do, but this is the least painful and intrusive method to go about it.

## Step 1/2 - Installing Software
1. Install Git Bash (install link above). When going through the installer, be sure to check the "Get daily updates for Git Bash" option (or whatever the most similar option is).
1. Install Python (install link above). The standard install for all users is fine. Do *not* add to PATH, since that apparently messes up your IDEs.

## Step 2/2 - Adding Python and Pip to Git Bash
1. Go to the Windows Start Menu, and start typing "Python" in the box. Right click one of the consoles that appears, and click "Open File Location".
1. When the folder is opened, right click the shortcut icons there, and click "Open File Location".
1. You should now appear at some folder with a bunch of executables and whatnot. Right click anywhere in the window, and in the context menu that appears, click "Open in Git Bash".
1. Run the command:
```sh
pwd
```
Your current directory will appear in the form `/path/to/python install/PythonXX`. We will tell Git Bash that our Python is located here in the next few steps. In the following commands, replace `/path/to/python install/PythonXX` with the *actual* result of `pwd`.

1. Run the command:
```sh
echo 'export PATH=$PATH:"/path/to/python install/PythonXX"' >> ~/.bashrc
```
This `~/.bashrc` file will run every time you open a new Git Bash window. We're telling Git Bash that every time we open a window, we want to add this directory to our PATH so Git Bash knows what to look for.

1. Test this by running `source ~/.bashrc`. If this works without error, run `python --version`. If there is no error, then congrats! Your Git Bash window knows there is Python here.

1. Now, we will do the same for `pip`, the Python package manager. We need this to install Git Gud in the first place. Run the same command as before, except add `/Scripts` to the end, like so:
```sh
echo 'export PATH=$PATH:"/path/to/python install/PythonXX/Scripts"' >> ~/.bashrc
```
This is where Python has installed `pip`.

1. Test this by running `source ~/.bashrc`. If this works without error, run `pip --version`. If there is no error, then congrats! Your Git Bash window knows there is `pip` is here too.

1. Now, run `pip install --user git-gud` to install Git Gud. After that, you're good to go!

NOTE: There's a bug on Windows where you must run `winpty` before `git gud` in order for `git gud` to work properly. Rather than typing this all the time, just run this command to make Git Bash do the work for you (so you don't ever have to think about this):

```sh
echo 'alias git="winpty git"' >> ~/.bashrc
```

After running this, close and reopen your Git Bash window to let the changes take effect.