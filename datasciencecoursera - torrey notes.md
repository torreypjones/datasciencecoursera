#Notes for DataScienceToolbox course on coursea

## Assignment Steps
 - Install R (http://cran.r-project.com)
 - Install R Studio (http://rstudio.com)
 - Install git (http://git-scm.com)
	- open git bash & configure git username / email:
	```
	git config user.name "Torrey Jones"
	git config user.email "torreypjones@gmail.com"
		TJones@BOI-NTB-TJONES ~
		$ git config -l
		core.symlinks=false
		core.autocrlf=true
		color.diff=auto
		color.status=auto
		color.branch=auto
		color.interactive=true
		pack.packsizelimit=2g
		help.format=html
		http.sslcainfo=/bin/curl-ca-bundle.crt
		sendemail.smtpserver=/bin/msmtp.exe
		diff.astextplain.textconv=astextplain
		rebase.autosquash=true
		user.name=Torrey Jones
		user.email=torreypjones@gmail.com
	```
 - Create GitHub account
 - create GitHub repository (https://github.com/torreypjones/datasciencecoursera)
 - create local directory to sync with newly created github repository
	Note: the class video's implied the following would work (but see below for wahat i actually did):
	- open git bash and run the following:
	```
		TJones@BOI-NTB-TJONES ~/
		mkdir ~/datasciencecoursera
		TJones@BOI-NTB-TJONES ~/
		cd ~/datasciencecoursera
		TJones@BOI-NTB-TJONES ~/datasciencecoursera
		$ git init
		Initialized empty Git repository in c:/Users/TJones/datasciencecoursera/.git/

		TJones@BOI-NTB-TJONES ~/datasciencecoursera (master)
		$ git remote add origin https://github.com/torreypjones/datasciencecoursera.git
	```
		
	what i actually did was:
	```
		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox
		$ git clone https://github.com/torreypjones/datasciencecoursera datasciencecoursera_repository
		Cloning into 'datasciencecoursera_repository'...
		remote: Counting objects: 3, done.
		remote: Compressing objects: 100% (2/2), done.
		remote: Total 3 (delta 0), reused 0 (delta 0)
		Unpacking objects: 100% (3/3), done.
		Checking connectivity... done.

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox
		$ cd datasciencecoursera_repository/

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$ ll
		total 1
		-rw-r--r--    1 TJones   Administ       68 Jan 18 09:16 README.md

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$ mv ../datasciencecoursera\ -\ torrey\ notes.txt ./

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$ git add .

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$ git commit -am "added notes txt file"
		[master 281cbf4] added notes txt file
		 1 file changed, 41 insertions(+)
		 create mode 100644 datasciencecoursera - torrey notes.txt

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$ git push origin master
		Username for 'https://github.com': torreypjones
		Password for 'https://torreypjones@github.com':
		Counting objects: 4, done.
		Delta compression using up to 4 threads.
		Compressing objects: 100% (3/3), done.
		Writing objects: 100% (3/3), 875 bytes | 0 bytes/s, done.
		Total 3 (delta 0), reused 0 (delta 0)
		To https://github.com/torreypjones/datasciencecoursera
		   1f0a707..281cbf4  master -> master

		TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
		oursera_repository (master)
		$
		```

# Random Notes
## conigure github repo to always use same username/password for this remote origin:		
	```
	TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
	oursera_repository (master)
	$ git config remote.origin.url https://username:password@github.com/torreyp
	jones/datasciencecoursera/

	TJones@BOI-NTB-TJONES ~/Google Drive/DataScience/DataScienceToolbox/datasciencec
	oursera_repository (master)
	$ git push origin master
	Everything up-to-date
	```
	
## markdown syntax
	- pound signs (#) create headers; add more pound signs to add sub-headings
	- use asterisks (*) to create bulleted lists