# Apache Kafka

## Introduction

Apache Kafka® is a distributed streaming platform.

A streaming platform has three key capabilities:

* Publish and subscribe to streams of records, similar to a message queue or enterprise messaging system.
* Store streams of records in a fault-tolerant durable way.
* Process streams of records as they occur. Kafka is generally used for two broad classes of applications:
* Building real-time streaming data pipelines that reliably get data between systems or applications
* Building real-time streaming applications that transform or react to the streams of data

  To understand how Kafka does these things, let's dive in and explore Kafka's capabilities from the bottom up.

First a few concepts:

* Kafka is run as a cluster on one or more servers that can span multiple datacenters.
* The Kafka cluster stores streams of records in categories called topics.
* Each record consists of a key, a value, and a timestamp.

## References

* [https://kafka.apache.org/](https://kafka.apache.org/)
* Tutorial [https://www.udemy.com/apache-kafka/](https://www.udemy.com/apache-kafka/)
* Books [https://www.confluent.io/apache-kafka-stream-processing-book-bundle](https://www.confluent.io/apache-kafka-stream-processing-book-bundle)
* GCP [https://cloud.google.com/blog/big-data/2018/05/google-cloud-platform-and-confluent-partner-to-deliver-a-managed-apache-kafka-service](https://cloud.google.com/blog/big-data/2018/05/google-cloud-platform-and-confluent-partner-to-deliver-a-managed-apache-kafka-service)
* AWS [https://aws.amazon.com/kafka/](https://aws.amazon.com/kafka/), [https://aws.amazon.com/quickstart/architecture/confluent-platform/](https://aws.amazon.com/quickstart/architecture/confluent-platform/), [https://www.confluent.io/confluent-cloud/](https://www.confluent.io/confluent-cloud/)
* Beam has KafkaIO [https://cloud.google.com/blog/big-data/2016/09/apache-kafka-for-gcp-users-connectors-for-pubsub-dataflow-and-bigquery](https://cloud.google.com/blog/big-data/2016/09/apache-kafka-for-gcp-users-connectors-for-pubsub-dataflow-and-bigquery)
* Spring Boot and Kafka [https://cloud.spring.io/spring-cloud-stream/](https://cloud.spring.io/spring-cloud-stream/)
* Kafka has many connectors [https://www.confluent.io/product/connectors/](https://www.confluent.io/product/connectors/) one for Blockchain.info too
* KSQL - enables something really effective: reading, writing and transforming data in real-time and a scale using a semantic already known by the majority of the community working in the data space, the SQL! [https://www.confluent.io/product/ksql/](https://www.confluent.io/product/ksql/) oraz [https://www.rittmanmead.com/blog/2017/10/ksql-streaming-sql-for-apache-kafka/](https://www.rittmanmead.com/blog/2017/10/ksql-streaming-sql-for-apache-kafka/)

  similar to blockchain in some way [https://www.rittmanmead.com/blog/2017/10/ksql-streaming-sql-for-apache-kafka/](https://www.rittmanmead.com/blog/2017/10/ksql-streaming-sql-for-apache-kafka/)

* it is fast [https://softwaremill.com/mqperf/](https://softwaremill.com/mqperf/)
* you can keep data forever there ... [https://www.confluent.io/blog/okay-store-data-apache-kafka/](https://www.confluent.io/blog/okay-store-data-apache-kafka/)
* Google PubSub vs Kafka [https://stackoverflow.com/questions/38572071/i-am-evaluating-google-pub-sub-vs-kafka](https://stackoverflow.com/questions/38572071/i-am-evaluating-google-pub-sub-vs-kafka)
* Neo4j Use Case: Low Latency Graph Analytics & OLTP - Update 1M Nodes in 90 secs with Kafka and Neo4j Bolt [https://gist.github.com/graphadvantage/a148613f75818897e396a64957dc6ef1](https://gist.github.com/graphadvantage/a148613f75818897e396a64957dc6ef1)
* Streaming Comparison [https://databaseline.bitbucket.io/images/2016-03-12-apache-streaming-technologies.png](https://databaseline.bitbucket.io/images/2016-03-12-apache-streaming-technologies.png)
* What is Apache Kafka? Why is it so popular? Should you use it? [https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it](https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it)
* [https://content.pivotal.io/blog/understanding-when-to-use-rabbitmq-or-apache-kafka](https://content.pivotal.io/blog/understanding-when-to-use-rabbitmq-or-apache-kafka)
* [https://www.infoq.com/articles/apache-kafka](https://www.infoq.com/articles/apache-kafka)
* Free books bundle [https://www.confluent.io/apache-kafka-stream-processing-book-bundle](https://www.confluent.io/apache-kafka-stream-processing-book-bundle)
* [https://blog.scottlogic.com/2018/04/17/comparing-big-data-messaging.html](https://blog.scottlogic.com/2018/04/17/comparing-big-data-messaging.html)
* Rabbit & Kafka microservices [https://news.ycombinator.com/item?id=11284765](https://news.ycombinator.com/item?id=11284765)
* Rabbit & Kafka [https://tech.trello.com/why-we-chose-kafka/](https://tech.trello.com/why-we-chose-kafka/)
* Rabbit & Kafka [https://blog.mavenhive.in/which-one-to-use-and-when-rabbitmq-vs-apache-kafka-7d5423301b58](https://blog.mavenhive.in/which-one-to-use-and-when-rabbitmq-vs-apache-kafka-7d5423301b58)
* [https://www.confluent.io/blog/event-driven-2-0](https://www.confluent.io/blog/event-driven-2-0)
* [https://www.confluent.io/product/confluent-platform/](https://www.confluent.io/product/confluent-platform/)
* [https://www.slideshare.net/ConfluentInc/common-patterns-of-multi-datacenter-architectures-with-apache-kafka](https://www.slideshare.net/ConfluentInc/common-patterns-of-multi-datacenter-architectures-with-apache-kafka)
* [https://www.slideshare.net/ConfluentInc/common-patterns-of-multi-datacenter-architectures-with-apache-kafka](https://www.slideshare.net/ConfluentInc/common-patterns-of-multi-datacenter-architectures-with-apache-kafka)

## Apache Kafka and Microservices

* [https://www.slideshare.net/KaiWaehner/eventdriven-microservices-with-apache-kafka-kafka-streams-and-ksql](https://www.slideshare.net/KaiWaehner/eventdriven-microservices-with-apache-kafka-kafka-streams-and-ksql)
* [https://www.confluent.io/blog/building-a-microservices-ecosystem-with-kafka-streams-and-ksql/](https://www.confluent.io/blog/building-a-microservices-ecosystem-with-kafka-streams-and-ksql/)
* [https://github.com/ewolff/microservice-kafka](https://github.com/ewolff/microservice-kafka)
* [https://www.slideshare.net/wangxia5/netflix-kafka](https://www.slideshare.net/wangxia5/netflix-kafka)
* [https://medium.com/netflix-techblog/kafka-inside-keystone-pipeline-dd5aeabaf6bb](https://medium.com/netflix-techblog/kafka-inside-keystone-pipeline-dd5aeabaf6bb)
* [https://blog.keen.io/architecture-of-giants-data-stacks-at-facebook-netflix-airbnb-and-pinterest-9b7cd881af54](https://blog.keen.io/architecture-of-giants-data-stacks-at-facebook-netflix-airbnb-and-pinterest-9b7cd881af54)
* [https://engineering.linkedin.com/blog/2016/04/kafka-ecosystem-at-linkedin](https://engineering.linkedin.com/blog/2016/04/kafka-ecosystem-at-linkedin)
* [https://engineering.linkedin.com/kafka/running-kafka-scale](https://engineering.linkedin.com/kafka/running-kafka-scale)
* [https://www.thoughtworks.com/radar/techniques/recreating-esb-antipatterns-with-kafka](https://www.thoughtworks.com/radar/techniques/recreating-esb-antipatterns-with-kafka)

## Apache Kafka and Blockchain

* [https://www.linkedin.com/pulse/scaling-blockchains-apache-kafka-alex-miller/](https://www.linkedin.com/pulse/scaling-blockchains-apache-kafka-alex-miller/)
* [https://codeburst.io/the-abcs-of-kafka-in-hyperledger-fabric-81e6dc18da56](https://codeburst.io/the-abcs-of-kafka-in-hyperledger-fabric-81e6dc18da56)
* [https://made2591.github.io/posts/kakfa-and-blockchain](https://made2591.github.io/posts/kakfa-and-blockchain)
* [https://www.kdnuggets.com/2016/07/postgres-kafka-bitcoin-common.html](https://www.kdnuggets.com/2016/07/postgres-kafka-bitcoin-common.html)
* [https://www.linkedin.com/pulse/immutable-append-only-log-blockchain-apache-kafka-rajesh-yogi/](https://www.linkedin.com/pulse/immutable-append-only-log-blockchain-apache-kafka-rajesh-yogi/)
* [https://www.landoop.com/docs/lenses/1.0/lenses/connectors/source/blockchain.html](https://www.landoop.com/docs/lenses/1.0/lenses/connectors/source/blockchain.html)
* [https://github.com/lucrussell/kafka-blockchain](https://github.com/lucrussell/kafka-blockchain)
* [http://kafka-connect-ui.landoop.com/\#/cluster/UAT](http://kafka-connect-ui.landoop.com/#/cluster/UAT)
* [http://hyperledger-fabric.readthedocs.io/en/release/kafka.html](http://hyperledger-fabric.readthedocs.io/en/release/kafka.html)
* [https://docs.google.com/document/d/1vNMaM7XhOlu9tB\_10dKnlrhy5d7b1u8lSY8a-kVjCO4/](https://docs.google.com/document/d/1vNMaM7XhOlu9tB_10dKnlrhy5d7b1u8lSY8a-kVjCO4/)
* [https://symbiont.io/blog/2016/10/18/introducing-symbiont-assembly](https://symbiont.io/blog/2016/10/18/introducing-symbiont-assembly)
* [https://www.reddit.com/r/Bitcoin/comments/53d9cq/what\_advantage\_does\_a\_private\_blockchain\_have/](https://www.reddit.com/r/Bitcoin/comments/53d9cq/what_advantage_does_a_private_blockchain_have/)
* [https://github.com/btccom/btcpool](https://github.com/btccom/btcpool)

