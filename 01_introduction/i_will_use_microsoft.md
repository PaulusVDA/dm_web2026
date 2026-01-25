# Windows Setup

Oh... I see you've decided to use Windows. Don't worry, nobody's perfect!

## Installing Conda on Windows

1. **Download Miniconda Installer**:
   - Visit the [Miniconda download page](https://docs.conda.io/en/latest/miniconda.html).
   - Select the `Miniconda3 Windows 64-bit` installer for Windows.

2. **Run the Installer**:
   - After downloading, double-click the installer executable (`Miniconda3-latest-Windows-x86_64.exe`) to run it.

3. **Follow On-Screen Instructions**:
   - Click 'Next' on the installer window.
   - Accept the license agreement by selecting 'I agree' and click 'Next'.
   - Choose the installation location or leave it as the default, then click 'Next'.
   - Select 'Just Me' as the installation type and click 'Next'.
   - Check the option to "Add Miniconda3 to my PATH environment variable" (optional but recommended).
   - The installation will begin and may take a few minutes.

4. **Open Command Prompt**:
   - Press `Win + S` and search for 'Anaconda Powershell' or 'Anaconda Prompt' to open a new terminal window.
   - Alternatively, you can use Windows PowerShell or Command Prompt if you added Miniconda to PATH.

5. **Verify Installation**:
   - Run the following command to verify that Conda is installed:
     ```bash
     conda --version
     ```

## Install Essential Libraries

For this class, we will use the `base` environment that comes with Conda. If you see `(base)` at the beginning of your terminal prompt, it worked!

Now, install some essential libraries:

```bash
pip install pandas
pip install matplotlib
pip install ipykernel
```

If all goes well, you're ready to start!

## Installing Visual Studio Code

1. **Download the Visual Studio Code Installer**:
   - Go to the [Visual Studio Code download page](https://code.visualstudio.com/download).
   - Choose the Windows installer.

2. **Run the Installer**:
   - After downloading, double-click the installer executable (`VSCodeSetup-x64.exe`) to run it.

3. **Follow On-Screen Instructions**:
   - Click 'Next' on the installer window.
   - Select the installation location or leave it as the default, then click 'Next'.
   - Choose whether you want to create desktop and Start menu shortcuts, then click 'Next'.
   - Click 'Install' to begin the installation.

4. **Open VSCode**:
   - After installation, open Visual Studio Code from the Start menu or by searching for "Visual Studio Code" in the taskbar.

## Setting up VSCode

1. **Create a project folder**: Create a folder for our first project and open it in VSCode (File -> Open Folder).

2. **Install extensions**: Click on the Extensions icon in the left sidebar (or press `Ctrl + Shift + X`) and install:
   - Python
   - Jupyter

3. **Select the Python interpreter**: Press `Ctrl + Shift + P`, type `select interpreter`, and choose the `base` environment.

4. **Test your setup**: Create a new file called `test.ipynb`. This is a Jupyter notebook. Click on a cell, type `print("Hello!")`, and press `Ctrl + Enter` to run it. If it asks you to select a kernel, choose `base`.

---

## Terminal Basics (PowerShell)

The terminal is a text-based way to interact with your computer. Here are the essential commands for PowerShell/Anaconda Prompt:

| Command | What it does | Example |
|---------|--------------|---------|
| `pwd` | Shows your current location | `pwd` |
| `ls` or `dir` | Lists files in current folder | `ls` |
| `cd` | Changes directory | `cd Documents` |
| `cd ..` | Goes up one folder | `cd ..` |
| `mkdir` | Creates a new folder | `mkdir my_project` |
| `copy` | Copies a file | `copy file.txt copy.txt` |
| `move` | Moves or renames a file | `move old.txt new.txt` |
| `del` | Deletes a file (careful!) | `del file.txt` |

**Tips:**
- Use `Tab` to autocomplete file names
- Use `↑` arrow to repeat previous commands
- PowerShell also supports most Linux commands (`ls`, `pwd`, `cp`, `mv`, `rm`)

---

## Git Basics

Git is a version control system - it tracks changes to your files and lets you collaborate with others.

### Installing Git on Windows

1. Download Git from [git-scm.com](https://git-scm.com/download/win)
2. Run the installer and follow the default options
3. Restart your terminal after installation

### First-time setup

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Essential commands

| Command | What it does |
|---------|--------------|
| `git clone <url>` | Downloads a repository |
| `git status` | Shows what changed |
| `git add <file>` | Stages a file for commit |
| `git add .` | Stages all changes |
| `git commit -m "message"` | Saves your changes with a description |
| `git push` | Uploads your commits to the server |
| `git pull` | Downloads updates from the server |

### Typical workflow

```bash
# 1. Check what changed
git status

# 2. Stage your changes
git add .

# 3. Commit with a message
git commit -m "Added new feature"

# 4. Push to the server
git push
```

---

Congratulations! You're all set!
