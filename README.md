# ML-Agents Installation

This repo contains instructions for installing the ML-Agents toolkit.

## Prerequisites

* [Python (version 3.6.1 or higher)](https://www.python.org/doc/versions/)

## Installation

1. Make sure your branch is synced with the latest changes so that it atleast includes the commit with the message `Install com.unity.ml-agents Unity package`.
2. Open up a terminal in your capstone repository folder.
3. Change directory to the folder inside `capstone` called `Tower Defense`.
   ```sh
   cd "Tower Defense"
   ```
4. Create a Python virtual environment by entering this command line into the terminal. This should create a folder called `venv` inside `Tower Defense`. If starting the command with `python` doesn't work, try replacing it with `py` or `python3`.
   ```sh
   python -m venv venv
   ```
5. Activate the virtual environment by entering this command line into the terminal. The command prompt now should start with (venv) to indicate that the virtual environment is active.
   ```sh
   venv\Scripts\activate
   ```
6. Install the PyTorch package with this command.
   ```sh
   pip install torch~=1.7.1 -f https://download.pytorch.org/whl/torch_stable.html
   ```
7. Install the mlagents package with this command.
   ```sh
   python -m pip install mlagents==0.28.0
   ```
8. After the mlagents package is installed, you can run this command to check that everything has been installed correctly.
   ```sh
   mlagents-learn --help
   ```
