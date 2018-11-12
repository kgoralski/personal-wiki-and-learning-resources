# Janusgraph

## Introduction 

JanusGraph is a scalable [graph database](http://en.wikipedia.org/wiki/Graph_database) optimized for storing and querying graphs containing hundreds of billions of vertices and edges distributed across a multi-machine cluster.   
JanusGraph is a transactional database that can support thousands of concurrent users executing complex graph traversals in real time.

Official website [http://janusgraph.org/](http://janusgraph.org/)

## Links

* Docs [http://docs.janusgraph.org/latest/](http://docs.janusgraph.org/latest/)
* [https://github.com/JanusGraph/janusgraph/blob/master/docs/basics.adoc](https://github.com/JanusGraph/janusgraph/blob/master/docs/basics.adoc)
* Schema [http://docs.janusgraph.org/latest/schema.html](http://docs.janusgraph.org/latest/schema.html)
* Config reference [http://docs.janusgraph.org/latest/config-ref.html](http://docs.janusgraph.org/latest/config-ref.html)
* Eventual Consistency & ConsistencyModifier.LOCK  [http://docs.janusgraph.org/latest/eventual-consistency.html](http://docs.janusgraph.org/latest/eventual-consistency.html)
* Storage Backends [http://docs.janusgraph.org/latest/storage-backends.html](http://docs.janusgraph.org/latest/storage-backends.html) BigTable, Hbase, Cassandra, ScyllaDB, BerkeleyDB, DynamoDB, InMemory
* Index Backends [http://docs.janusgraph.org/latest/index-backends.html](http://docs.janusgraph.org/latest/index-backends.html) Elastic, Solr, Lucene
* Transactions [http://docs.janusgraph.org/latest/tx.html](http://docs.janusgraph.org/latest/tx.html)
* Bulk Loading [http://docs.janusgraph.org/latest/bulk-loading.html](http://docs.janusgraph.org/latest/bulk-loading.html)
* Optimizing Reads & Writes [http://docs.janusgraph.org/latest/bulk-loading.html\#\_optimizing\_writes\_and\_reads](http://docs.janusgraph.org/latest/bulk-loading.html#_optimizing_writes_and_reads)
* TinkerPop3 docs [http://tinkerpop.apache.org/docs/current/reference/](http://tinkerpop.apache.org/docs/current/reference/)
* SQL2Gremlin [http://sql2gremlin.com/](http://sql2gremlin.com/)
* Practical Gremlin Tutorial [https://github.com/krlawrence/graph](https://github.com/krlawrence/graph) and Book [https://github.com/krlawrence/graph/tree/master/book](https://github.com/krlawrence/graph/tree/master/book)
* Gremlin Recipes [http://tinkerpop.apache.org/docs/current/recipes/](http://tinkerpop.apache.org/docs/current/recipes/)
* JanusGraph Tutorial [https://github.com/marcelocf/janusgraph\_tutorial](https://github.com/marcelocf/janusgraph_tutorial)
* Janusgraph Utils [https://github.com/IBM/janusgraph-utils](https://github.com/IBM/janusgraph-utils)
* Testing [https://github.com/JanusGraph/janusgraph/blob/master/TESTING.md](https://github.com/JanusGraph/janusgraph/blob/master/TESTING.md)
* Write Performance [https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance](https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance)
* Loading data from file [http://tinkerpop.apache.org/docs/current/tutorials/getting-started/\#\_loading\_data](http://tinkerpop.apache.org/docs/current/tutorials/getting-started/#_loading_data)
* [https://github.com/mohataher/awesome-tinkerpop](https://github.com/mohataher/awesome-tinkerpop)
* docs improvement [https://github.com/JanusGraph/janusgraph/issues/452](https://github.com/JanusGraph/janusgraph/issues/452)
* docs improvement [https://github.com/JanusGraph/janusgraph/issues/119](https://github.com/JanusGraph/janusgraph/issues/119)
* [https://stackoverflow.com/questions/40105047/setup-and-configuration-of-titan-for-a-spark-cluster-and-cassandra/40180104\#40180104](https://stackoverflow.com/questions/40105047/setup-and-configuration-of-titan-for-a-spark-cluster-and-cassandra/40180104#40180104)
* [https://stackoverflow.com/questions/41674226/how-does-the-titan-not-backend-storage-clustering-work](https://stackoverflow.com/questions/41674226/how-does-the-titan-not-backend-storage-clustering-work)
* [https://www.compose.com/articles/importing-graphs-into-janusgraph/](https://www.compose.com/articles/importing-graphs-into-janusgraph/)
* [https://developer.ibm.com/dwblog/2018/whats-janus-graph-learning-deployment/](https://developer.ibm.com/dwblog/2018/whats-janus-graph-learning-deployment/) [https://developer.ibm.com/dwblog/2018/janusgraph-composite-mixed-indexes-traversals/](https://developer.ibm.com/dwblog/2018/janusgraph-composite-mixed-indexes-traversals/) [https://cloud.google.com/solutions/running-janusgraph-with-bigtable](https://cloud.google.com/solutions/running-janusgraph-with-bigtable)
* [https://cloud.google.com/blog/big-data/2018/07/developing-a-janusgraph-backed-service-on-google-cloud-platform](https://cloud.google.com/blog/big-data/2018/07/developing-a-janusgraph-backed-service-on-google-cloud-platform)
* [https://stackoverflow.com/questions/46386299/gremlin-server-withremote-connection-closed-how-to-reconnect-automatically](https://stackoverflow.com/questions/46386299/gremlin-server-withremote-connection-closed-how-to-reconnect-automatically)
* [https://stackoverflow.com/questions/47536418/how-to-connect-to-gremlin-server-through-java-using-the-gremlin-driver-with-sess](https://stackoverflow.com/questions/47536418/how-to-connect-to-gremlin-server-through-java-using-the-gremlin-driver-with-sess)
* [http://gremlindocs.spmallette.documentup.com/](http://gremlindocs.spmallette.documentup.com/)

## Traversal promises

[http://tinkerpop.apache.org/docs/3.3.0/upgrade/\#\_traversal\_promises](http://tinkerpop.apache.org/docs/3.3.0/upgrade/#_traversal_promises)

```text
gremlin> promise = g.V().out().promise{it.next()}
==>java.util.concurrent.CompletableFuture@4aa3d36[Completed normally]
gremlin> promise.join()
==>v[3]
gremlin> promise.isDone()
==>true
gremlin> g.V().out().promise{it.toList()}.thenApply{it.size()}.get()
==>6
```

## Important

* JanusGraph can work with embedded gremlin server and it is able to connect to remote standalone gremlin servers
* Possible to use JanusGraph Embedded Gremlin with multiple graphs with multiple config files 
* It is strongly encouraged to explicitly define all schema elements and to disable automatic schema creation by setting `schema.default=none` in the JanusGraph graph configuration.
* query.force-index=false/true. Whether JanusGraph should throw an exception if a graph query cannot be answered using an index. Doing solimits the functionality of JanusGraph’s graph queries but ensures that slow graph queries are avoided on large graphs. Recommended for production use of JanusGraph.
* Enabling the `storage.batch-loading` configuration option will have the biggest positive impact on bulk loading times for most applications. Enabling batch loading disables Janus internal consistency checks in a number of places. Most importantly, it disables locking. In other words, Titan assumes that the data to be loaded into Titan is consistent with the graph and hence disables its own checks in the interest of performance. **Important**: Enabling `storage.batch-loading` requires the user to ensure that the loaded data is internally consistent and consistent with any data already in the graph. In particular, concurrent type creation can lead to severe data integrity issues when batch loading is enabled. Hence, we **strongly** encourage disabling automatic type creation by setting `schema.default = none` in the graph configuration. Batch loading disabling locks.
* PermamentLockExceptions will appear only on properties marked as ConsistencyModifier.LOCK
* Without graph.commit\(\) you can get cached result if handled in same thread
* Transactions are started automatically with the first operation executed against the graph. One does NOT have to start a transaction manually. The method `newTransaction` is used to start [multi-threaded transactions](http://docs.janusgraph.org/latest/tx.html#multi-thread-tx) only
* fold/unfold get or create upsert [https://stackoverflow.com/a/46053115/7120456](https://stackoverflow.com/a/46053115/7120456)
* When updating an element that is guarded by a uniqueness constraint, JanusGraph uses the following protocol at the end of a transaction when calling `tx.commit()`:
  1. Acquire a lock on all elements that have a consistency constraint
  2. Re-read those elements from the storage backend and verify that they match the state of the element in the current transaction prior to modification. If not, the element was concurrently modified and a PermanentLocking exception is thrown.
  3. Persist the state of the transaction against the storage backend.
  4. Release all locks.

## Bulk/Batch loading

[https://docs.janusgraph.org/latest/bulk-loading.html](https://docs.janusgraph.org/latest/bulk-loading.html)

[https://docs.janusgraph.org/latest/limitations.html\#\_batch\_loading\_speed](https://docs.janusgraph.org/latest/limitations.html#_batch_loading_speed)

**Important**: Enabling `storage.batch-loading` requires the user to ensure that the loaded data is internally consistent and consistent with any data already in the graph. In particular, concurrent type creation can lead to severe data integrity issues when batch loading is enabled. 

![](https://ci5.googleusercontent.com/proxy/0azkNkJhdmb9aqFL-ogPjJgjohioyXX-cb7G3LrjyGA342U1bzefk2TGfMSFsrLVtL0DJBiknHLdLwyhlz1mLfLAR1iSeQ2OhYWBw-XEMWQmVm1yUxyCeKhM_eYJw_P31O6qyam1SchGVv-udHPYt7YbyuveKEBFH5bbXDw6jqdk=s0-d-e1-ft#https://image.slidesharecdn.com/powersoftenredux1-180127202647/95/powers-of-ten-redux-25-638.jpg?cb=1517084949)

![](https://ci4.googleusercontent.com/proxy/OYlJi5ry2vJew2BfIEsT97JHPLhuuzWJmWgjgDGRJawggFOHAFHZTuwQOVf7sotpeRgeRwkv59IeB2thuZufSyx-ufrP1Jlx_7nK4-mOlxYMU3KJqMPladlD7Ax_3QTQR8vsk5PJn4fWiPG61dwK5eyRCke1f3DrD6WlIkVk3zqFruepsByE2oQ5Zht0sZFL8DplxD8Xg9D4JGySERhmA8WmDGZpoRISjLXzhhoCWuHojrvTh8hc1XWymgvl=s0-d-e1-ft#https://bitgamelabs.atlassian.net/wiki/download/thumbnails/645988413/image2018-6-23_8-58-38.png?version=1&modificationDate=1529737121488&cacheVersion=1&api=v2&height=250)

[https://github.com/IBM/janusgraph-utils/blob/master/doc/users\_guide.md\#import-csv-file-to-janusgraph](https://github.com/IBM/janusgraph-utils/blob/master/doc/users_guide.md#import-csv-file-to-janusgraph)

[https://docs.datastax.com/en/dse/6.0/dse-dev/datastax\_enterprise/graph/dgl/dglOverview.html](https://docs.datastax.com/en/dse/6.0/dse-dev/datastax_enterprise/graph/dgl/dglOverview.html)

**Batching** - Looking at our script, you’ll notice that I’m including more than one addV per call. The exact number you’ll want to send over at once may vary, but the basic idea holds that there are performance benefits to be gained from batching. In addition to batching, note that I chained all of the mutations into a single traversal. This amortizes the cost of traversal compilation, which can be non-trivial when you’re going for as high of throughput as possible. Note that Gremlin is quite powerful and you can mix reads and writes into the same traversal, extending way beyond my simple insert example. So keep that in mind as you write your mutating traversals. The chosen batch size 10 is rather arbitrary so plan to test a few different sizes when you’re doing performance tuning.

[https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance](https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance)

_"Florian Hockmann lis 14 2017 09:27_  
_`@alimuzaffarkhan I would try it without any locks as they can slow down parallel inserts a lot. That's why it's often a good idea to handle de-duplication in your client application or at least make it robust against duplicate data. See also Chapter 29 of the docs for this topic. Even if you really need the locks, it might be interesting to benchmark performance without locks as that will tell whether locks are responsible for the low performance or whether there's another issue.`_

_Thijs lis 14 2017 10:19_  
_`@alimuzaffarkhan I have also struggled with the performance due to unique constraints which caused a lot of locking. After a while I removed all constraints and build a de-duplication mechanism to merge duplicate nodes (when detected) and now I can insert thousands of vertices and edges a second. I build a linked data platform and hence when I query for some URI I perform a dedup-action if multiple nodes are found. I use additional timestamp properties and some other arbitrary rules to determine which elements to keep. This way I can have a reliable eventual consistent linked data platform.My setup: 1 cassandra node (non-unique-indexes on my URI-identifiers), 1 es node (indexes on all properties), 1 kafka node, zookeeper, scala-data-listeners importing data from multiple sources and pushing it to Kafka, scala-graph-importer listening to Kafka and importing incoming records to the graph. I stream the Kafka-topics in batches of 100 and am also commiting to the graph by batch (committing single records is slow). I also stream the batches concurrently and this is where a little optimization/tuning can be done, I currently have set the parallelism to 30 (so processing 30x100 records/sec, where a record results in committing one or more vertices and zero or more edges).Currently I am running this on a single machine.So my dedup-mechanism is ad-hoc executed but you could also scan for duplicate id's after a certain delay since the moment a new id was inserted last (perhaps do this in batches)."`_

## Standalone Gremlin Server

"I generally wouldn't recommend embedding Janus in your app though unless you have a really good reason to." - by Ted Wilmes [https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance](https://www.experoinc.com/post/janusgraph-nuts-and-bolts-part-1-write-performance) 

[https://github.com/JanusGraph/janusgraph/issues/1108](https://github.com/JanusGraph/janusgraph/issues/1108)

"By default, communication with Gremlin Server occurs over WebSockets and exposes a custom sub-protocol for interacting with the server."  
[http://tinkerpop.apache.org/docs/3.2.3/reference/\#starting-gremlin-server](http://tinkerpop.apache.org/docs/3.2.3/reference/#starting-gremlin-server)  
[http://tinkerpop.apache.org/docs/3.2.3/reference/\#connecting-via-console](http://tinkerpop.apache.org/docs/3.2.3/reference/#connecting-via-console)  
[http://tinkerpop.apache.org/docs/3.2.3/reference/\#\_connecting\_via\_rest](http://tinkerpop.apache.org/docs/3.2.3/reference/#_connecting_via_rest)  
[http://docs.janusgraph.org/0.2.0/server.html\#\_websocket\_versus\_http](http://docs.janusgraph.org/0.2.0/server.html#_websocket_versus_http)  
[http://docs.janusgraph.org/0.2.0/server.html\#\_janusgraph\_server\_as\_a\_websocket\_endpoint](http://docs.janusgraph.org/0.2.0/server.html#_janusgraph_server_as_a_websocket_endpoint)  
[http://docs.janusgraph.org/0.2.0/server.html\#\_advanced\_janusgraph\_server\_configurations](http://docs.janusgraph.org/0.2.0/server.html#_advanced_janusgraph_server_configurations)

## Presentations about Janusgraph

* [https://www.slideshare.net/JasonPlurad/airline-reservations-and-routing-a-graph-use-case](https://www.slideshare.net/JasonPlurad/airline-reservations-and-routing-a-graph-use-case)
* [https://www.slideshare.net/ChinHuang4/onboarding-with-janusgraph-performance](https://www.slideshare.net/ChinHuang4/onboarding-with-janusgraph-performance)
* Airline reservations and routing: a graph use case [https://www.youtube.com/watch?v=zOq1FtnWDuE](https://www.youtube.com/watch?v=zOq1FtnWDuE) 
* JanusGraph Journey [https://www.youtube.com/watch?v=1TQcPWgPvF8](https://www.youtube.com/watch?v=1TQcPWgPvF8)
* Scylla Summit 2017: Performance Evaluation of Scylla as a Database Backend for JanusGraph [https://www.youtube.com/watch?v=YBsbXYvyZnA](https://www.youtube.com/watch?v=YBsbXYvyZnA)
* Ted Wilmes on the state of JanusGraph 2018 [https://www.youtube.com/watch?v=yLm0ruUGgng](https://www.youtube.com/watch?v=yLm0ruUGgng)
* [https://www.scylladb.com/2017/12/21/performance-evaluation-scylla-4-janusgraph/](https://www.scylladb.com/2017/12/21/performance-evaluation-scylla-4-janusgraph/)

