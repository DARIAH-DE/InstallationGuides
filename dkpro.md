# Installationsanleitung: DARIAH-DKPro-Wrapper
<img src="https://www.ukp.tu-darmstadt.de/fileadmin/user_upload/Shared_Icons/DKPro.png" width="150" height="150">

Der DARIAH-DKPro-Wrapper bündelt eine Reihe von Annotationstechniken aus dem Bereich Natural Language Processing (NLP), die über die Kommandozeile ohne tiefgreifende Computerkenntnisse genutzt werden können, Ausgabe des Wrappers ist eine Datei im CSV-Format. Die Software ist betriebssystemunabhängig und erfordert lediglich Java Runtime Enivronment.

#### Vorbereitung: Terminal öffnen
- Windows: Tastenkombination **Windowstaste + R**
- OS X: Tastenkombination **cmd + Leertaste**, **terminal** eintippen und mit Enter bestätigen
- Linux: Tastenkombination **Strg + Alt + T**

#### Java installieren
1. Überprüfen Sie mit dem Befehl `java -version` ob und in welcher Version Java SE Runtime Environment installiert ist
2. Wird `command not found` angezeigt, downloaden Sie die entsprechende Installationsdatei von [Oracle Website](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html)
3. Folgen Sie den Anweisungen des Installationsmanagers

**Hinweis Windows Nutzer**: Um festzustellen, ob auf Ihrem Computer eine **32-Bit** oder **64-Bit** Version von Windows installiert ist, klicken Sie mit der rechten Maustaste unten links auf das **Windows-Symbol**, klicken Sie auf **System**. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die Version eingesehen werden.

#### DARIAH-DKPro-Wrapper einsatzbereit machen
1. Downloaden Sie [hier](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/releases) das ZIP-Archiv des aktuellen Release, z. B. **ddw-0.4.5.zip**
2. Entpacken Sie das Archiv an einen Ort Ihrer Wahl
3. Tippen Sie `cd /pfad/zum/dkpro/wrapper` in das Terminal und bestätigen mit Enter

#### DARIAH-DKPro-Wrapper benutzen
1. Um den DKPro-Wrapper nun zu testen, downloaden Sie sich [hier](https://wiki.de.dariah.eu/download/attachments/40213783/EffiBriestKurz.txt) ein Textbeispiel
2. Tippen Sie `java -Xmx4g -jar ddw-0.4.5.jar -language de -input /pfad/zu/EffiBriestKurz.txt -output .` in das Terminal und bestätigen nach Anpassung der Parameter mit Enter

**Hinweis**: Ersetzen Sie `/pfad/zu/EffiBriestKurz.txt` mit dem tatsächlichen Pfad zur Textdatei.
