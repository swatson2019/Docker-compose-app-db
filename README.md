Docker commands:

# Run docker compose
docker-compose up

# Remove all unused containers and images
docker system prune -a

# waste code
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6
RUN echo "deb [ arch=amd64 ] http://repo.mongodb.org/apt/ubuntu/ xenial/mongodb-org/3.4 multiverse" |  tee /etc/apt/sources.list.d/mongodb-3.4.list
RUN apt-get update && apt-get install -y mongodb
