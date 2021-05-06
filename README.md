# Minecraft server
This project is a ready to deploy structure of minecraft game multiplayer server.
Before start it, make sure you have `docker` and `docker-compose` installed.
# Deploy
## First 
After project cloned, create a copy of `.env.sample` in project directory and name it `.env`.
## Second 
Fill `.env` file.<br/>
`LOCAL_PORT` - port number on your server/local machine that you want to map container port to it. <br/>
`MAX_RAM` - maximum ram size that you want server use. e.g. `2G` or `2048M`<br/>
`MIN_RAM` - minimum ram size that you want server use. e.g. `1G` or `1024M`
## Third
In project directory, run `docker-compose -f docker-compose.yml up -d` and try to connect to your `server_ip/local_ip:server_port`.<br/>
Wish you enjoy it.
# Change server properties
To change server behavoir, you have to modify `server.properties` file and `docker-compose -f docker-compose.yml restart -d` or `docker-compose -f docker-compose.yml down` and after that run `docker-compose -f docker-compose.yml up -d --build`.
