# GrAPiC 

http://licence-info.univ-lyon1.fr/grapic

[![Github All Releases](https://img.shields.io/github/downloads/ucacaxm/grapic/total.svg)]()


## Linux & VS Code Fix

This repository is a modified version of the original Grapic project.
It contains configuration fixes and documentation improvements for Linux users.


### Original Repository

https://github.com/ucacaxm/grapic
All original code belongs to the original author.


## Purpose

The original workspace was configured mainly for Windows.
This version fixes the configuration to make it work properly on Linux using Visual Studio Code.


### Fixes Made

* Fixed Linux compilation issues
* Updated Makefile
* Added Visual Studio Code configuration
* Fixed include paths
* Modified `.vscode/tasks.json` to work on Linux
* Added a keyboard shortcut to compile and run the program
* Added a tutorial in the README explaining how to configure the shortcut `Ctrl + Alt + G`


### Tested On

* Ubuntu Linux
* Visual Studio Code
* g++
## Prerequisites / Install

Before using this workspace on Linux, make sure you have the following tools and libraries installed:

```bash
sudo apt update
sudo apt install -y g++ doxygen zip lib-sdl2-dev libsdl2-image-dev libsdl2-ttf-dev
```

---

## How to Compile and Run

### Step 1 — Open the project in Visual Studio Code

Open the `grapic` folder using Visual Studio Code.

### Step 2 — Use the shortcut

Press:

Ctrl + Shift + B

This will:

* Compile Grapic

### Step 3 - How to Add the Keyboard Shortcut (Ctrl + Alt + G)

1. Open Keyboard Shortcuts:

   * Press `Ctrl + K` then `Ctrl + S`

2. Click the icon in the top-right: **Open Keyboard Shortcuts (JSON)** 

3. Add the following block:


```json
{
    "key": "ctrl+alt+g",
    "command": "workbench.action.tasks.runTask",
    "args": "Run Grapic"
}
```

**Important: do not remove the existing brackets `[ ]`. Just paste this block inside the array.**

4. Save the file

  * Press `Ctrl + S`

Now you can press:

`Ctrl + Alt + G`

to compile and run the program.
