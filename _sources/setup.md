# Setup for the workshop

There are four ways how you can follow this workshop:

1. Via `Conda` (`Python`): Full workshop experience, interactive, with only `Python` based software dependencies.
2. Via `Mybinder`: Full workshop experience, interactive and online, with restricted computational power.
3. Via `JupyterBook`: Only visual exploration of the workshop content, no interactive aspect.

<div style="text-align: justify;">

While option 2. is nice and easy to follow in an interactive manner and option 3. might work for a quick overview, we don't recommended either of them as getting `Python` to work
reliably on your machine is going to be very beneficial. This holds true for the workshop and especially beyond. Via installing these tools, you will be equipped to basically continue right
away and start using them and thus ML/DL on your everyday research workflow. Having that in mind and integrating other tools/resources focusing open and reproducible (neuro-/data) science, we
generated a rather comprehensive set of install instructions below. While not all of them might be totally necessary for the workshop, they all will help you a great deal going further and 
are especially useful/needed if we have to hold the workshop virtually or if you can only attend virtually.  

Don't worry, you got this!

</div>

![logo](https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805)\
<sub><sup><sub><sup>https://media1.tenor.com/images/f72cb542d6b3e3c3421889e0a3d9628d/tenor.gif?itemid=4533805</sup></sub></sup></sub>


## General things

<div style="text-align: justify;">

There are a few computing requirements for the course that are absolutely necessary (beyond the few software packages we would like you to install, described below):

</div>

1. You must have administrator access to your computer (i.e., you must be able to install things yourself without requesting IT approval).
1. You must have at least 20 GB of free disk space on your computer (but we would recommend more, to be safe).
1. If you are using Windows you must be using Windows 10; Windows 7 and 8 will not be sufficient for this course.

<div style="text-align: justify;">

If you foresee any of these being a problem please reach out to one of the instructors for what steps you can take to ensure you are ready for the workshop start.

</div>

## Installation office hours

<div style="text-align: justify;">

If you are having trouble installing the software, we will be holding virtual installation office hours on the following date: Monday, 24.02.2025, 9 - 10 AM (CET). You will get the `zoom link` via Email from the organizers.

</div>

<div style="text-align: justify;">
If you can't attend the office hour, please reach out to Peer Herholz (herholz dot peer at gmail dot com) to get an invite a 1-1 `zoom` meeting.

</div>


## Required software

To get the most out of our course, we ask that you arrive with the following software already installed:

- A command-line shell: `Bash`
- A version control system: `Git`
- A remote-capable text editor: `VSCode`
- Python 3 via `Miniconda`
- A modern browser

<div style="text-align: justify;">

