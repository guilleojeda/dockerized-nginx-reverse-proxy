Nginx setup as a reverse proxy, running on Docker.

Prerrequisites:
- Docker installed

Instructions:
- Clone repo
- Edit default.conf and on line 5 replace port 8000 with your local port
- sudo docker build -t rproxy
- sudo docker run -d --name rproxy -p 80:80 --network="host" rproxy
