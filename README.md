<p align="center">
  <img src="https://i.imgur.com/CyxC7a4.jpg" alt="Logo"></img>
</p>

<p align="center">
  <img src="https://img.shields.io/github/license/QTechOfficial/OpenPeripherals" alt="License">
  <img src="https://img.shields.io/travis/QTechOfficial/OpenPeripherals/master" alt="Build Status">
  <img src="https://img.shields.io/github/release-date/QTechOfficial/OpenPeripherals" alt="Release">
  <br>
  <img src="https://img.shields.io/github/contributors/QTechOfficial/OpenPeripherals" alt="Contributors">
  <img src="https://img.shields.io/github/commit-activity/m/QTechOfficial/OpenPeripherals" alt="Commits per month">
  <img src="https://img.shields.io/github/last-commit/QTechOfficial/OpenPeripherals" alt="Last commit">
</p>

<h3 align="center">An open source program to control your peripherals written in Python.</h3>

<!-- 
Screenshots will go here!
-->

OpenPeripherals is an open source driver and frontend for controlling peripherals with special features that aims to replace and unify 3rd party software into a crossplatform, easy to use interface.

Currently OpenPeripherals only supports Linux, but Windows support is currently being worked on.

## Getting Started
### Linux:

Begin by cloning the repository using git.

`git clone https://github.com/QTechOfficial/OpenPeripherals.git`

If you happen to not have git you can install it by running:

| **Distro**    | **Command**            |
|---------------|------------------------|
| Debian/Ubuntu | `sudo apt install git` |
| Arch/Manjaro  | `sudo pacman -S git`   |

**Dependencies:**

You will need to run the following commands to download the dependencies:

| **Distro**    | **Command**                                          |
|---------------|------------------------------------------------------|
| Debian/Ubuntu | `sudo apt install python3 python3-pip libhidapi-dev` |
| Arch/Manjaro  | `sudo pacman -S python python-pip hidapi`            |

After those have installed, install the pip packages by running:

| **Distro**                 | **Command**                        |
|----------------------------|------------------------------------|
| Debian ≥ 9/Ubuntu ≥ 18.04  | `pip install -r requirements.txt`  |
| Debian < 9/Ubuntu < 18.04  | `pip3 install -r requirements.txt` |
| Latest Arch/Latest Manjaro | `pip install -r requirements.txt`  |

**Running:**
On first run do:

`sudo chmod 777 /dev/hidraw*`\
`python /OpenPeripherals/backend/daemon.py`\
`python /OpenPeripherals/ui/main.py`

After the first run do:

`python /OpenPeripherals/backend/daemon.py`\
`python /OpenPeripherals/ui/main.py`


***Note***
The method showed above will not be in the final version and in the final version it will either be ran by one .py file on linux or an executable (.exe) file on windows.

## Hardware Support
If your device is not on here, please submit a pull request!

**Supported devices:**
- Redragon
  * K556
  * K552

**WIP devices:**
- ASUS Aura (SMBus only)

**Currently unsupported devices:**
- ASUS Aura (USB)
