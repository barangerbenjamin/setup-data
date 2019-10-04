# Setup instuctions

The following instructions will help you get your machine ready for the bootcamp.

# Anaconda

Anaconda is the world's most popular data science platform.

Go to [anaconda's website](https://www.anaconda.com/distribution/) and click on `Download` under "Python 3.7".
Open the file downloaded.

Click on next, then accept the License Agreement, then next until you reach "Advanced Installation Options". Check "Add Anaconda to my PATH environment variable", click on Install.

Click on finish.

Once Anaconda is installed, press Start and look for "Control Panel"

Click on System and Security, click on System, click on Advanced System Settings and finally click on Environment Variables.

Locate "Path" then click on it to select it then click on Edit.

Click on "New" then type "C:\Users\your-windows-username\Anaconda3\Scripts"

Click on OK.

# Git Bash

Git bash will allow you to run some linux command on Windows
Go to [Git-SCM](https://git-scm.com/download/wim), the download should start automatically. If not you can click on "64-bit Git for Windows Setup".
Install it following the instructions on the screen leaving everything by default.
When the installation is finished, Git Bash should start on his own.

Run the following commands:

```bash
cd
touch .bashrc
```
You should be prompted telling you that a file bash_profile will be created for you to load your bashrc profile.
Close Git bash by typing

```bash
exit
```

Click Start, search for "Git Bash", right click, "Run as administrator"
Run the following command:

```bash
echo 'export PATH="~/./Anaconda3/:${PATH}"
```

Re-open Git Bash the same way as above, and this time run the command:

```bash
conda init bash
```

Restart another time Git bash and run:

```bash
conda activate base
```

Restart your terminal a last time and run:

```bash
conda install pytest
conda install pylint
```

To make sure everything is properly set, please run the command:

```bash
python -i
```
 it should give you an answer like "Python 3.7.3..." 
# Make

Make is a build automation tool that build executable.
Go to this [url](https://sourceforge.net/projects/ezwinports/files) and click on "make-4.2.1-without-guile-w32-bin.zip"

The download will start shortly, save the file.

Go to the folder where the file has been saved, probably "Downloads" and right click on it and choose "Extract All..." then click on "Extract"

A new explorer window will open with several directories in it. Select them all and copy them.

In an explorer windows, go to "C:\Program Files\Git\mingw64" and merge the directories with those already there.
Do not replace existing file/folder.

If it is open, restart your Git Bash.

Typing the command:
```bash
make -v
```
It should give you an answer like "GNU Make 4.2.1", if not please ask a teacher.

# Check

To make sure you're setup correctly, please run the following command:
```bash
jupyter notebook
```

It shoul open your default browser to "localhotst:8888/tree". If not please ask a teacher.
