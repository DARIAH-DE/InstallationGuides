# Installationsanleitung: Docker

![Docker Logo](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png)

Docker ist eine [Open-Source-Software](https://de.wikipedia.org/wiki/Open_Source), mit der Anwendungen in einem [virtuellen Betriebssystem](https://de.wikipedia.org/wiki/Virtualisierung_(Informatik)) ausgeführt werden können. Dies vereinfacht die Bereitstellung der Anwendungen und beugt Probleme bei der Installation einzelner Komponenten vor.

## Navigation
1. [Installation unter Windows](#windows-vorbereitung)
2. [Installation unter OS X](#os-x-vorbereitung)
3. [Installation unter Linux](#linux-ubuntu-vorbereitung)

***

#### Windows: Vorbereitung
1. Um festzustellen, ob auf Ihrem Computer eine 32-Bit oder 64-Bit Version von Windows installiert ist, klicken Sie mit der rechten Maustaste unten rechts auf das **Windows Symbol**
2. Klicken Sie auf **System**
3. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die Version eingesehen werden
4. Wenn eine 64-Bit Version installiert ist, klicken Sie [hier](https://download.docker.com/win/beta/InstallDocker.msi) um die Docker-Installationsdatei zu downloaden
5. Wenn Windows 7, Windows 8 oder die 32-Bit Variante von Windows 10 installiert ist, klicken Sie [hier](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.exe) um die korrekte Docker-Installationsdatei zu downloaden

#### Windows: Installation
1. Öffnen Sie **InstallDocker.msi** bzw. **DockerToolbox-1.11.2.exe** mit einem Doppelklick
2. Folgen Sie den Anweisungen und beenden Sie den Manager nach erfolgreicher Installation mit **Fertigstellen**
3. Vergewissern Sie sich, dass ein Häkchen bei **Docker ausführen** gesetzt ist

#### Windows: Docker starten
1. Wenn der Installationsmanager beendet wurde, startet Docker automatisch
2. Der Wal in der Statusleiste weist darauf hin, dass Docker funktionstüchtig ist und über den [Terminal](https://de.wikipedia.org/wiki/Terminal_(Computer)) bedient werden kann

#### Windows: Terminal öffnen
1. Öffnen Sie mit der Tastenkombination **Windowstaste + R** das Ausführen-Fenster
2. Tippen Sie **cmd.exe** ein und bestätigen mit Enter
3. Der Terminal, mit dem sich Docker bedienen lässt, öffnet sich
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
3. Im nun geöffneten Fenster kann die Version des Betriebssystems eingesehen werden (z. B. 10.10.5)
4. Wenn mindestens Version 10.10 installiert ist, klicken Sie [hier](https://download.docker.com/mac/beta/Docker.dmg) um die Docker-Installationsdate zu downloaden
5. Wenn eine ältere Version als 10.10 installiert ist, klicken Sie [hier](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.pkg) um die korrekte Docker-Installationsdate zu downloaden

#### OS X: Installation
1. Öffnen Sie **Docker.dmg** bzw. **DockerToolbox-1.11.2.pk** mit einem Doppelklick
2. Folgen Sie den Anweisungen

#### OS X: Docker starten
1. Über das Launchpad kann Docker gestartet werden
2. Der Wal in der Statusleiste oben rechts weist darauf hin, dass Docker funktionstüchtig ist und über den [Terminal](https://de.wikipedia.org/wiki/Terminal_(Computer)) bedient werden kann

#### OS X: Terminal öffnen
1. Klicken Sie oben rechts in der Statusleiste auf die Lupe und öffnen so Spotlight-Suche
2. Tippen Sie **terminal** ein und bestätigen mit Enter
3. Der Terminal, mit dem sich Docker bedienen lässt, öffnet sich
4. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker run hello-world` in das Terminal und bestätigen mit Enter
5. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~

***

#### Linux Ubuntu: Vorbereitung
1. Öffnen Sie mit der Tastenkombination **Strg + Alt + T** das Terminal und überprüfen Sie mit `uname -r` die Kernel-Version. Um Docker problemlos nutzen zu können, muss mindestens **3.10** installiert sein
2. Aktualisieren Sie die Paket-Datenbank mit `sudo apt-get update`

#### Linux Ubuntu: Installation
1. Fügen Sie den GPG Schlüssel des offiziellen Docker Repositorys dem System hinzu
~~~
sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
~~~
2. Fügen Sie das Docker Repository APT hinzu
~~~
echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list
~~~
3. Aktualisieren Sie Die Paket-Datenbank mit `sudo apt-get update` erneut um die Docker Packages sehen zu können
4. Vergewissern Sie sich mit `apt-cache policy docker-engine`, dass Sie direkt vom Docker Repository installieren. Folgendes sollte angezeigt werden (die `docker-engine` Version könnte eine andere sein)
~~~
docker-engine:
  Installed: (none)
  Candidate: 1.11.1-0~xenial
  Version table:
     1.11.1-0~xenial 500
        500 https://apt.dockerproject.org/repo ubuntu-xenial/main amd64 Packages
     1.11.0-0~xenial 500
        500 https://apt.dockerproject.org/repo ubuntu-xenial/main amd64 Packages
~~~
5. Um Docker schließlich zu installieren, bestätigen Sie folgenden Befehl mit Enter
~~~
sudo apt-get install -y docker-engine
~~~
4. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker run hello-world` in das Terminal und bestätigen mit Enter
5. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

~~~
Hello from Docker.
This message shows that your installation appears to be working correctly.
...
~~~
