FROM openjdk:8u242-stretch
ENV DAEMON_RUN=true
ENV SPARK_VERSION=3.0.1
ENV HADOOP_VERSION=2.7
ENV SPARK_HOME=/spark
RUN apt-get update && apt-get install -y curl vim wget software-properties-common ssh net-tools ca-certificates jq ca-certificates wget tar
RUN wget --no-verbose https://mirror.klaus-uwe.me/apache/spark/spark-${SPARK_VERSION}/spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz && tar -xvzf spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
      && mv spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION} spark \
      && rm spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz