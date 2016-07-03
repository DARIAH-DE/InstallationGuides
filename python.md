# Installationsanleitung: Python für Topic Modeling
![Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)

[Python](https://www.python.org) ist eine universelle und [interpretierte](https://de.wikipedia.org/wiki/Interpreter) Programmiersprache, die über eine klare und übersichtliche Syntax verfügt sowie eine umfangreiche Standardbibliothek und zahlreiche Pakete im [PyPI](https://pypi.python.org/pypi) besitzt. Ihre Entwurfsphilosophie betont Programmlesbarkeit, außerdem ist Python-Code im Vergleich mit anderssprachigem Code teilweise deutlich kürzer.

## Navigation
1. Installation unter Windows
2. Installation unter OS X
3. Installation unter Linux

***

#### Windows: Python 3 + Pakete installieren
1. Klicken Sie [hier](https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe) um die Installationsdatei zu downloaden 2. Öffnen Sie die Datei `python-3.5.2.exe` und folgen Sie den Anweisungen
3. Achten Sie darauf, dass ein Häkchen bei **Add Python to PATH** gesetzt ist  
4. Öffnen Sie mit der Tastenkombination **Windowstaste + R** das Terminal und aktualisieren Sie das Setuptool **pip** mit dem Befehl `pip3 install --upgrade pip`
5. Mit `pip3 install numpy matplotlib gensim` installieren Sie nun alle für Topic Modeling relevanten Pakete

***

#### OS X: Python 3 + Pakete installieren
1. Klicken Sie [hier](https://www.python.org/ftp/python/3.5.2/python-3.5.2-macosx10.6.pkg) um die Installationsdatei zu downloaden
2. Öffnen Sie die Datei `python-3.5.2-macosx10.6.pkg` und folgen Sie den Anweisungen
3. Mit der Tastenkombination **cmd + Leertaste** die Spotlight-Suche öffnen, **terminal** eintippen und mit Enter bestätigen
4. Mit `pip3 install numpy matplotlib gensim` installieren Sie nun alle für Topic Modeling relevanten Pakete

#### Linux Ubuntu: Pakete installieren + opt. Python 3
**Hinweis:** Ubuntu 16.04 wird standardmäßig mit Python 3 ausgeliefert, deshalb kann 2. übersprungen werden.

1. Mit der Tastenkombination **Strg + Alt + T** das Terminal öffnen
2. Mit `sudo apt-get install python3` installieren Sie Python 3 über die Package-Datenbank
3. Mit `sudo apt-get install python3-pip`installieren Sie das Setuptool **pip**
4. Alle nötigen Pakete werden mit `sudo pip3 install numpy matplotlib gensim` installiert
