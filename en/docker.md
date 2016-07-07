# Installation Guide: Docker

![Docker Logo](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png)

[Docker](https://www.docker.com) is an [Open-Source-Software](https://de.wikipedia.org/wiki/Open_Source), that wraps up applications in a [software container](https://en.wikipedia.org/wiki/Operating-system-level_virtualization). This simplifies the deployment of applications and prevents problems with the installation of individual components.

## Navigation
1. [Installation on Windows](#windows-vorbereitung)
2. [Installation on OS X](#os-x-vorbereitung)
3. [Installation on Linux Ubuntu](#linux-ubuntu-vorbereitung)

***

#### Windows: Prearrangement
1. To determine whether a 32-bit or 64-bit version of Windows is installed, click with the right mouse button on the **Windows icon**
2. Click **System**
3. Check the line **System Type**
4. In case you have a 64-bit version of Windows 10, click [here](https://download.docker.com/win/beta/InstallDocker.msi) to download the installation file
5. Otherwise (using **Windows 7**, **Windows 8** or **32-bit version of Windows 10**) click [here](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.exe) to download the correct installation file

#### Windows: Installation
1. Open **InstallDocker.msi** as the case may be **DockerToolbox-1.11.2.exe** with a double-click
2. Follow the instructions
3. Before closing the installation manager, make sure **Execute Docker** is selected

#### Windows: Starting Docker
1. After closing the installation manager, Docker is starting automatically
2. The **whale in the statusbar** points out that Docker is working well and can be used through the terminal

#### Windows: Open the terminal
1. Open the Run-window using the key combination **Windows key + R**
2. Type **cmd.exe** and press Enter, the terminal opens
3. Type `docker run hello-world` into the terminal and press Enter
5. If the following lines will be displayed, everything works out just fine

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~

***

#### OS X: Vorbereitung
1. Um festzustellen, welche Version von OS X auf Ihrem Mac installiert ist, klicken oben links auf das **Apple-Symbol**
2. Klicken Sie auf **Über diesen Mac**
3. Im nun geöffneten Fenster kann die Version des Betriebssystems eingesehen werden
4. Wenn OS X 10.10 oder höher installiert ist, klicken Sie [hier](https://download.docker.com/mac/beta/Docker.dmg) um die Docker-Installationsdatei zu downloaden
5. Wenn eine ältere Version als 10.10 installiert ist, klicken Sie [hier](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.pkg) um die korrekte Docker-Installationsdatei zu downloaden

#### OS X: Installation
1. Öffnen Sie **Docker.dmg** bzw. **DockerToolbox-1.11.2.pkg** mit einem Doppelklick
2. Folgen Sie den Anweisungen

#### OS X: Docker starten
1. Über das **Launchpad** kann Docker durch Klicken des Docker-Symbols gestartet werden
2. Der **Wal in der Statusleiste** oben rechts weist darauf hin, dass Docker funktionstüchtig ist und über den [Terminal](https://de.wikipedia.org/wiki/Terminal_(Computer)) bedient werden kann

#### OS X: Terminal öffnen
1. Öffnen Sie mit der Tastenkombination **cmd + Leertaste** die **Spotlight-Suche**
2. Tippen Sie **terminal** ein und bestätigen mit Enter
3. Das Terminal, mit dem sich Docker bedienen lässt, öffnet sich
4. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker run hello-world` in das Terminal und bestätigen mit Enter
5. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~

***

#### Linux Ubuntu: Vorbereitung
1. Öffnen Sie mit der Tastenkombination **Strg + Alt + T** das Terminal und überprüfen Sie mit `uname -r` die Kernel-Version
2. Um Docker problemlos nutzen zu können, muss mindestens **3.10** installiert sein
3. Aktualisieren Sie die Package-Datenbank mit `sudo apt-get update`

#### Linux Ubuntu: Installation
1. Fügen Sie den [GPG Schlüssel](https://de.wikipedia.org/wiki/GNU_Privacy_Guard) des offiziellen Docker Repositorys mit `sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D` dem System hinzu

2. Um das Docker Repository ihrer Package-Datenbank hinzuzufügen, bestätigen Sie `echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list` im Terminal

**Hinweis**: Dieser Befehl ist für Ubuntu 16.04 LTS (Xenial Xerus) geschrieben. Verfügen Sie über eine ältere Version, ersetzen Sie `ubuntu-xenial main` mit `ubuntu-trusty main` für Ubuntu 14.04 LTS (Trusty Tahr) oder `ubuntu-wily main` für Ubuntu 15.10 (Wily Werewolf).

3. Aktualisieren Sie nun die Package-Datenbank mit `sudo apt-get update` erneut
4. Installieren Sie schließlich Docker mit `sudo apt-get install -y docker-engine`
5. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker run hello-world` in das Terminal und bestätigen mit Enter
6. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~
