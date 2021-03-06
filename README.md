# Kafka Java App

## Group Members
 - Golla Durga Prasad
 - RaviTeja Pagidoju
 - Gopichand Bandarupalli
 - Pruthvi Naskanti
 - Shiva Rama Krishna Vodnala
 - Sai Krishna Emmadishetty
 
 <table>
<td align="center"><a href="https://github.com/GD-Prasad"><img src="https://avatars.githubusercontent.com/u/59986885?s=400&u=df8057f5d9aa0936da702cdb1a5a776ceddf12a5&v=4" width="100px;" alt=""/><br /><sub><b>GD Prasad</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/RaviTeja444"><img src="https://github.com/chanduhvg/Flink-Fraud-Scala/blob/main/Ravi_pic.jpeg?raw=true" width="100px;" alt=""/><br /><sub><b>Ravi Teja Pagidoju</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/chanduhvg"><img src="https://avatars.githubusercontent.com/u/60024244?s=460&u=1f54a606cfb5ca1af59d89980ccd0597c0794b17&v=4" width="100px;" alt=""/><br /><sub><b>Gopichand Bandarupalli</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/pruthvi-naskanti"><img src="https://github.com/chanduhvg/Flink-Fraud-Scala/blob/main/Pruthvi_pic.jpg?raw=true" width="100px;" alt=""/><br /><sub><b>Pruthvi Naskanti</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/srkvodnala"><img src="https://avatars.githubusercontent.com/u/28599511?s=400&u=b1f6f569110d0150f844184d33a3d7b8e0a4dc4b&v=4" width="100px alt=""/><br /><sub><b>Shiva Rama Krishna</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/Saikrishna1545"><img src="https://avatars.githubusercontent.com/u/60013018?s=460&u=4687be0646ecbb59bd281276c302eba966ff5f64&v=4" width="100px;" alt=""/><br /><sub><b>Sai Krishna Emmadishetty
</b></sub></a><br /></td>

</table>

## Gopichand Bandarupalli - Team Lead

Welccome, I used the random function to display Actor names and Movie names.
 
#### Commands used:

1. Start Zookeeper in kafka folder on C drive.
```
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```
1. Start Kafka in kafka folder on C drive.
```
.\bin\windows\kafka-server-start.bat .\config\server.properties
```
1. Creat a new topic and list all of them.
```
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic gopi-dirc
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list
```
1. Run the MVN command to compile the code.
```
mvn clean compile assembly:single
```
1. Once the build is complete, start Consumer.
```
java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.Consumer gopi-dirc group4
```
1. Then start the Producer.
```
java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.ProducerGopi gopi-dirc
```

#### References:

1. [Dr. Case's Twitter Example](https://github.com/denisecase/kafka-case)
1. [Dr. Case's Kafka Example](https://github.com/denisecase/kafka-api)

## Ravi Teja Pagidoju - Team Member
As part of my work im displaying national park names randomly.
In the used pub-sub model,I have created a Producer file named ProducerRavi.I implemented code such a way a random number is generated from the given national parks list length.Based on the random number generated im displaying the national parks using the number as index.

As part of this app,i have to run the following
- Zookeeper
- Kafka Service
- Consumer
- Producer

For acheiving the above,i have used the following commands
- ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties```
- ```.\bin\windows\kafka-server-start.bat .\config\server.properties```
- ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic raviteja-kafka-messages```
- ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list```
- ```java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.Consumer raviteja-kafka-messages test2```
- ```java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.ProducerRavi raviteja-kafka-messages```

Refrences:
- [Kafka Example](https://github.com/denisecase/kafka-api)

## Sai Krishna Emmadishetty - Team member

I used the random function to display Resturant, Prices and items.
 
#### Commands used:

1. Start Zookeeper in kafka folder on C drive.
```
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```
1. Start Kafka in kafka folder on C drive.
```
.\bin\windows\kafka-server-start.bat .\config\server.properties
```
1. Creat a new topic and list all of them.
```
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic saikrishna-msg
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list
```
1. Run the MVN command to compile the code.
```
mvn clean compile assembly:single
```
1. Once the build is complete, start Consumer.
```
java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.Consumer saikrishna-msg group4
```
1. Then start the Producer.
```
java -cp target/kafka-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.bigdatasection1group4.ProducerSai saikrishna-msg
```

#### References:
- (https://github.com/denisecase/kafka-api)