If you already have all of the above software tools/packages installed, or are confident you’ll be able to install them by the time the course starts, you can jump straight to [checking your install](#checking-your-install).
The rest of this page provides more detail on installation procedures for each of the above elements, with separate instructions for each of the three major operating systems (Windows, Mac OS, and Linux).

</div>

### Some quick general notes on instructions

- There is no difference between `Enter` and `Return` in these instructions, so just press whatever the equivalent on your keyboard is whenever one is stated
- If you already have some of these things installed on your computer already that should (theoretically) be okay.
  However, you need to make sure that you are able to complete the steps described in [checking your install](#checking-your-install) without issue.
  - For example, having multiple different Python installations on your computer can lead to incredibly frustrating issues that are very difficult to debug.
    As such, if you have already installed Python via some other application (not Miniconda/Anaconda), we strongly encourage you to uninstall it before following the instructions below.
    You _must_ have Python installed via Miniconda for this course.

### OS-specific installation instructions

Please select the tab that corresponds to your operating system and follow the instructions therein.

````{tab-set} 
```{tab-item} Windows
**Windows Subsystem for Linux (WSL)**

1. Search for `Windows Powershell` in your applications; right click and select `Run as administrator`.
   Select `Yes` on the prompt that appears asking if you want to allow the app to make changes to your device.
2. Type the following into the Powershell and then press `Enter`:

        Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux

3. Press `Enter` again when prompted to reboot your computer.
4. Once your computer has rebooted, open the Microsoft Store and search for "Ubuntu."
   Install the program labelled "Ubuntu 22.04" (not "Ubuntu 16.04" or "Ubuntu") by clicking the tile, pressing `Get`, and then `Install`.
5. Search for and open Ubuntu from your applications.
   There will be a slight delay (of a few minutes) while it finishes installing.
6. You will be prompted to `Enter new UNIX username`.
   You can use any combination of alphanumeric characters here for your username, but a good choice is `<first_initial><last_name>` (e.g., `jsmith` for John Smith).
   You will then be prompted to enter a new password.
   (Choose something easy to remember as you will find yourself using it frequently.)
7. Right click on the top bar of the Ubuntu application and select "Properties".
   Under the "Options" tab, under the "Edit Options" heading, make sure the box reading "Use Ctrl+Shift+C/V as Copy/Paste" is checked.
   Under the "Terminal" tab, under the "Cursor Shape" heading, make sure the box reading "Vertical Bar" is checked.
   Press "Okay" to save these settings and then exit the application.

(The above step-by-step WSL instructions are distilled from [here](https://docs.microsoft.com/en-us/windows/wsl/install-win10) and [here](https://docs.microsoft.com/en-us/windows/wsl/initialize-distro).
If you have questions during the installation procedure those resources may have answers!)

From this point on whenever the instructions specify to "open a terminal" please assume you are supposed to open the Ubuntu application.

**Bash shell**

You already have it, now that you’ve installed the WSL!

**Git**

You already have it, now that you’ve installed the WSL!

**VSCode**

1. Go to https://code.visualstudio.com/ and click the download button, then run the `.exe` file.
1. Leave all the defaults during the installation with the following exception:
      - Please make sure the box labelled "Register Code as an editor for supported file types" is selected

**VSCode extensions**

1. Open the Ubuntu application.
1. Type `code .` into the terminal and press `Enter`.
   You should see a message reading "Installing VS Code Server" and then a new windows will open up.
1. Press `Ctrl+Shift+P` in the new window that opens and type "Extensions: Install extensions" into the search bar that appears at the top of the screen.
   Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads "Extensions: Install extensions").
1. A new panel should appear on the left-hand side of the screen with a search bar.
   Search for each of the following extensions and press `Install` for the first entry that appears. (The author listed for all of these extensions should be "Microsoft".)
      - Python (n.b., you will need to reload VSCode after installing this)
      - Live Share (n.b., you may need to press "Ctrl/Cmd+Shift+P" and type "install extensions" again after installing this)
      - WSL
      - Remote Development

**Python**

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
        bash Miniconda3-latest-Linux-x86_64.sh

1. A license agreement will be displayed and the bottom of the terminal will read `--More--`.
   Press `Enter` or the space bar until you are prompted with "Do you accept the license terms? [yes|no]."
   Type `yes` and then press `Enter`
1. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`).
   Leave this default and press `Enter`.
1. When you are asked "You can undo this by running `conda init --reverse $SHELL`? [yes|no]" type `no` and press `Enter`.
   Exit the terminal once the installation has finished.
1. Re-open the Ubuntu application.
   Type `which python` into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
   - If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
     If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel on the BHS Slack.
1. Type the following to remove the installation script that was downloaded:

        rm ./Miniconda3-latest-Linux-x86_64.sh


**Python packages**

Open a terminal and type the following commands:

        conda config --append channels conda-forge
        conda config --set channel_priority strict
        conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```

```{tab-item} Linux
**Bash shell**

You already have it!
Depending on which version of Linux you’re running you may need to type `bash` inside the terminal to access it.
To check whether this is necessary, follow these steps:

1. Open a terminal and type `echo $SHELL`.
   If it reads `/bin/bash` then you are all set!
   If not, whenever the instructions read "open a terminal," please assume you are to open a terminal, type `bash`, and the proceed with the instructions as specified.

**Git**

You may already have it; try typing `sudo apt-get install git` (Ubuntu, Debian) or `sudo yum install git` (Fedora) inside the terminal.
If you are prompted to install it follow the instructions on-screen to do so.

**VSCode**

1. Go to https://code.visualstudio.com/ and click the download button for either the .deb (Ubuntu, Debian) or the .rpm (Fedora, CentOS) file.
1. Double-click the downloaded file to install VSCode.
   (You may be prompted to type your administrator password during the install).

**VSCode extensions**

1. Open the Visual Studio Code application.
1. Press `Ctrl+Shift+P` in the new window that opens and type "Extensions: Install extensions" into the search bar that appears at the top of the screen.
   Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads "Extensions: Install extensions").
