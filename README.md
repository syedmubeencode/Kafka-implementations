========================== Apache kafka ==========================

Run the application -> kafka
URL :- http://localhost:8080/rest/api/producer?message=%22syed%22

	1)  start zookeeper.start bat file like below
		* Go to this folder (D:\kafka\bin\windows) open cmd prompt and type below command to start zookeeper.start
		(cmd) ->zookeeper-server-start.bat D:\kafka\config\zookeeper.properties
		
	2)  start kafka server
		* Go to this folder (D:\kafka\bin\windows) open cmd prompt and type below command to start zookeeper.start
		(cmd) ->kafka-server-start.bat D:\kafka\config\server.properties
		
	3)  Create Topic:
		* Go to this folder (D:\kafka\bin\windows) open cmd prompt and type below command to start zookeeper.start
		(cmd) ->kafka-topics.bat --create --topic test-topic1 --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1
		NOTE :- Here "test-topic1" -> is topic name.
		
	4)  Consume a message
		* Go to this folder (D:\kafka\bin\windows) open cmd prompt and type below command to start zookeeper.start
		(cmd) ->kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic CodeDecodeTopic
