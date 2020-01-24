Getting Started Docker Version

If you dont have windows 10 pro or enterprise
-------
navigate to docs.docker.com/toolbox/toolbox-install_windows/

You might have to enable virtualization in your bios

scroll down to step 2: Install docker toolbox
	Click toolbox releases
	As of the time of writing version 19.03.1

Make sure full installation is selected
--------
if you have pro or enterprise
download docker desktop
--------
once you have either tool box or desktop installed

open docker quickstart terminal
	allow admin access

try docker ps

this shows your docker containers it should be empty

docker pull hello-world

docker ps

you should now see a container with hello world

now open a system explorer window and navigate to where you want to house the project

clone interview-tracker

https://github.com/revaturelabs/interview-tracker

navigate into folder with git bash

	run git submodule init
	run git submodule sync
	run git submodule --recursive --init

now in your docker terminal navigate to the repo
	run docker-compose config

this will check your docker-compose file for errors

now run docker-compose up

It will autobuild

After autobuild look up your docker IP
and use your docker IP to access the website on port :4200
and your 
 postrgres on interview-service
	 port : 5432
	 user : postgres
     password : password
           db : interviewDB

 postgres on user-service
	 port : 5433
	 user : postgres
     password : password
           db : userDB
	
