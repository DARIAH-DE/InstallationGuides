# Installationsanleitung: Python für Topic Modeling
![Python](https://upload.wikimedia.org/wikipedia/commons/f/f8/Python_logo_and_wordmark.svg)

[Python](https://www.python.org) ist eine universelle und [interpretierte](https://de.wikipedia.org/wiki/Interpreter) Programmiersprache, die über eine klare und übersichtliche Syntax verfügt sowie eine umfangreiche Standardbibliothek und zahlreiche Pakete im [PyPI](https://pypi.python.org/pypi) besitzt. Ihre Entwurfsphilosophie betont Programmlesbarkeit, außerdem ist Python-Code im Vergleich mit anderssprachigem Code teilweise deutlich kürzer.

## Navigation
1. Installation unter Windows
2. Installation unter OS X
3. Installation unter Linux

##### Windows
* Die neuste Python Version [von hier herunterladen](https://www.python.org/downloads/) und die *.exe* ausführen, dabei unbedingt einen **Haken bei *Add Python to PATH*** setzen  
* Die Eingabeaufforderung öffnen (Win10: *cmd* in die Searchbar eingeben, Win7: Windows-Taste + R und *cmd* eingeben) und das Setuptool *pip* aktualisieren:
*     python -m pip install --upgrade pip
*  Mit *pip* die fürs Topic Modeling notwendigen Libraries installieren:    
*     pip3 install numpy matplotlib gensim

##### Mac OS X
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
