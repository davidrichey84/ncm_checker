# ncm_checker
Checks the installed version of Nimble Connection Manager on Windows machines by grabbing microsoft IQNs from the nimble array

# Info
This project uses the Nimble Storage class from Casey Crawford and can be found @ https://github.com/caseycrawford/nimblestorage_python
Both .py source and a compiled stand-alone .exe are included with this project. If you do not have a python environment installed and built then I recommend the executable. I am working on a full build with 'requirements.txt' all worked out that will bring in all necessary pieces if you do want to run from source. 
This script will ***only work when being run on a windows box with proper remote access to servers you are checking. It works by utilizing the windows command line 'wmic' commands to check for installed software and assumes you have not set custom IQNs for your servers.***

# How-To
Run using python like so: "python ncm_checker.py" 
Use the compiled binary: "ncm_checker.exe"


You will be prompted for the following: a) nimble array hostname b) username c) password. 
***at no point are credentials stored***

# In-Progress
Exploring the option of automatically (if desired) uninstalling the NCM and upgrading to the new one along with all required KBs from MS. Also working on checking several arrays instead of just one. 

# Python Requirements (here, for now)
-requests
