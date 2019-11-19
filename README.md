# Implementing Graph Traversal Builder in Java
This project demonstrates how to [implement](src/main/java/com/datastax/examples/builder/shortestPath/ShortestPathQueryBuilder.java) and
[use](src/main/java/com/datastax/examples/builder/ShortestPathTraversals.java) a traversal builder that can significantly simplify
the construction of complex traversals.

Contributor(s): [Daniel Kuppitz](https://github.com/dkuppitz)

## Objectives

* Demonstrate how to use the builder pattern to simplify the construction of complex Gremlin traversals
  
## Project Layout

* [ShortestPathQueryBuild.java](/src/main/java/com/datastax/examples/builder/shortestPath/ShortestPathQueryBuilder.java) - This file implements the builder pattern logic for simplifying traversal construction

## How this Works
The graph being used in this project is based on [TinkerPop's modern graph](http://tinkerpop.apache.org/docs/current/reference/#tinkerpop-modern).
The only difference is an added `uses` edge between `peter` and `ripple`.

The application can run without a connection to a DataStax Enterprise (DSE) cluster (in that case, it will execute all traversals on a `TinkerGraph`). The application's
user interface will show all the available commands that can be used to establish a connection to a DSE cluster and build/execute certain
traversals (note, that there's also support for tab completion).

## Setup and Running

### Prerequisites
* Java 8
* DSE Cluster with Graph enabled or TinkerGraph

### Running
To start the sample application, which is a simple CLI application, run the following command from the application's root directory:

```bash
bin/run.sh
```

This shell script will start the application, or recompile  and start the application if any source file is newer than the current binary file.



