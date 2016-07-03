# Installationsanleitung: Python für Topic Modeling
![Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)

[Python](https://www.python.org) ist eine universelle und [interpretierte](https://de.wikipedia.org/wiki/Interpreter) Programmiersprache, die über eine klare und übersichtliche Syntax verfügt sowie eine umfangreiche Standardbibliothek und zahlreiche Pakete im [PyPI](https://pypi.python.org/pypi) besitzt. Ihre Entwurfsphilosophie betont Programmlesbarkeit, außerdem ist Python-Code im Vergleich mit anderssprachigem Code teilweise deutlich kürzer.

## Navigation
1. Installation unter Windows
2. Installation unter OS X
3. Installation unter Linux

***

#### Windows: Python 3 installieren
1. Klicken Sie [hier](https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe) um die Installationsdatei zu downloaden 2. Öffnen Sie die Datei `python-3.5.2.exe` und folgen Sie den Anweisungen
3. Achten Sie darauf, dass ein Häkchen bei *Add Python to PATH* gesetzt ist  

#### Windows: Pakete installieren
1. Öffnen Sie mit der Tastenkombination **Windowstaste + R** das Terminal und aktualisieren Sie das Setuptool **pip** mit dem Befehl `pip3 install --upgrade pip`
3. Mit `pip3 install numpy matplotlib gensim` installieren Sie nun alle für Topic Modeling relevanten Pakete

***

#### OS X: Python 3 installieren
* Python (mindestens v3.5.1) auf der [Website](https://www.python.org/downloads/) downloaden und installieren
* Sicher gehen, dass bei **Install or upgrade pip** ein  Häkchen gesetzt ist
* Spotlight öffnen, "terminal" eintippen und bestätigen
* Über die nun geöffnete Kommandozeile alle erforderlichen Libraries installieren:
*       pip3 install numpy matplotlib gensim

##### Linux Ubuntu
**Hinweis:** Ubuntu 16.04 wird standardmäßig mit Python 3 ausgeliefert, deswegen entfällt hier der erste Befehl.
* Terminal öffnen, folgende Befehle eintippen und jeweils mit Enter bestätigen:
*       sudo apt-get install python3
*       sudo apt-get install python3-pip
*       sudo pip3 install numpy matplotlib gensim
