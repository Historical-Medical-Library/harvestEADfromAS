# harvestEADfromAS
A Python script for writing .xml files in EAD to your local machine from online ArchivesSpace instances.

In order to run the script you will need Python 3.

Four parameters must be set within the script before running: the URL of the AS instance you wish to pull EAD from, the repository id of the repository you wish to pull the EAD from, the range of resource ids that you wish to crawl and the local directory you wish to save the XML files in. The script will create a new directory named after the URL within the directory path you set and add the files one by one with the naming convention of resource id and accession number (the same naming convention used by the ead_export.sh script provided in AS). Resource ids not in the database or that point to empty records will be skipped.

Note: for instances with more than one repository, each will need to crawled individually. Another loop could be added to do it programatically, but since the majority of archives I've check use only one, I've left it as it. Checking for multiple repositories is simple, type the base url followed by /repositories/ and an id into your browser (such as http://cpparchives.org/repositories/2), if it exists you will see a listing of all the objects in it, if not you'll be met with an error page. If you wish to save these in different directories, simple change the directory name in line 39 such as <code>directory = archiveName + '_EADXML_repo5'</code>.

Comments within the script provide more information.

Written by Tristan Dahn at The Historical Medical Library of The College of Physicians of Philadelphia.

e-mail: tdahn@collegeofphysicians.org
