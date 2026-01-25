# Setting up the Environment

For this class, I recommend using Conda combined with Visual Studio Code (yes, it's from Microsoft!). I believe this to be the easiest and fastest setup across all platforms.

## Linux

For this class, I recommend the use of Linux, preferably Debian-based systems like Ubuntu. Why? Because this is the system I am most familiar with, so I can effectively assist you with any problems. However, if you prefer Windows or macOS, that's fine too! I will still help, but resolving issues might take longer as we'll need to search for solutions online.

### Installing Conda on Linux

1. **Download Miniconda Installer**:
   - Visit the [Miniconda download page](https://docs.conda.io/en/latest/miniconda.html).
   - Select the `Miniconda3 Linux 64-bit` installer for Linux.

2. **Open Terminal**:
   - Open your terminal after downloading.

3. **Navigate to the Download Directory**:
   - Use the `cd` command to go to the directory where Miniconda was downloaded, usually the `Downloads` folder:
     ```bash
     cd ~/Downloads
     ```

4. **Check if the .sh file is in the folder**:
   ```bash
   ls 

   # Expected file:
   Miniconda3-latest-Linux-x86_64.sh
   ```

5. **Run the Installer**:
   - Execute the installer script:
     ```bash
     bash Miniconda3-latest-Linux-x86_64.sh
     ```

6. **Follow On-Screen Instructions**:
   - Accept the license agreement by pressing `Enter` continuously. (Note: you need to go through the entire license agreement, so just hold down `Enter`. I know, it's tedious.)
   - Type `yes` to proceed with the installation.
   - Press `Enter` to accept the default installation location.
   - The installation might take a few minutes.

7. **Initialize Conda**:
   - At the end, the installer will ask if you wish to initialize Miniconda. Type `yes`.
   - This adds Conda to your PATH and enables Conda commands from the terminal.

8. **Close and Reopen Terminal**:
   - Close the terminal and reopen it for changes to take effect.

9. **Verify Installation**:
   - Run `conda list` to confirm a successful installation.

### Create an Environment

Once installed, create a Conda environment:

```bash
conda create --name dm_web python=3.11
``` 
This creates an environment named `dm_web` with Python 3.11 as the default.

Activate the environment:

```bash
conda activate dm_web
```

Now, install some essential libraries:

```bash
pip install pandas
pip install matplotlib
```

If all goes well, you're ready to start!

### Installing Visual Studio Code

1. **Download the Visual Studio Installer**:
   - Go to the [Visual Studio Code download page](https://code.visualstudio.com/download).
   - Choose the Linux installer (the one with the penguin). For Debian systems, select the .deb installer.

2. **Open Terminal**:
   - Open your terminal after downloading.

3. **Navigate to the Download Directory**:
   - Use `cd` to go to the directory where the installer was downloaded, usually the `Downloads` folder:
     ```bash
     cd ~/Downloads
     ```

4. **Check if the .deb file is in the folder**:
   ```bash
   ls 

   # Expected file:
   code_1.85.2-1705561292_amd64.deb
   ```

5. **Run the Installer**:
   - Execute the installer script. *Note: Superuser privileges are required to install VSCode.*:
     ```bash
     sudo dpkg -i code_1.85.2-1705561292_amd64.deb 
     ```

6. **Initialize VSCode**:
   - After installation, open VSCode from the "Show Applications" menu or using the `code` command in the terminal.

## Windows

### Installing Conda on Windows

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

### Create an Environment

Once installed, create a Conda environment:

```bash
conda create --name dm_web python=3.11
``` 
This creates an environment named `dm_web` with Python 3.11 as the default.

Activate the environment:

```bash
conda activate dm_web
```

Now, install some essential libraries:

```bash
pip install pandas
pip install matplotlib
```

If all goes well, you're ready to start!

### Installing Visual Studio Code

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

4. **Initialize Visual Studio Code**:
   - After installation, you can open Visual Studio Code from the Start menu or by searching for 'Visual Studio Code' in the taskbar search.

You have now successfully installed Conda and Visual Studio Code on Windows.

## macOS (Apple)

### Installing Conda on macOS

1. **Download Miniconda Installer**:
   - Visit the [Miniconda download page](https://docs.conda.io/en/latest/miniconda.html).
   - Select the appropriate installer for your Mac:
     - For Apple Silicon (M1, M2, M3, M4): Choose `Miniconda3 macOS Apple M1 64-bit pkg` or the bash installer.
     - For Intel Macs: Choose `Miniconda3 macOS Intel x86 64-bit pkg` or the bash installer.

2. **Run the Installer**:

   **Option A - Using the .pkg installer (recommended for beginners):**
   - Double-click the downloaded `.pkg` file.
   - Follow the on-screen instructions, accepting the license agreement.
   - The installer will place Miniconda in your home directory.

   **Option B - Using the .sh installer (terminal):**
   - Open Terminal (press `Cmd + Space`, type "Terminal", and press Enter).
   - Navigate to your Downloads folder:
     ```bash
     cd ~/Downloads
     ```
   - Run the installer:
     ```bash
     # For Apple Silicon:
     bash Miniconda3-latest-MacOSX-arm64.sh

     # For Intel Macs:
     bash Miniconda3-latest-MacOSX-x86_64.sh
     ```
   - Follow on-screen instructions and type `yes` when prompted.

3. **Initialize Conda**:
   - If prompted, type `yes` to initialize Miniconda.
   - Close and reopen Terminal for changes to take effect.

4. **Verify Installation**:
   - Open a new Terminal window and run:
     ```bash
     conda --version
     ```

### Create an Environment

Once installed, create a Conda environment:

```bash
conda create --name dm_web python=3.11
```
This creates an environment named `dm_web` with Python 3.11 as the default.

Activate the environment:

```bash
conda activate dm_web
```

Now, install some essential libraries:

```bash
pip install pandas
pip install matplotlib
```

If all goes well, you're ready to start!

### Installing Visual Studio Code

1. **Download Visual Studio Code**:
   - Go to the [Visual Studio Code download page](https://code.visualstudio.com/download).
   - Click on the macOS button (the Apple logo).
   - This will download a `.zip` file.

2. **Install VSCode**:
   - Open Finder and go to your Downloads folder.
   - Double-click the downloaded `.zip` file to extract it.
   - Drag `Visual Studio Code.app` to the `Applications` folder.

3. **Open VSCode**:
   - Open Finder, go to Applications, and double-click on Visual Studio Code.
   - Alternatively, press `Cmd + Space`, type "Visual Studio Code", and press Enter.

4. **Install the 'code' command in PATH** (optional but recommended):
   - Open VSCode.
   - Press `Cmd + Shift + P` to open the Command Palette.
   - Type "shell command" and select "Shell Command: Install 'code' command in PATH".
   - Now you can open VSCode from Terminal by typing `code`.

You have now successfully installed Conda and Visual Studio Code on macOS.


## Defining the Work Environment in VSCode

Now, let's prepare our VSCode setup. These steps apply to Linux, Windows, and macOS.

**Note for macOS users:** Replace `Ctrl` with `Cmd` for keyboard shortcuts (e.g., `Cmd + Shift + P` instead of `Ctrl + Shift + P`).

1. First, create a folder for our first project and open it in VSCode.

2. Next, set up our Conda environment in VSCode. Press `Ctrl + Shift + P`, type `select interpreter`, and choose the `dm_web` environment. To check if it's working, open a new terminal from "Terminal" -> "New Terminal". If it's working, you'll see the Conda environment name in the terminal. Try a simple "hello world" program to test.

3. VSCode offers helpful extensions. Install the following:
   - Python
   - Pylance
   - Jupyter

4. Test our Jupyter notebook setup by creating a `test.ipynb` file. Try executing a cell with a simple Python command (use `Ctrl + Enter`). VSCode will prompt you to select the Python interpreter again. Choose `dm_web`. You may be asked to install `Ipykernel`. After installation, you should be able to run Jupyter cells.


Congratulations! You now have a functional environment with VSCode, Jupyter, and the necessary tools!
