# ports to use:
# 9987:9987/udp
# 10011:10011
# 30033:30033

FROM debian:latest

ENV TS3SERVER_LICENSE=accept

RUN apt-get update
RUN apt-get install wget bzip2 -y

RUN wget https://files.teamspeak-services.com/releases/server/3.9.1/teamspeak3-server_linux_amd64-3.9.1.tar.bz2
RUN tar -jxvf ./*.bz2

ENTRYPOINT ["./teamspeak3-server_linux_amd64/ts3server_minimal_runscript.sh"]
