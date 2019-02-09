#Tools for ACI

Description

This code/tools will allow an Engineer to retrieve data and push data very easy and fast for the ACI Fabric. 
The user will be accessing an existing fabric for this exercise. The process uses two different methods which are the ACITOOLKIT and POSTMAN. 
There will be a series of installation to get the system ready for this. The idea is to use various methods toi accomplish this.

Installation

	Install pip
	Install python
	Install the requirements.txt = pip install -r requirements.txt
	Download the acitoolkit and install via https://github.com/datacenter/acitoolkit
	Install and setup acitoolkit - https://acitoolkit.readthedocs.io/en/latest/tutorialsetup.html
	Install virtualenv
		Create a virtual environment in your laptop (This is so the space in which you will run the various scripts are totally clean)
		You will be working from this environment
	Install Postman
		
Usage
	ACITOOLKIT
	The acitoolkit README.md file has all the instructions in how to install python and all the environments required
		Make sure you are using the credentials.py file provided in the build as it already has the information to login into the fabric.

	POSTMAN
	Download the ACI Collection file called ACI-Inspector.postman_collection.json
	Download the ACI Runner environment called ACI-Runner-Tenant-Environment.postman_environment.json
	
		
Files

credentials.py - Contains the login credentials REQUIRED to access the ACI Fabric
ACI-Runner-Tenant-Environment.postman_environment.json - has the correct environment variables to run the scripts from the collection file
ACI-Inspector.postman_collection.json - collection files which has the items to run
The phython scripts are within the acitoolkit/samples directiory. Here are some of the scripts to be run against the fabric:
	yourprompt$ python aci-show-external-networks.py
	yourprompt$ python aci-show-subnets.py
	yourprompt$ python aci-show-epgs.py 
	yourprompt$ python aci-create-epg.py --tenant ROCKS1 --app APP_ROCKS1 --bd ROCKS1-BD --epg ROCKS1-EPG1 (Creating an EPG)
	yourprompt$ python aci-show-faults-by-domain.py 
	
	You can go to the acitoolkit/samples and look at more scripts to run and modify to your needs.
