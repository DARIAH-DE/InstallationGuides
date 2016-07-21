# Installation Guide: Docker

![Docker Logo](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png)

[Docker](https://www.docker.com) is an [open-source software](https://en.wikipedia.org/wiki/Open-source_model) that wraps up software in a [container](https://en.wikipedia.org/wiki/Operating-system-level_virtualization). This simplifies the deployment of applications, saves time and prevents user issues and problems with the installation of individual components.

## Table of Contents
1. [Installation on Windows](#windows)
2. [Installation on OS X](#os-x)
3. [Installation on Linux Ubuntu](#linux-ubuntu)

***

## Windows
### Preparation
1. To determine whether a 32-bit or 64-bit version of Windows is installed on your machine, click on the **Windows icon** in the bottom left corner, then **System**
2. Check the line **System Type**
4. To download the 64-bit version, click [here](https://download.docker.com/win/beta/InstallDocker.msi)
5. Otherwise (using **Windows 7**, **Windows 8** or the **32-bit version of Windows 10**) click [here](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.exe) to download the correct installation file

### Installation and starting Docker
1. Open **InstallDocker.msi** resp. **DockerToolbox-1.11.2.exe** with a double-click and follow the instructions
2. After starting Docker, the **whale in the statusbar** points out that Docker is working well and is ready-to-use

### Using the command-line
1. Open the Run-window using the shortcut **Windows key + R**
2. Type **cmd.exe** and press Enter, the command prompt opens
3. Type `docker run hello-world` and press Enter
5. If the following lines are displayed, everything works out just fine

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~

***

## OS X
### Preparation
1. To determine which version of OS X is installed on your Mac, click the **Apple-symbol** in the top left corner, then **About this Mac**
2. If ≥ 10.10 installed, click [here](https://download.docker.com/mac/beta/Docker.dmg) to download the installation file
5. Otherwise, click [here](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.pkg) to download the correct installation file

### Installation
1. Open **Docker.dmg** resp. **DockerToolbox-1.11.2.pkg** with a double-click and follow the instructions

### Starting Docker
1. Click the Docker-symbol through [**Launchpad**](https://en.wikipedia.org/wiki/Launchpad_(OS_X))
2. The **whale in the statusbar** points out that Docker is working well and can be used through the terminal

### Using the command-line
1. Open [**Spotlight**](https://en.wikipedia.org/wiki/Spotlight_(software)) using the shortcut **cmd + spacebar**, then type **terminal** and press Enter
2. Type `docker run hello-world` into the command-line and press Enter
3. If the following lines are displayed, everything works out just fine

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~

***

## Linux Ubuntu
### Preparation
1. Open the terminal using the shortcut **Ctrl + Alt + T** to check the kernel version using `uname -r` (required: at least **3.10**)
3. Update the package database with `sudo apt-get update`

### Installation
1. Add the [GPG key](https://en.wikipedia.org/wiki/GNU_Privacy_Guard) of the official Docker repository to your system with `sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D`
2. To add the Docker repository to your package database, copy and paste `echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list` into the terminal before pressing Enter

**Hint**: This command is written for Ubuntu 16.04 LTS (Xenial Xerus). Otherwise replace `ubuntu-xenial main` with `ubuntu-trusty main` for Ubuntu 14.04 LTS (Trusty Tahr) or `ubuntu-wily main` for Ubuntu 15.10 (Wily Werewolf).

3. Update your package database with `sudo apt-get update`
4. Finally, install Docker with `sudo apt-get install -y docker-engine`
3. Type `docker run hello-world` into the terminal and press Enter
5. If the following lines are displayed, everything works out just fine

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~
