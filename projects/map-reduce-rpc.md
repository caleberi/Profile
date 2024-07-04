---
description: 'REPO: https://github.com/caleberi/map_reduce_rpc'
---

# Map Reduce RPC

#### MapReduce Implementation in Go using RPC and Channels

The following implementation demonstrates the MapReduce algorithm in Go, using a single coordinator to orchestrate the processing of files by worker processes to produce a final output. This implementation is inspired by the MapReduce white paper and leverages RPC and channels for communication between the coordinator and workers.

**Components**

1. **Coordinator**: Manages the entire MapReduce process, assigns tasks to workers, and collects results.
2. **Worker**: Processes tasks assigned by the coordinator (either Map or Reduce tasks).

#### Explanation

* **Coordinator**:
  * Manages the list of files to be processed tracks the status of the map and reduces tasks.
  * Provides tasks to workers upon request and updates the task status upon receiving results.
  * Marks the entire job as done when all map and reduce tasks are completed.
* **Worker**:
  * Continuously requests tasks from the coordinator.
  * Processes the received tasks (either map or reduce) and reports the results back to the coordinator.

#### Running the Application

1. &#x20;Build plugins in plugin directories:

```
.sh
go build -buildmode=plugin ./plugin/wc.go

```

2. Start the coordinator:

```
.sh
go run mr_coordinator.go

```

3. Start the worker :

```
.sh
go run mr_worker.go

```
