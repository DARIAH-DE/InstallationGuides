# Installation Guide: DARIAH-DKPro-Wrapper
![DKPro](https://www.ukp.tu-darmstadt.de/fileadmin/user_upload/Shared_Icons/DKPro.png)

[DARIAH-DKPro-Wrapper] (https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper) bundles the abilities of [several](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/blob/master/doc/tutorial.adoc#AvailableComponents) state-of-the-art [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing) tools. You have to use the wrapper with the command prompt, but profound computer science knowledge is not necessary. The software is operating system independent and simply requires [Java Runtime Enivronment](https://en.wikipedia.org/wiki/Java_virtual_machine#Execution_environment).

#### Prearrangement: Open terminal
- Windows: Key combination **Windows key + R**
- OS X: Key combination **cmd + Space bar**, type **terminal** and then press Enter
- Linux: Key combination **Ctrl + Alt + T**

#### Installing Java
1. Type `java -version` into the terminal and press Enter to check whether the correct version is installed or not
2. If `command not found` is displayed, download the appropriate installation file from the [Oracle website] (http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) (at least v1.8)
3. Follow the instructions of the installation manager

**Note Windows users**: To determine whether a **32-bit** or **64-bit** version of Windows is installed, click with the right mouse button on the **Windows** icon, click **System**. Check the line **System Type**.

#### DARIAH-DKPro-Wrapper ready-to-use
1. Download [here](https://github.com/DARIAH-DE/DARIAH-DKPro-Wrapper/releases) the ZIP-archive of the current release, e.g. **ddw-0.4.5.zip**
2. Unpack the archive
3. Type ` cd /path/to/extracted/archive` into the terminal
4. Make sure that the actual [path](https://en.wikipedia.org/wiki/Path_(computing)) is set and press Enter

#### Using DARIAH-DKPro-Wrapper
1. To test the DKPro-Wrapper, download a text example [here](https://wiki.de.dariah.eu/download/attachments/40213783/EffiBriestKurz.txt)
2. Type `java -Xmx4g -jar ddw-0.4.5.jar -language de -input /pfad/zu/EffiBriestKurz.txt -output .` into the terminal, make sure the `-input` parameter leads to the actual file and press Enter
3. If the following lines will be displayed, everything works out just fine

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

**Note**: A [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) file with annotated text has been created and placed in the previously unpacked archive.