1. A new panel should appear on the left-hand side of the screen with a search bar.
   Search for each of the following extensions and press `Install` for the first entry that appears. (The author listed for all of these extensions should be "Microsoft".)
      - Python (n.b., you will need to reload VSCode after installing this)
      - Live Share (n.b., you may need to press "Ctrl/Cmd+Shift+P" and type "install extensions" again after installing this)

**Python**

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
        bash Miniconda3-latest-Linux-x86_64.sh


1. A license agreement will be displayed and the bottom of the terminal will read `--More--`.
   Press `Enter` or the space bar until you are prompted with "Do you accept the license terms? [yes|no]."
   Type `yes` and then press `Enter`
1. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`).
   Leave this default and press `Enter`.
1. When you are asked "You can undo this by running `conda init --reverse $SHELL`? [yes|no]" type `yes` and press `Enter`.
   Exit the terminal once the installation has finished.
1. Re-open a new terminal.
   Type `which python` into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
   - If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
     If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.
1. Type the following to remove the installation script that was downloaded:

        rm ./Miniconda3-latest-Linux-x86_64.sh

**Python packages**

Open a terminal and type the following commands:

        conda config --append channels conda-forge
        conda config --set channel_priority strict
        conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```

```{tab-item} MacOs
**Bash shell**

You already have it!
Depending on which version of Mac OS you’re running you may need to type `bash` inside the terminal to access it.
To check whether this is necessary, follow these steps:

1. Open a terminal and type `echo $SHELL`.
   If it reads `/bin/bash` then you are all set!

Note: If you are using Mac Catalina (10.15.X) then it is possible your default shell is NOT CORRECT.
To set the default to bash, type `chsh -s /bin/bash` in the terminal, enter your password when prompted, and then close + re-open the terminal.

**Git**

You may already have it!
Try opening a terminal and typing `git --version`.
If you do not see something like “git version X.XX.X” printed out, then follow these steps: 

1. Follow [this link](https://sourceforge.net/projects/git-osx-installer/files/git-2.23.0-intel-universal-mavericks.dmg/download?use_mirror=autoselect) to automatically download an installer.
1. Double click the downloaded file (`git-2.23.0-intel-universal-mavericks.dmg`) and then double click the `git-2.23.0-intel-universal-mavericks.pkg` icon inside the dmg that is opened.
1. Follow the on-screen instructions to install the package.

**VSCode**

1. Go to https://code.visualstudio.com/ and click the download button.
1. Unzip the downloaded file (e.g., `VSCode-darwin-stable.zip`) and moving the resulting `Visual Studio Code` file to your Applications directory.

**VSCode extensions**

1. Open the Visual Studio Code application
1. Type `Cmd+Shift+P` and then enter "Shell command: Install 'code' command in PATH" into the search bar that appears at the top of the screen.
   Select the highlighted entry.
   A notification box should appear in the bottom-right corner indicating that the command was installed successfully.
1. Type `Cmd+Shift+P` again and then enter "Extensions: Install extensions" into the search bar.
   Select the appropriate entry from the dropdown menu that appears (there should be four entries; simply select the one that reads "Extensions: Install extensions").
1. A new panel should appear on the left-hand side of the screen with a search bar.
   Search for each of the following extensions and press `Install` for the first entry that appears. (The author listed for all of these extensions should be "Microsoft".)
      - Python (n.b., you will need to reload VSCode after installing this)
      - Live Share (n.b., you may need to press "Ctrl/Cmd+Shift+P" and type "install extensions" again after installing this)

**Python**

1. Open a new terminal and type the following lines (separately) into the terminal, pressing `Enter` after each one:

        curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
        bash Miniconda3-latest-MacOSX-x86_64.sh


1. A license agreement will be displayed and the bottom of the terminal will read `--More--`.
   Press `Enter` or the space bar until you are prompted with "Do you accept the license terms? [yes|no]."
   Type `yes` and then press `Enter`
1. The installation script will inform you that it is going to install into a default directory (e.g., `/home/$USER/miniconda3`).
   Leave this default and press `Enter`.
1. When you are asked "You can undo this by running `conda init --reverse $SHELL`? [yes|no]" type `yes` and press `Enter`.
   Exit the terminal once the installation has finished.
1. Re-open a terminal.
   Type `which python` into the terminal and it should return a path (e.g., `/home/$USER/miniconda3/bin/python`).
   - If you do not see a path like this then please try typing `conda init`, closing your terminal, and repeating this step.
     If your issue is still not resolved skip the following step and contact an instructor on the #help-installation channel of the BHS Slack.
1. Type the following to remove the installation script that was downloaded:

        rm ./Miniconda3-latest-MacOSX-x86_64.sh


**Python packages**

Open a terminal and type the following commands:

        conda config --append channels conda-forge
        conda config --set channel_priority strict
        conda install -y flake8 ipython jupyter jupyterlab matplotlib nibabel nilearn numpy pandas scipy seaborn
```
````

