# archelon
A distributed key-value store for academic purpose. The high level goal is to study and implement various concepts from distributed systems. These include but are not limited to:

1. An atomic broadcast layer: this shall be implemented using Raft or ZAB or paxos. The layer shall be pluggable and provide appropriate
   APIs for higher layers.
2. A failure detector: many algorithms exist. The one by Chandra et al is a good candidate to start with.
3. Leader election: Any of the existing algorithms can be used. Good candidates are; failure detector by Chandra et al, sequencer by
   Defago et al.
4. Write Ahead Logging (WAL) for crash recovery mechanism. A paper on ARIES is a must read.
5. Sharding techniques in data-base.

Basic plumbing blocks:
1. gRPC and protocol buffers (Google).
2. in-memory key-value store using B-Tree (code from Google).
3. A multi-threaded server.
4. Google C++ testing framework.

References:
1. "Writing a Database: Learning By Doing", by Daniel Chia.
2. MIT 6.824: Distributed Systems (2016 version).

