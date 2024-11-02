# Apache-kafka


1. zookeeper start windows command
   -> bin\windows\zookeeper-server-start.bat config\zookeeper.properties
   
  2. Running kafka cluster server
  -> bin\windows\kafka-server-start.bat config\server.properties
  
  3. Creating kafka topics 
  -> bin\windows\kafka-topics.bat --create --topic quickstart-events --bootstrap-server localhost:9092
  
  4. creating topics with producer
  -> bin\windows\kafka-console-producer.bat --topic quickstart-events --bootstrap-server localhost:9092
  
  5. creating consumer events (with same id which is quickstart-events to listen)
  -> bin\windows\kafka-console-consumer.bat --topic quickstart-events --from-beginning --bootstrap-server (from beginning will read from start)
  -> bin\windows\kafka-console-consumer.bat --topic quickstart-events --bootstrap-server (this will read from point the consumer created)
  
  
  ***IMPORTANT POINTS -> First we need to start zookeeper server before starting the kafka server
