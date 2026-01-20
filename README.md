[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ZM7vCdJb)
# :mortar_board:Lab 1 Development Environment Setup (Mac & Windows)

**Course:** Software Defined Networking  
**Lab Type:** Setup /Prerequisite  
**Objective:** Prepare your development environment to complete all labs using VS Code, Docker, and Dev Containers. 

---

## :triangular_flag_on_post:Learning Goals

By the end of this lab, you will:

- Have Git, Docker, and Visual Studio Code installed
- Be able to launch a coding workspace using a Dev Container
- Understand the workflow using GitHub Classroom

---

## :computer:Step 1: Install Git

### :globe_with_meridians:Git for Windows

1. Download Git for Windows: [Git for Windows](https://git-scm.com/download/win)
2. Run the Standalone installer for x64 with default settings (make sure to select “Use Git from the command line and also from 3rd-party software”).
3. Open Command Prompt or PowerShell, and type:

```bash
git --version
```

### :apple:Git for Mac OS

1. Open **Terminal**
2. Run

```bash
git --version
```

If Git is not installed, macOS will prompt you to install the Command Line Developer Tools.  
3. Accept the Installation

---

## :whale:Step 2: Install Docker

You need Docker Desktop to run Dev Containers

### :globe_with_meridians:Docker Desktop for Windows

1. Donwload [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. During installation, enable WSL 2 and Install Ubuntu if prompted
3. Restart your machine
4. Open Docker and verify it's running (you should see a whale icon in the system tray.
5. Run in **Powershell:**

```Powershell
docker --version
```

### :apple:Docker Desktop for Mac OS

1. Donwload [Docker Desktop](https://www.docker.com/products/docker-desktop/)
2. Install and run it  
3. Check Docker is running from **Terminal:**

```bash
docker --version
```

## :cloud:Step 3: Install Visual Studio Code

Download and Install [Visual Studio Code](https://code.visualstudio.com/)

After installation, open the **Extensions** tab and install:  
Dev Containers by Microsoft  

---

## :clipboard:Step 4: Clone Your Assignment

1. Go to the GitHub Classroom link for this lab
2. Click "Accept" and then "Go to your assignment"
3. Copy the repository URL

### Open the repo in VS Code

```bash
git clone <repo-url>

cd <repo-folder>

code .
```

## :bookmark_tabs:Step 5: Open the Dev Container

Once the project is open in VS Code:

1. You’ll be prompted to **Reopen in Container** — click it.
    If not prompted:
    - Press `F1` (or `Cmd + Shift + P`)
    - Type: `Dev Containers: Reopen in Container`

VS Code will build the container and launch a development-ready Python environment.  

## :white_check_mark:Success Criteria

:white_check_mark:You can run the following inside the container terminal:

```bash
python3 --version

pip --version
```

:white_check_mark:You can edit files, install packages, and run scripts.  
:white_check_mark:You understand how to use GitHub Classroom, Git, Docker, and VS Code together  

## :heavy_check_mark:Test Your Setup

Run this in the terminal in VS Code which is the terminal of your Dev Container  

```bash
python3 -c "print('Hello from my Dev Container')" > hello_message.txt
```

## :warning:Troubleshooting Tips

- Docker won't start? Make sure virtualization is enabled in your BIOS (Windows)
- Dev Container failes to Build? Try reopening VS Code or Press `Ctrl + Shift + P` and enter the command

```bash
Dev Container: Rebuild Container
```

- Permissions Error on Mac: Try Restarting Docker and granting disk access under `System Settings > Privacy`

## :calendar:What to Submit

:white_check_mark:Push your repository to GitHub after confirming your setup by committing the file you created Testing your Setup  
