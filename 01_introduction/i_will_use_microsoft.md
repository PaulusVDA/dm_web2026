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

Congratulations! You're all set!
