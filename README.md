# kafkaplay


Based off of: https://medium.com/pharos-production/kafka-using-java-e10bfeec8638 tutorial

docker it:
https://www.kaaproject.org/kafka-docker


<h2>Run the Producer locally via cmd</h2>
Navigate to the producer module directory
Run and make jar for **Producer** with:  mvn clean compile assembly:single

<h2>Run the Producer via Docker</h2>
From the root of the project, run:
docker build -t demo .

docker run -it demo:latest --network="host" -p 9092:9092 2181:2181


current bug - build nested jar in maven multi project
https://stackoverflow.com/questions/20801874/how-to-build-an-executable-jar-from-multi-module-maven-project