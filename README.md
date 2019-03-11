# Apache Spark Master Docker Container

Based on the latest release of [Apache Spark](http://spark.apache.org/)

Current release: Spark 2.3.1 with Hadoop 2.7

------

### Configuration

Required environment variables:

- PUBLIC_IP => public IP of the host

- SPARK_MASTER_PORT => Spark Master PORT

- SPARK_MASTER_UI_PORT => Spark Web Interface

- JMS_IP => JMS IP for the Metric Agent

- JMS_PORT => JMS PORT for the Metric Agent

- APP_NAME => name of the application to monitor

------

### Usage:

```dockerfile
docker run -d -p 7077:7077 -p 8080:8080 -e PUBLIC_IP=localhost -e SPARK_MASTER_PORT=7077  -e SPARK_MASTER_UI_PORT=8080 -e JMS_IP=localhost JMS_PORT=61616 -e APP_NAME=dummy   cloudiator/spark-master:latest
```

