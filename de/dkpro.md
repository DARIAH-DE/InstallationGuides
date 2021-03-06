# Installationsanleitung: DARIAH-DKPro-Wrapper
![DKPro](https://www.ukp.tu-darmstadt.de/fileadmin/user_upload/Shared_Icons/DKPro.png)

Der [DARIAH-DKPro-Wrapper](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper) bündelt eine Reihe von [Annotationstechniken](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/blob/master/doc/tutorial.adoc#AvailableComponents) aus dem Bereich [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing), die mithilfe der [Kommandozeile](https://de.wikipedia.org/wiki/Kommandozeile) auch ohne tiefgreifende Informatikkenntnisse genutzt werden können. Die Software ist betriebssystemunabhängig und erfordert lediglich [Java Runtime Enivronment](https://de.wikipedia.org/wiki/Java-Laufzeitumgebung) und eine Internetverbindung.

#### Vorbereitung: Terminal öffnen
- Windows: Tastenkombination **Windowstaste + R**
- OS X: Tastenkombination **cmd + Leertaste**, **terminal** eintippen und mit Enter bestätigen
- Linux: Tastenkombination **Strg + Alt + T**

#### Java installieren
1. Downloaden Sie die entsprechende Installationsdatei von der [Oracle Website](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html)
2. Öffnen Sie die Datei und folgen den Anweisungen
3. Überprüfen Sie mit dem Befehl `java -version` über die Kommandozeile in welcher Version Java Runtime Environment vorliegt
3. Wird Ihnen folgendes angezeigt, war die Installation erfolgreich

~~~
java version "1.8.0_91"
Java(TM) SE Runtime Environment (build 1.8.0_91-b14)
Java HotSpot(TM) 64-Bit Server VM (build 25.91-b14, mixed mode)
~~~

**Hinweis Windows Nutzer**: Um die korrekte Installationsdatei (**32-Bit** oder **64-Bit**) zu downloaden, klicken Sie mit der rechten Maustaste unten links auf das **Windows-Symbol**, anschließend auf **System**. Im nun geöffneten Fenster kann in der Zeile **Systemtyp** die erforderliche Version eingesehen werden. Die 64-Bit Version wird empfohlen, um ≥ 4 GB RAM bereitstellen zu können.

#### DARIAH-DKPro-Wrapper einsatzbereit machen
1. Downloaden Sie [hier](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/releases) das ZIP-Archiv des aktuellen Release, z. B. **ddw-0.4.6.zip**
2. Entpacken Sie das Archiv
3. Tippen Sie `cd /pfad/zum/entpackten/archiv` in die Kommandozeile
4. Achten Sie darauf, dass der tatsächliche [Pfad](https://de.wikipedia.org/wiki/Pfadname) angegeben ist und bestätigen mit Enter

#### DARIAH-DKPro-Wrapper benutzen (optional)
1. Um den DKPro-Wrapper zu testen, downloaden Sie [hier](https://wiki.de.dariah.eu/download/attachments/40213783/EffiBriestKurz.txt) ein Textbeispiel
2. Tippen Sie `java -Xmx4g -jar ddw-0.4.5.jar -language de -input /pfad/zu/EffiBriestKurz.txt -output .` in die Kommandozeile und bestätigen nach Anpassung des Parameters (`/pfad/zu/EffiBriestKurz.txt`) mit Enter
3. Wenn nach etwa einer Minuten folgendes angezeigt wird, war die Installation erfolgreich

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

**Hinweis**: Eine CSV-Datei mit annotiertem Text der `EffiBriestKurz.txt`-Datei wurde in dem zuvor entpackten Archiv abgelegt.
