The docker-compose file contains one http backend, one gocd server and one gocd agent:

* GoCD Server is from official GoCD github page: https://github.com/gocd/docker-gocd-server
* GoCD agent that is based on Docker DinD image https://hub.docker.com/r/gocd/gocd-agent-docker-dind
* HTTP backend from Docker git-http-backend image: https://hub.docker.com/r/gocdcontrib/git-http-backend


Note:

* The server and agents will take a while to initialize and startup correctly. GoCD agent will automatically register with GoCD server (however agents need to be enabled from server UI before they can be used for any pipeline).
* GoCD server can be accessed through: http://localhost:8156

Start docker compose command: `docker-compose up`