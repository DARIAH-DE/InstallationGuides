# Installationsanleitung: Docker

![Docker Logo](https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png)

Docker ist eine [Open-Source-Software](https://de.wikipedia.org/wiki/Open_Source), mit der Anwendungen in einem [virtuellen Betriebssystem](https://de.wikipedia.org/wiki/Virtualisierung_(Informatik)) ausgeführt werden können. Dies vereinfacht die Bereitstellung der Anwendungen und beugt Probleme bei der Installation einzelner Komponenten vor.

##Navigation
1. [Installation unter Windows](windows-vorbereitung)
2. Installation unter OS X
3. Installation unter Linux

### Windows: Vorbereitung
1. Um festzustellen, ob auf Ihrem Computer eine 32-Bit oder 64-Bit Version von Windows installiert ist, klicken Sie mit der rechten Maustaste unten rechts auf das **Windows Symbol**
2. Klicken Sie auf **System**
3. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die Version eingesehen werden
4. Wenn eine 64-Bit Version installiert ist, klicken Sie [hier](https://download.docker.com/win/beta/InstallDocker.msi) um die Docker-Installationsdatei zu downloaden
5. Wenn Windows 7, Windows 8 oder die 32-Bit Variante von Windows 10 installiert ist, klicken Sie [hier](https://github.com/docker/toolbox/releases/download/v1.11.2/DockerToolbox-1.11.2.exe) um die korrekte Docker-Installationsdatei zu downloaden

### Windows: Installation
1. Öffnen Sie **InstallDocker.msi** bzw. **DockerToolbox-1.11.2.exe** mit einem Doppelklick
2. Folgen Sie den Anweisungen und beenden Sie den Manager nach erfolgreicher Installation mit **Fertigstellen**
3. Vergewissern Sie sich, dass ein Häkchen bei **Docker ausführen** gesetzt ist

### Windows: Docker starten
1. Wenn der Installationsmanager beendet wurde, startet Docker automatisch
2. Der Wal in der Statusleiste weist darauf hin, dass Docker funktionstüchtig ist und über den [Terminal](https://de.wikipedia.org/wiki/Terminal_(Computer)) bedient werden kann

### Windows: Terminal öffnen
1. Öffnen Sie mit der Tastenkombination **Windowstaste + R** das Ausführen-Fenster
2. Geben Sie in das Fenster **cmd.exe** und bestätigen mit Enter
3. Der Terminal, mit dem sich Docker bedienen lässt, öffnet sich
4. Um zu überprüfen, ob Docker erfolgreich installiert wurde, tippen Sie `docker version` in das Terminal und bestätigen mit Enter
5. Wenn folgende Meldung angezeigt wird, wurde Docker erfolgreich installiert

~~~
Client:
Version:      1.12.0-rc2
API version:  1.24
Go version:   go1.6.2
Git commit:   906eacd
Built:        Fri Jun 17 20:35:33 2016
OS/Arch:      windows/amd64
Experimental: true

Server:
Version:      1.12.0-rc2
API version:  1.24
Go version:   go1.6.2
Git commit:   a7119de
Built:        Fri Jun 17 22:09:20 2016
OS/Arch:      linux/amd64
Experimental: true
~~~




***
