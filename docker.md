# Installationsanleitung: Docker

![Docker Logo](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png)

[Docker](https://www.docker.com) ist eine [Open-Source-Software](https://de.wikipedia.org/wiki/Open_Source), mit der Anwendungen in einem [virtuellen Betriebssystem](https://de.wikipedia.org/wiki/Virtualisierung_(Informatik)) ausgeführt werden können. Dies vereinfacht die Bereitstellung der Anwendungen und beugt Probleme bei der Installation einzelner Komponenten vor.

## Navigation
1. [Installation unter Windows](#windows-vorbereitung)
2. [Installation unter OS X](#os-x-vorbereitung)
3. [Installation unter Linux Ubuntu](#linux-ubuntu-vorbereitung)

***

#### Windows: Vorbereitung
1. Um festzustellen, ob auf Ihrem Computer eine 32-Bit oder 64-Bit Version von Windows installiert ist, klicken Sie mit der rechten Maustaste unten links auf das **Windows-Symbol**
2. Klicken Sie auf **System**
3. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die Version eingesehen werden
4. Wenn eine 64-Bit Version installiert ist, klicken Sie [hier](https://download.docker.com/win/beta/InstallDocker.msi) um die Docker-Installationsdatei zu downloaden
5. Wenn **Windows 7**, **Windows 8** oder die **32-Bit Variante von Windows 10** installiert ist, klicken Sie [hier](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.exe) um die korrekte Docker-Installationsdatei zu downloaden

#### Windows: Installation
1. Öffnen Sie **InstallDocker.msi** bzw. **DockerToolbox-1.11.2.exe** mit einem Doppelklick
2. Folgen Sie den Anweisungen
3. Bevor Sie den Manager nach erfolgreicher Installation mit **Fertigstellen** beenden, vergewissern Sie sich, dass ein Häkchen bei **Docker ausführen** gesetzt ist

#### Windows: Docker starten
1. Wenn der Installationsmanager beendet wurde, startet Docker automatisch
2. Der **Wal in der Statusleiste** weist darauf hin, dass Docker funktionstüchtig ist und über den [Terminal](https://de.wikipedia.org/wiki/Terminal_(Computer)) bedient werden kann

#### Windows: Terminal öffnen
1. Öffnen Sie mit der Tastenkombination **Windowstaste + R** das Ausführen-Fenster
2. Tippen Sie **cmd.exe** ein und bestätigen mit Enter
3. Das Terminal, mit dem sich Docker bedienen lässt, öffnet sich
4. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker run hello-world` in das Terminal und bestätigen mit Enter
5. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

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
1. Klicken Sie oben rechts in der Statusleiste auf die Lupe und öffnen so **Spotlight-Suche**
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
