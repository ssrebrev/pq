# pq
Pragmatic queue is unbounded multi producer single consumer queue for Go. 

`pq.Writer` is safe for concurrent access while `pq.Reader` should be accessed from a single goroutine.

**pq** is fast with stable throughput. 
With single producer and single consumer it handles around 60 million `writer.Enqueue` & `reader.Dequeue` operations per second.
With up to a million producers the throughput is in the range 30-40M OPS.


