# exportEADfromAS
A Python script for writing .xml files in EAD to your local machine from online ArchivesSpace instances.

In order to run the script you will need Python 3.

Four parameters must be set within the script before running: the URL of the AS instance you wish to pull EAD from, the repository id of the repository you wish to pull the EAD from, the range of resource ids that you wish to crawl and the local directory you wish to save the XML files in. The script wil create a new directory named after the URL within the directory path you set and add the files one by one with the naming convention of resource id and accession number (the same naming convention used by the ead_export.sh script provided in AS). Resource ids not in the database or that point to empty records will be skipped.

Comments within the script provide more information.

Written by Tristan Dahn at The Historical Medical Library of The College of Physicians of Philadelphia.

e-mail: tdahn@collegeofphysicians.org
