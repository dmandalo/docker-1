# 1) docker build -t minecraft .
# 2) docker run --rm -d -p 25565:25565 minecraft

FROM debian:latest

RUN apt-get update -y && apt-get upgrade -y && \
	apt-get install -y wget && apt-get install default-jdk -y

WORKDIR minecraft-server

RUN wget https://launcher.mojang.com/v1/objects/3737db93722a9e39eeada7c27e7aca28b144ffa7/server.jar

RUN echo "eula=true" > eula.txt

EXPOSE 25565

ENTRYPOINT java -Xmx1024M -Xms1024M -jar server.jar nogui