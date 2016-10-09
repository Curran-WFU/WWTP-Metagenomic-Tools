# WWTP-Metagenomic-Tools

A set of small databases and programs for analyzing metagenomes from wastewater treatment plant reactors. These programs will run on personal computers.  

A.  Components in this site:

We provide three database files.  The Global MG file is a reference database containing averages, standard deviations, and other data on genera from eight activated sludge basins (ASB) from WWTP around the globe.  One may compare their own WWTP samples to this reference.  For demonstration purposes we include two other files.  The "foam" file contains a list of genera and their numbers of occurrence from an ASB during a surface foam episode.  The "anaerobic" file contains genera and numbers for a mesophilic anaerobic digester. 

We also provide a program, "1.MGIT.Compare.MG.GASM.1.py", that will make plots of your input file vs. the reference ASB database.  

B.  What your computer must have installed in order to run this program:

Python version 2.7, numpy, and matplotlib. These may be downloaded for free with the Anaconda Python package.  You will also need a Python IDE (editor/interpreter).  I recommend Wing 101, which may be downloaded for free.  There are many other good IDEs available. 

The program (1.MGIT.Compare...) and all of the databases that you intend to use should be in the same directory.  

C.  How to run the program:

Open your IDE and from the file menu, open the 1.MGIT program.  You can then run it!  

The program will prompt you for a filename.  For plots using the control foamy and ananerobic databases, enter "f" or "n", respectively.  To enter your database, type (or 'copy-paste') its filename at the prompt. 

The program will then prompt you for a plot type.  

D. Other important details:

All input metagenome file names and file formats must be standardized.  Input files should be "comma-delimited" (*.csv) and have two columns of data, the first should conatin genus names, and the second should contain the number of "hits" for the corresponding genus.  The file should also be sorted from high-to-low numbers of hits.  The Python progam will determine the total number of hits for the database and then calculate frequencies for each genus.  Filenames must have 6 parts, each separated by a "."  As an example:  A.Z.USA.4663792.3_organism_genus_hits.csv   In this filename, the first two letters are for internal tracking, the third is the country where the sample was isolated, the fourth is the metagenome number assigned by MG-RAST, the fifth contains information about the data in the file, and "csv" is the extension for a comma-delimited file.

Plot interpretation
