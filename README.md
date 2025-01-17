# database-book
The guide for understanding databases from scracth, it helps learners to start with simple key value store, and takes all the way to epaxos kind of databases. It's 170+ slides pdf, so wait for complete loading. Slides [link]([url](https://docs.google.com/presentation/d/1UI3I-hWTgxi59jAFqAuJTIa_Ei7TolXpvpb7vMOzCvY/edit?usp=sharing))

### The jounery
Takes how can we build a system that supports SELECT, INSERT, UPDATE, DELETE statements from scratch. We start with simple key value store, and take step by step approach by adding more real world use cases/challenges.

### Journey to MySQL/Postgresql
* Simple in memory key value store
* Understanding disk storage types -> B+tree and LSM
* Add durability (with single thread)
* Add multiple threads support (Transactions)
* Understanding Transactions, LOCKs, implemenation
* Postgresql vs MySQL data structures and operations

### Journey to Scale reads and writes
* Add fault tolerance
* Scale writes -> Aurora/AlloyDB
* Solve split brain challenge
* Improve availability of simple writer systems
* Imporve IO & network performance - Aurora/AlloyDB
* Cloud provider internal architecture of database deployments for scale.
* Scaling reads -> Facebook memcache architecture
* Scaling read/writes -> Vitees, Cassandra architecture
* Improving garbage collection and operating system constructs for database - ScyallDB
* Solving conflicts in data -> DynamoDB vector clocks
* Scale single row read/writes --> Conflict free replicated data types (CRDT)

### Journey to consistent distributed systems with scale
* Selecting leader -> Paxos
* Building consistent storage systems -> Spanner
* Spanner truetime advantage in reads
* Spanner transactions support -> 2-phase commit
* Locks in spanner
* Limitations of spanner 2-phase commit
* Limitations of spanner writes and roundtrips
* Storage layer optimisations -> Interval tables and Ressi format
* Simplify paxos -> Raft

### Improving performance with custom hardware
* Remote direct memory access (RDMA) machines advantages
* Example database - FaRMDB

### Coming soon
* Avoid single writer with consistency -> E paxos
