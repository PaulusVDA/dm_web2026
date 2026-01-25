# macOS Setup

Oh... I see you've decided to use macOS. Don't worry, nobody's perfect!

## Installing Conda on macOS

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

4. **Install the 'code' command** (optional):
   - Open VSCode.
   - Press `Cmd + Shift + P`, type "shell command", and select "Shell Command: Install 'code' command in PATH".
   - Now you can open VSCode from Terminal by typing `code`.

## Setting up VSCode

1. **Create a project folder**: Create a folder for our first project and open it in VSCode (File -> Open Folder).

2. **Install extensions**: Click on the Extensions icon in the left sidebar (or press `Cmd + Shift + X`) and install:
   - Python
   - Jupyter

3. **Select the Python interpreter**: Press `Cmd + Shift + P`, type `select interpreter`, and choose the `base` environment.

4. **Test your setup**: Create a new file called `test.ipynb`. This is a Jupyter notebook. Click on a cell, type `print("Hello!")`, and press `Cmd + Enter` to run it. If it asks you to select a kernel, choose `base`.

Congratulations! You're all set!
