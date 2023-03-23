The docker-compose file contains one server and one agent:

* Server is from official GoCD github page: https://github.com/gocd/docker-gocd-server
* GoCD agent that is based on Docker DinD image https://hub.docker.com/r/gocd/gocd-agent-docker-dind


Note:

* The server and agents will take a while to initialize and startup correctly. GoCD agent will automatically register with GoCD server (however agents need to be enabled from server UI before they can be used for any pipeline).
* GoCD server can be accessed through: http://localhost:8155