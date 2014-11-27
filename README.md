Distributed_System
==================
###Python, Big data, ZooKeeper, MapReduce, Dynamo
_________
1. In project 1, these are the Bully Algorithm and the Invitation Algorithm implemented by Python, which using ZeroRPC to comunicate with other servers.

2. In project 2, 

> -Part 1: Leader Election

    I Use Kazoo and ZooKeeper, implement leader election, which follow the technique described in the Leader Election section of http://zookeeper.apache.org/doc/trunk/recipes.html.



> -Part 2: A Reliable Distributed Key-Value Store

    I implement a reliable key-value store based on ZooKeeper.  This storage system has at least 3 storage servers with all the data replicated on all servers.  Reads and writes all go through a elected storage leader.In this project, clients only need to know about the ZooKeeper server addresses.

    A put operation does succeed unless the value is stored at all of the live storage nodes.  A StoreException IS raised if the put operation fails or times out.
