# Installationsanleitung: Python für Topic Modeling
![Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)

[Python](https://www.python.org) ist eine universelle und [interpretierte](https://de.wikipedia.org/wiki/Interpreter) Programmiersprache, die über eine klare und übersichtliche Syntax sowie eine umfangreiche Standardbibliothek und zahlreiche Pakete im [PyPI](https://pypi.python.org/pypi) verfügt. Ihre Entwurfsphilosophie betont Programmlesbarkeit, außerdem ist Python-Code im Vergleich mit anderssprachigem Code teilweise deutlich kürzer.

Mithilfe dieser Anleitung können Sie Python 3 sowie die Pakete [numpy](http://www.numpy.org), [matplotlib](http://matplotlib.org) und [gensim](https://radimrehurek.com/gensim/) installieren.

## Navigation
1. [Installation unter Windows](#windows-python-und-pakete-installieren)
2. [Installation unter OS X](#os-x-python-und-pakete-installieren)
3. [Installation unter Linux](#linux-ubuntu-python-und-pakete-installieren)

***

#### Windows: Python und Pakete installieren
1. Klicken Sie [hier](https://www.python.org/ftp/python/3.5.2/python-3.5.2-amd64.exe) um die Installationsdatei zu downloaden
2. Öffnen Sie die Datei `python-3.5.2.exe` und folgen den Anweisungen
3. Achten Sie darauf, dass ein Häkchen bei **Add Python to PATH** gesetzt ist  
4. Öffnen Sie mit der Tastenkombination **Windowstaste + R** die Kommandozeile und aktualisieren Sie das Setuptool **pip** mit dem Befehl `pip3 install --upgrade pip`
5. Mit `pip3 install numpy matplotlib gensim` installieren Sie alle für Topic Modeling relevanten Pakete

***

#### OS X: Python und Pakete installieren
1. Klicken Sie [hier](https://www.python.org/ftp/python/3.5.2/python-3.5.2-macosx10.6.pkg) um die Installationsdatei zu downloaden
2. Öffnen Sie die Datei `python-3.5.2-macosx10.6.pkg` und folgen den Anweisungen
3. Mit der Tastenkombination **cmd + Leertaste** öffnen Sie die Spotlight-Suche, tippen **terminal** ein und bestätigen mit Enter
4. Aktualisieren Sie das Setuptool **pip** mit dem Befehl `pip3 install --upgrade pip`
4. Mit `pip3 install numpy matplotlib gensim` installieren Sie alle für Topic Modeling relevanten Pakete

***

#### Linux Ubuntu: Python und Pakete installieren
**Hinweis:** Ubuntu 16.04 wird standardmäßig mit Python 3 ausgeliefert, deshalb kann 2. übersprungen werden.

1. Öffnen Sie mit der Tastenkombination **Strg + Alt + T** die Kommandozeile
2. Mit `sudo apt-get install python3` installieren Sie Python 3 und mit `sudo apt-get install python3-pip` das Setuptool **pip** (alternativ Upgrade mit `pip3 install --upgrade pip`)
4. Mit `sudo pip3 install numpy matplotlib gensim` installieren Sie alle für Topic Modeling relevanten Pakete
