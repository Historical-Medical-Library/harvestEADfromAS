# exportEADfromAS
A Python script for writing .xml files in EAD to your local machine from online ArchivesSpace instances.

In order to run the script you will need Python 3.

Four parameters must be set within the script before running: the URL of the AS instance you wish to pull EAD from, the repository id of the repository you wish to pull the EAD from, the range of resource ids that you wish to crawl (to view a full list of resources from a given instance navigate to http://example-archive.com/search?type=resource and look at the number of results) and the local directory you wish to save the XML files in. The script wil create a new directory named after the URL within the directory path you set and add the files one by one with the naming convention of resource id and accession number. Resource ids with no records will be skipped.

Comments within the script provide more information.

Written by Tristan Dahn at The Historical Medical Library of The College of Physicians of Philadelphia.
