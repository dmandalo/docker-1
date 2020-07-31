FROM debian

RUN apt-get update && apt-get install -y  cowsay fortune lolcat

ENTRYPOINT /usr/games/fortune | /usr/games/cowsay | /usr/games/lolcat

#docker build -t b05
#docker run --rm b05