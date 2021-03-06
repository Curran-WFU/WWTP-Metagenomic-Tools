# WWTP-Metagenomic-Tools

A set of small databases and a program for analyzing genus-level taxons in metagenomes from wastewater treatment plant reactors. The program will run either in Google Colaboratory or on personal computers.  

A.  Database files:

  1. The database of seven Activated Sludeg Aeration Basins, MGIT.A_H.Ex.C.500.Genera.Freq.csv ; 
  
  2. The same database but without the ASB from Switzerland, MGIT.A_H.Ex.EC.500.Genera.Freq.csv ;
  
  3.  A metagenome from an ASB effluent that produced foam in the final clarifer, A.I.Fm1.4663792.3_organism_genus_hits.csv ;
  
  4.  A metagenome from a high-ammonia adapted ASB in Switzerland, A.e.Switzerland.4568625.3_organism_genus_hits.csv .

B. A program for comparing metagenomes to a reference ASB genus database:  "MG_Plotter.ipynb", that will make plots of your input file vs. the reference ASB database.  

C.  All input metagenome file names and file formats must be standardized.  

Input files should be "comma-delimited" (*.csv) and have two columns of data, the first should conatin genus names, and the second should contain the number of "hits" for the corresponding genus.  The file should also be sorted from high-to-low by numbers of hits.  The Python progam will determine the total number of hits for the database and then calculate frequencies for each genus.  

Filenames must have 6 parts, each separated by a "."  As an example:  A.Z.USA.4663792.3_organism_genus_hits.csv   In this filename, the first two letters are for internal tracking, the third is the country where the sample was isolated, the fourth is the metagenome number assigned by MG-RAST, the fifth contains information about the data in the file, and "csv" is the extension for a comma-delimited file.

