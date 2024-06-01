# MPT Updater and Installer

## Overview
The MPT Updater and Installer project consists of two main components:

- **Updater**: A script that checks for updates, downloads new versions if available, and runs an installer to apply the updates.
- **Installer**: A script that extracts the contents of a downloaded `.rar` file into the appropriate directory.

## Components

- **updater.py**: This Python script checks for updates, downloads new versions, and runs the installer. It is converted into an executable named `MPT.exe`.
- **Installer.exe**: This executable is created from the installer script and is responsible for extracting the contents of downloaded `.rar` files.
- **unrar.exe**: A required executable for extracting `.rar` files. - Is merged into Installer.exe

## Features

- **Automatic Update Checking**: The updater script checks for the latest version from a specified URL.
- **Download and Install Updates**: If a new version is found, it downloads the new files and runs the installer.
- **Error Handling**: Logs errors and provides feedback in the console.

## How It Works

1. **Check for Updates**: The updater script checks for the latest version from a specified URL.
2. **Download New Version**: If a new version is found, it downloads the new version to the `MPTDownloads` folder.
3. **Run Downloader**: Executes the downloaded updater executable to download the necessary `.rar` file.
4. **Run Installer**: Runs the installer executable to extract the contents of the `.rar` file to the appropriate directory.
5. **Update Version**: If the installation is successful, the local version file is updated.
