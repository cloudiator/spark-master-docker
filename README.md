# Apache Spark Master Docker Container

Based on the latest release of [Apache Spark](http://spark.apache.org/)

Current release: Spark 2.3.1 with Hadoop 2.7

------

### Configuration

Required environment variables:

- SPARK_MASTER_PORT => Spark Master PORT

- SPARK_MASTER_UI_PORT => Spark Web Interface

------

### Usage:

```dockerfile
docker run -d -p 7077:7077 -p 8080:8080 -e SPARK_MASTER_PORT=7077  -e SPARK_MASTER_UI_PORT=8080  cloudiator/spark-master:latest
```

