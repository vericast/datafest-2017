[![Gitter](https://badges.gitter.im/maxpoint/datafest-2017.svg)](https://gitter.im/maxpoint/datafest-2017?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

Materials for the 2017 *Data Analysis with Python* DataFest workshop at Duke University.

# Instructions for Participants

## Before you Attend the Workshop

Please try to complete the following setup instructions before the day of the
workshop. They take you through installing a [conda
environment](https://conda.io/docs/index.html) on your computer containing
common Python packages for data analysis as well as the [Jupyter
Notebook](https://jupyter.org) tool.

If you get stuck, don't worry. You can ask for help from the instructors and
other participants in our [Gitter chat
room](https://gitter.im/maxpoint/datafest-2017).  We'll also have some time at
the beginning of the session to help you. If you already have an environment
setup for data analysis with Python, don't worry. These instructions will not
touch your existing setup.

1. Grab your Windows 7+, Mac OS X 10.11+, or Linux laptop.
2. Visit [updatemybrowser.org](https://updatemybrowser.org) to make sure you
   have a modern web browser installed. If you don't, download and install
   either [Google Chrome](https://www.google.com/chrome/browser/desktop/) or
   [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/) for free.
3. Visit the [*Data Analysis with Python* releases
   page](https://github.com/maxpoint/datafest-2017/releases).
4. Click the link next to the latest *datafest* installer for your computer.
5. Save the installer to your typical downloads folder.
    * Windows: `C:\User\<your username>\Downloads`
    * Linux/OSX: `~/Downloads`

When the download completes, continue to the section for your operating system
below.

### Windows

1. Use Windows Explorer to open your Downloads folder.
2. Double-click the installer file you downloaded.
3. Step through the pages of the installer, using the default values
   except in two cases:
   1. Choose `C:\Users\<your username>\datafest` for the install location,
      substituting the appropriate drive letter if C is not your main drive.
   2. Uncheck both checkboxes on the *Advanced Options* page.
5. Click *Install*.
6. Click *Finish* when the installer completes.
7. Click the *Start* menu button in the task bar.
8. Type `cmd` in the search box and press *Enter*.
9. Enter the following commands, one per line, in the terminal window.

```bash
# switches to your home directory
cd
# activates the conda environment you installed
datafest\Scripts\activate.bat
# pulls the workshop materials from GitHub
git clone https://github.com/maxpoint/datafest-2017.git
# runs a Jupyter Notebook server for local use
jupyter notebook --notebook-dir .\datafest-2017\notebooks
```

If your web browser opens to a page with the Jupyter logo in the top right
corner, congratualations, you have everything you need. If not, ask
for help in our [Gitter chat room](https://gitter.im/maxpoint/datafest-2017).

After testing your setup, you can clean up by pressing *Ctrl-C* twice in the
command prompt window, closing that window, and closing any Jupyter Notebook
tabs in your web browser.

### Mac / Linux

1. Open a *Terminal* application.
2. Enter the following commands, one per line, in the terminal window.

```bash
# switches to the folder where you saved the installer
cd ~/Downloads
# runs the installer
bash datafest-*.sh -b -p ~/datafest

# switches to your home directory
cd ~
# activates the conda environment you installed
source datafest/bin/activate
# pulls the workshop materials from GitHub
git clone https://github.com/maxpoint/datafest-2017.git
# runs a Jupyter Notebook server for local use
jupyter notebook --notebook-dir ./datafest-2017/notebooks
```

If your web browser opens to a page with the Jupyter logo in the top right
corner, congratualations, you have everything you need. If not, ask
for help in our [Gitter chat room](https://gitter.im/maxpoint/datafest-2017).

After testing your setup, you can clean up by pressing *Ctrl-C* twice in the
terminal window, closing the terminal window, and closing any Jupyter Notebook
tabs in your web browser.

### During the Workshop

The instructors will guide you through staring and using Jupyter Notebook to
analyze sample datasets on the day of the workshop. You can start the notebook
server before the session begins by opening a command prompt and
running the following commands.

### Windows

```bash
# switches to your home directory
cd
# activates the conda environment you installed
datafest\Scripts\activate
# runs a Jupyter Notebook server for local use
jupyter notebook --notebooks-dir .\datafest-2017\notebooks
```

### Mac / Linux

```bash
# switches to your home directory
cd ~
# activates the conda environment you installed
source datafest/bin/activate
# runs a Jupyter Notebook server for local use
jupyter notebook --notebooks-dir ./datafest-2017/notebooks
```

### During DataFest

You can reuse the tools from the workshop during DataFest. Simply run the
commands from the previous section to start Jupyter Notebook and have at it!

## Instructions for Admins

To build the installers:

```bash
# on a Windows box
constructor . --platform win-32
constructor . --platform win-64

# on an OSX box
constructor . --platform osx-64
constructor . --platform linux-32
constructor . --platform linux-64
```
