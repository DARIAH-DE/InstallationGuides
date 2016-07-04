# Installationsanleitung: DARIAH-DKPro-Wrapper
<img src="https://www.ukp.tu-darmstadt.de/fileadmin/user_upload/Shared_Icons/DKPro.png" width="150" height="150">

Der [DARIAH-DKPro-Wrapper](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper) bündelt eine Reihe von [Annotationstechniken](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/blob/master/doc/tutorial.adoc#AvailableComponents) aus dem Bereich [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing), die mithilfe der [Kommandozeile](https://de.wikipedia.org/wiki/Kommandozeile) auch ohne tiefgreifende Informatikenntnisse genutzt werden können. Die Software ist betriebssystemunabhängig und erfordert lediglich [Java Runtime Enivronment](https://de.wikipedia.org/wiki/Java-Laufzeitumgebung).

#### Vorbereitung: Terminal öffnen
- Windows: Tastenkombination **Windowstaste + R**
- OS X: Tastenkombination **cmd + Leertaste**, **terminal** eintippen und mit Enter bestätigen
- Linux: Tastenkombination **Strg + Alt + T**

#### Java installieren
1. Überprüfen Sie mit dem Befehl `java -version` über das Terminal ob und in welcher Version Java Runtime Environment installiert ist (**mindestens 1.8**)
2. Wird `command not found` angezeigt, downloaden Sie die entsprechende Installationsdatei von der [Oracle Website](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html)
3. Folgen Sie den Anweisungen des Installationsmanagers

**Hinweis Windows Nutzer**: Um festzustellen, ob auf Ihrem Computer eine **32-Bit** oder **64-Bit** Version von Windows installiert ist, klicken Sie mit der rechten Maustaste unten links auf das **Windows-Symbol**, klicken Sie auf **System**. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die Version eingesehen werden.

#### DARIAH-DKPro-Wrapper einsatzbereit machen
1. Downloaden Sie [hier](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/releases) das ZIP-Archiv des aktuellen Release, z. B. **ddw-0.4.5.zip**
2. Entpacken Sie das Archiv
3. Tippen Sie `cd /pfad/zum/entpackten/archiv` in das Terminal
4. Achten Sie darauf, dass der tatsächliche [Pfad](https://de.wikipedia.org/wiki/Pfadname) angegeben ist und bestätigen mit Enter

#### DARIAH-DKPro-Wrapper benutzen
1. Um den DKPro-Wrapper nun zu testen, downloaden Sie [hier](https://wiki.de.dariah.eu/download/attachments/40213783/EffiBriestKurz.txt) ein Textbeispiel
2. Tippen Sie `java -Xmx4g -jar ddw-0.4.5.jar -language de -input /pfad/zu/EffiBriestKurz.txt -output .` in das Terminal und bestätigen nach Anpassung der Parameter (`/pfad/zu/EffiBriestKurz.txt` mit dem tatsächlichen Pfad zur Textdatei ersetzen) mit Enter
3. Wenn nach etwa einer Minuten folgendes angezeigt wird, funktioniert der DARIAH-DKPro-Wrapper tadellos

~~~
INFO: Dependency Parsing: writeConstituency, false
INFO: Constituency Parsing: writeDependency, false
INFO: Coreference Resolver: postprocessing, false
INFO: Process 1 files
INFO: Start running the pipeline (this may take a while)...
INFO: Process file: EffiBriestKurz.txt
INFO: 16.27.677  is2.data.ParametersFloat 121:read ->        read parameters 134217727 not zero 1542768
INFO: 16.27.681  is2.data.Cluster 113:<init> ->              Read cluster with 0 words 
INFO: 16.27.683  is2.tag.Lexicon 103:<init> ->               Read lexicon with 0 words 
INFO: 16.27.683  is2.tag.Tagger 138:readModel ->             Loading data finished. 
INFO: 16.34.593  is2.data.ParametersFloat 121:read ->        read parameters 134217727 not zero 1012032
INFO: 16.34.608  is2.data.Cluster 113:<init> ->              Read cluster with 0 words 
INFO: 16.34.609  is2.lemmatizer.Lemmatizer 192:readModel ->  Loading data finished. 
INFO: 16.34.610  is2.lemmatizer.Lemmatizer 194:readModel ->  number of params  134217727
INFO: 16.34.610  is2.lemmatizer.Lemmatizer 195:readModel ->  number of classes 371
INFO: 16.41.759  is2.data.ParametersFloat 121:read ->        read parameters 134217727 not zero 4044229
INFO: 16.41.768  is2.data.Cluster 113:<init> ->              Read cluster with 0 words 
INFO: 16.41.770  is2.mtag.Tagger 148:readModel ->            Loading data finished. 
INFO: 16.41.770  is2.mtag.Tagger 150:readModel ->            number of parameter 134217727
INFO: 16.41.771  is2.mtag.Tagger 151:readModel ->            number of classes   268
INFO: ---- DONE -----
INFO: All files processed in 0,84 minutes
~~~

**Hinweis**: Eine CSV-Datei mit annotiertem Text wurde erstellt und in dem zuvor entpackten Archiv abgelegt.
