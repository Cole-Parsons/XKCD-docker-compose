# XKCD-docker-compose
A Docker Compose setup that runs the complete XKCD system — including the Go-based XKCD Server, XKCD Client, and React Frontend — in a containerized environment.
---
## Prerequisites  
* Docker Desktop v4.25+  
* Docker compose v2.20+  
* Git Latest  
---
## Overview 
The purpose of this repository is to assist you in running all 3 XKCD Scraper Projects simultaniously in Docker.  
---
# How To  
* First create a new folder and cd into it  
* Then clone the projects to your parent folder  
```bash
git clone https://github.com/Cole-Parsons/XKCD-Scraper-HTTP-Server
git clone https://github.com/Cole-Parsons/XKCD-Client
git clone https://github.com/Cole-Parsons/XKCD-frontend
```
* Next put the [docker-compose file](https://github.com/Cole-Parsons/XKCD-docker-compose/blob/main/docker-compose.yml) into the parent folder. It should look like this.  
<pre>
parent-folder/
│
├── docker-compose.yml
├── XKCD-Server
├── XKCD-Client
└── XKCD-Frontend
</pre>

* Now build and run
`docker compose up --build`
* You should now see all 3 containerized in your Docker desktop.
---
## Access
Frontend: http://localhost:3000  
Server API: http://localhost:8080

