Start the ZooKeeper service
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

Start the Kafka broker service
.\bin\windows\kafka-server-start.bat .\config\server.properties

STEP 3: CREATE A TOPIC TO STORE YOUR EVENTS
.\bin\windows\kafka-topics.bat --create --topic topic_demo --bootstrap-server localhost:9092

STEP 4: WRITE SOME EVENTS INTO THE TOPIC
.\bin\windows\kafka-console-producer.bat --topic topic_demo --bootstrap-server localhost:9092

STEP 5:  READ THE EVENTS
.\bin\windows\kafka-console-consumer.bat --topic topic_demo --from-beginning --bootstrap-server localhost:9092
hello world
topic demo

========================
zookeeper.properties — For the dataDir variable, assign your kafka folder path and add the name of the zookeeper data folder as below
![image](https://github.com/code-phenix/KakfaSpringRest/assets/55018311/32d2532d-0467-47f0-b04c-1be9d2545419)

server.properties — In the log.dirs varaibale, assign the path of your Kafka folder and then add the name of the Kafka log data folder as below.

![Uploading image.png…]()

