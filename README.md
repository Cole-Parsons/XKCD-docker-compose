# XKCD-docker-compose
A Docker Compose setup that runs the complete XKCD system — including the Go-based XKCD Server, XKCD Client, and React Frontend — in a unified multi-container environment.
---
## Prerequisites
* Docker Desktop v4.25+
* Docker compose v2.20+
* Git Latest
---
## Overview
The purpose of this Repository is to assist you in running all 3 XKCD Scraper Projects simultaniously in Docker.
---
# How To
* First ensure you have downloaded all 3 projects locally in their own files.
  [XKCD-Server](https://github.com/Cole-Parsons/XKCD-Scraper-HTTP-Server.git)    
  [XKCD-Client](https://github.com/Cole-Parsons/XKCD-Client.git)  
  [XKCD-Frontend](https://github.com/Cole-Parsons/XKCD-frontend.git)  

* Then put all 3 Repository files and docker-compose.yml file into the same parent folder. It should look like this
<pre>
parent-folder/
│
├── docker-compose.yml
├── XKCD-Server
├── XKCD-Client
└── XKCD-Frontend
</pre>

* Next Open up your terminal and cd into your parent folder with the 3 Repositories and docker-compose.yml file  
`cd parent-folder`

* Now build and run
`docker compose up --build`
* You should now see all 3 containerized in your Docker desktop.
---
## Access
Frontend: http://localhost:3000  
Server API: http://localhost:8080

