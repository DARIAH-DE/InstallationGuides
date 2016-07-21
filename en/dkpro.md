# Installation Guide: DARIAH-DKPro-Wrapper
![DKPro](https://www.ukp.tu-darmstadt.de/fileadmin/user_upload/Shared_Icons/DKPro.png)

[DARIAH-DKPro-Wrapper] (https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper) bundles the abilities of [several](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/blob/master/doc/tutorial.adoc#AvailableComponents) state-of-the-art [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing) tools. You have to use the wrapper with the command-line, but profound computer science knowledge is not necessary. The software is operating system independent and simply requires [Java Runtime Enivronment](https://en.wikipedia.org/wiki/Java_virtual_machine#Execution_environment) and an **internet connection**.

#### Prearrangement: Opening the command-line
- Windows: Keyboard shortcut **Windows key + R**
- OS X: Keyboard shortcut **cmd + Space bar**, type **terminal** and then press Enter
- Linux: Keyboard shortcut **Ctrl + Alt + T**

#### Installing Java
1. Download the appropriate installation file from the [Oracle website](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html)
2. Open the file and follow the instructions
3. Check Java Runtime Environment with the command `java -version` in the command prompt
3. If the following lines are displayed, everything works out just fine

~~~
java version "1.8.0_91"
Java(TM) SE Runtime Environment (build 1.8.0_91-b14)
Java HotSpot(TM) 64-Bit Server VM (build 25.91-b14, mixed mode)
~~~

**Note to Windows users**: To download the correct installation file, right-click the **Windows** icon, click **System**, and check the line **System Type**. You should use the 64-bit version of Java (at least **v1.8**) in order to be able to allocate ≥ 4 GB of RAM.

#### DARIAH-DKPro-Wrapper ready-to-use
1. Download [here](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/releases) the ZIP-archive of the current release, e.g. **ddw-0.4.6.zip**
2. Unpack the archive
3. Type ` cd /path/to/extracted/archive` into the terminal
4. Make sure that the actual [path](https://en.wikipedia.org/wiki/Path_(computing)) is set and press Enter

#### Using DARIAH-DKPro-Wrapper  (optional)
1. To test the DKPro-Wrapper, download a text example [here](https://wiki.de.dariah.eu/download/attachments/40213783/EffiBriestKurz.txt)
2. Type `java -Xmx4g -jar ddw-0.4.5.jar -language de -input /path/to/EffiBriestKurz.txt -output .` into the terminal, make sure the `-input` parameter leads to the actual file and press Enter
3. If the following lines are displayed, everything works out just fine

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

**Note**: A [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) file with annotated text of the `EffiBriestKurz.txt`-file has been created and placed in the previously unpacked archive.
