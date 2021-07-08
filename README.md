1) Start Zookeeper
cmd>cd C:\kafka_2.12-2.6.0
cmd> .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

2) Start Kafka setup
cmd> cd C:\kafka_2.12-2.6.0
cmd> .\bin\windows\kafka-server-start.bat .\config\server.properties

3) Create a Topic

cmd>.\bin\windows\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic myKafkaTest
4) Run Spring Boot Application

5) After starting application Enter below URLs on the Browser and test the results

♦ http:// localhost:9090/send?msg=I like
♥ http:// localhost:9090/send?msg=to work on
♦ http:// localhost:9090/send?msg=Kafka
♥ http:// localhost:9090/send?msg=with Spring Boot

   http://localhost:9090/getAll
