To start project without docker

clone repo

navigate to project directory in git bash


run git submodule init
run git submodule sync
run git submodule --recursive --update --init

open dev-services and interview-services in spring tool suite
boot up service-registry, user-service, interview-service, then api-gateway
in that order for most consistent results

open front-end in either vs code or git bash or similar command line
run npm install

then run ng serve

open then project on localhost:4200

for reference h2 local databases are on,
	User: 50222
	interview-service: 50111

you will need to make a user user-service db to login into the site