**Note**: If the instructions aren't working and you have spent more than 15-20 minutes troubleshooting on your own, please reach out to the workshop instructor (herholz dot peer at gmail dot com) with the exact problems you're having. He will try and get back to you quickly to help resolve the situation.


### Modern web browser

Install `Firefox` or `Chrome`.
(`Safari` will also work.)
`Microsoft Edge` is not modern, despite what Microsoft might try and otherwise tell you.

## Checking your install

Now that you've installed everything it's time to check that everything works as expected!
Type the following into your terminal:

    bash <( curl -s https://raw.githubusercontent.com/PeerHerholz/workshop_IRTG2150/main/check_install.sh)

If you installed everything correctly you should see a message informing you as such.
If any problems were detected you should receive some brief instructions on what is wrong with potential suggestions on how to remedy it.
If you followed these instructions step-by-step and cannot resolve the issue please contact one of the course instructors for more help.

Yeah, you did! Great job!

![logo](https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158)\
<sub><sup><sub><sup>https://media1.tenor.com/images/d5ebabf248130ec3842ed3b8627fd4f2/tenor.gif?itemid=4770158</sup></sub></sup></sub>

## Getting the workshop content

Now that you have installed the required software (or not) to follow the workshop, it's time to gather the respective
materials. Please use the `tab` matching your setup.

````{tab-set}  
```{tab-item} Conda (Recommended)

<img src="https://upload.wikimedia.org/wikipedia/commons/e/ea/Conda_logo.svg" alt="conda logo" width="300"/>\
<sub><sup><sub><sup>https://upload.wikimedia.org/wikipedia/commons/e/ea/Conda_logo.svg</sup></sub></sup></sub>

By installing `Python` on your system (i.e. specifically `Conda`) and setting up the appropriate environment, you will be able to open all the `Jupyter Notebooks` and go through the whole content of the course locally. 

To get things up and running, please follow these steps:

1. Download the [`environment.yml`](https://raw.githubusercontent.com/peerherholz/workshop_IRTG2150/main/environment.yml) file (e.g. with right mouse click -> Save As). Make sure that the file ends with `.yml` and not `.txt`.
2. Open up a conda terminal (or any other terminal), and create a new conda environment with the following command: `conda env create -f /path/to/file/environment.yml` - For example ``conda env create -f ~/Downloads/environment.yml`
3. Download the notebooks in this repository via [this link](https://github.com/PeerHerholz/workshop_IRTG2150/archive/refs/heads/main.zip) and unzip them to your preferred location, e.g. `Desktop/workshop_IRTG2150`.
4. Download the three datasets [ds000114](https://drive.google.com/drive/folders/1mvHQ4n0HijuKO6Pzr15elBnRKPJdfxKr?usp=sharing), [ds000228](https://drive.google.com/drive/folders/131BjdPhXL7qm38s62aCrRcoYW1uxqlms?usp=sharing), [pybids_7t_trt](https://drive.google.com/drive/folders/1mvHQ4n0HijuKO6Pzr15elBnRKPJdfxKr?usp=sharing) and [pybids_synthetic](https://drive.google.com/drive/folders/1xY4HqW3LA5eBkw9mD8FLQePn0-AfANvO?usp=sharing) and put them into the workshop folder as well, e.g. at `Desktop/workshop_IRTG2150/ds000114` and `Desktop/workshop_IRTG2150/ds000228`.
5. Next, open up a `conda terminal` (or any other `terminal`), activate the `conda environment` with `conda activate workshop_IRTG2150` (or on older `conda environment` with `source activate workshop_IRTG2150` for `mac` and `linux` and `activate workshop_IRTG2150` for `windows`).
6. Almost done. We need to make the `conda environment` available within `jupyter`. To do so, run the following command: `python -m ipykernel install --user --name=workshop_IRTG2150`.
7. Finally, via the `terminal`, move to the folder where you've put all the unzipped content of this workshop, e.g. with the command `cd ~/Desktop/workshop_IRTG2150` and run the command `jupyter notebook`. This should open a new tab in your browser running `jupyter notebook` and you should be able to see all the content of this workshop. If it does not open automatically, you can copy the link you should see in the `terminal` and paste it into your browser.
```

```{tab-item} Mybinder

<img src="https://mybinder.org/static/logo.svg?v=fe52c40adc69454ba7536393f76ebd715e5fb75f5feafe16a27c47483eabf3311c14ed9fda905c49915d6dbf369ae68fb855a40dd05489a7b9542a9ee532e92b" alt="binder logo" width="300"/>\
<sub><sup><sub><sup>https://mybinder.org/static/logo.svg?v=fe52c40adc69454ba7536393f76ebd715e5fb75f5feafe16a27c47483eabf3311c14ed9fda905c49915d6dbf369ae68fb855a40dd05489a7b9542a9ee532e92b</sup></sub></sup></sub>


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/PeerHerholz/workshop_IRTG2150/HEAD)

[MyBinder.org](https://mybinder.org/) is a great service that allows you to run Jupyter notebooks in a `Docker` or `Python` environment, directly online and for free. However, this service comes of course with a restricted computational environment (1-2GB of RAM). This means, many notebooks might be very slow and some might even crash, due to not enough memory.

You can use this approach to run and test most of the notebooks and to explore the slides. To access the MyBinder instance, use [this link](https://mybinder.org/v2/gh/peerherholz/mybinder_workshop_IRTG2150/HEAD).
```

```{tab-item} JupyterBook
<img src="https://jupyterbook.org/en/stable/_static/logo-wide.svg" alt="jupyter book logo" width="300"/>\
<sub><sup><sub><sup>https://jupyterbook.org/en/stable/_static/logo-wide.svg</sup></sub></sup></sub>


If you want to go through the content of this workshop without installing anything on your machine, you should chose this approach. To see all the notebooks and slides from this workshop, you can simply navigate through the sections of this website, ie `JupyterBook`.
```
````

## Enter the matrix

Once you reached this point, you should be ready the enter the matrix and follow the workshop in your preferred way. Congrats, fantastic work!

![logo](https://media1.tenor.com/images/e5c21d98f56c4af119b4e14b6a9df893/tenor.gif?itemid=4011236)\
<sub><sup><sub><sup>https://media1.tenor.com/images/e5c21d98f56c4af119b4e14b6a9df893/tenor.gif?itemid=4011236</sup></sub></sup></sub>

