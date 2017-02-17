### Python Installationsguide für DariahTopics
##### Windows
**1. Einfach**  
Um nur mit einer Installation Python und wichtige Pakete auf den Rechner zu laden empfiehlt sich das vorgefertigte Bundle **WinPython**, welches [hier](https://sourceforge.net/projects/winpython/files/) als Download verfügbar ist (*latest version*).

**2. Fortgeschritten**  
Anders als mit WinPython können Python und die notwendigen Pakete auch einzeln heruntergeladen werden. Der Vorteil hierbei liegt darin, dass man alle weiteren Features die WinPython mit sich bringt, aber nicht braucht, nicht auch noch auf dem Rechner speichern muss.
* Die neuste Python Version [von hier herunterladen](https://www.python.org/downloads/) und die *.exe* ausführen, dabei unbedingt einen Haken bei *Add Python to PATH* setzen  
* Die Eingabeaufforderung öffnen (*cmd* in die Searchbar eingeben) und das Setuptool *pip* aktualisieren
*     python -m pip install --upgrade pip
*  Mit *pip* die fürs Topic Modeling notwendige Pakete installieren (*numpy*, *gensim*, *pandas*)  
*     pip3 install numpy matplotlib gensim

##### Mac OS X
* Python (mindestens v3.5.1) auf der [Website](https://www.python.org/downloads/) downloaden und installieren
* Sicher gehen, dass bei **Install or upgrade pip** ein  Häkchen gesetzt ist
* Spotlight öffnen, "terminal" eintippen und bestätigen
* Über die nun geöffnete Kommandozeile alle erforderlichen Libraries installieren:
  * pip3 install -r "path/to/requirements.txt" oder:
  * pip3 install numpy matplotlib gensim regex scipy pandas werkzeug flask pyLDAvis wikipedia lxml

##### Linux Ubuntu
**Hinweis:** Ubuntu 16.04 wird standardmäßig mit Python 3 ausgeliefert, deswegen entfällt hier der erste Befehl
* Terminal öffnen, folgende Befehle eintippen und jeweils mit Enter bestätign:
  * `sudo apt-get install python3`
  * `sudo apt-get install python3-pip`
  * `sudo pip3 install numpy matplotlib gensim`
