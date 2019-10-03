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

Click start, search for Git Bash, right click, "Run as administrator"
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

