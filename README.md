# spark_streaming_kafka_with_twitter
spark streaming kafka with twitter via DStreams

Purpose:
- use twitter as producer to ingest tweets to be used by spark streaming 
- use kafka to implement producer to be used by spark streaming.
- create object class to be the producer for kafka using spark.

Requirements:
- Spark installed
- Twitter library installled
- Kafka library installled

Objective :
- use twitter as producer to generate input data to be consumed be spark streaming.
- implement some logic inside the spark to consume data from kakfa, process data, and send results to kafka.
- use object class in spark to be the engine to send results back to kakfa.

To run Spark :
start-dfs.sh      # start the hadoop daemons
start-master.sh   # start the spark cluster master 
start-slaves.sh   # start the spark cluster slaves
# have the kfk-producer compiled to be used as producer to kafka
spark-shell --master spark://spkm:7077 --jars KfkProducer/target/scala-2.11/kfk-producer_2.11-1.0.0.jar