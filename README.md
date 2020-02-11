Nginx setup as a reverse proxy, running on Docker.

Prerrequisites:
- Docker installed

Instructions:
1- Clone repo
2- Edit default.conf and on line 5 replace port 8000 with your local port
3- sudo docker build -t rproxy
4- sudo docker run -d --name rproxy -p 80:80 -p 443:443 --network="host" rproxy
