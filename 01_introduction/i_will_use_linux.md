# Linux Setup

Oh! Nice, I see you've decided to use Linux. Excellent choice!

For this class, I recommend the use of Linux, preferably Debian-based systems like Ubuntu. Why? Because this is the system I am most familiar with, so I can effectively assist you with any problems.

## Installing Conda on Linux

1. **Download Miniconda Installer**:

   **Option A - Using wget (easiest method, recommended for CREMI machines):**

   On CREMI machines and Linux in general, the easiest way to download Miniconda is directly from the terminal using `wget`:
   ```bash
   wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
   ```
   This will download the installer to your current directory. Then skip to step 5 to run the installer.

   **Option B - Using a browser:**
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

6. **Open VSCode**:
   - After installation, open VSCode from the "Show Applications" menu or by typing `code` in the terminal.

## Setting up VSCode

1. **Create a project folder**: Create a folder for our first project and open it in VSCode (File -> Open Folder).

2. **Install extensions**: Click on the Extensions icon in the left sidebar (or press `Ctrl + Shift + X`) and install:
   - Python
   - Jupyter

3. **Select the Python interpreter**: Press `Ctrl + Shift + P`, type `select interpreter`, and choose the `base` environment.

4. **Test your setup**: Create a new file called `test.ipynb`. This is a Jupyter notebook. Click on a cell, type `print("Hello!")`, and press `Ctrl + Enter` to run it. If it asks you to select a kernel, choose `base`.

Congratulations! You're all set!
