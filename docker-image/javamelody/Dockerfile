### Dockerfile

FROM openjdk:11

COPY . /usr/src/javamelodyclusterjar

CMD java -server -Dapp.home=/usr/src/javamelodyclusterjar/home -Xmx128m -jar /usr/src/javamelodyclusterjar/collector_server.war --httpPort=1337