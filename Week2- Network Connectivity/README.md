# 2. Network Connectivity 

### Triadic Closure

The tendency for people who share connections in a social network to become connected themselves. 

### Clustering Coefficient: Measuring Triadic Closure in Network

Measures the degree to which nodes in a network tend to cluster or form triangles. 

-	<b>Local clustering coefficient</b> of a node is the fraction of pairs of the node’s friends that are friends with each other. 

``` 
Clustering coefficient of node X = (# of pairs of X’s friends who are friends) / (# of pairs of X’s friends)
```

-	<b>Global clustering coefficient </b>

Approach 1: Average local clustering coefficient over all nodes in graph.

Approach 2: Measure number of open triads that are triangles in a network. Each triangle has 3 open triads. 

``` 
Transitivity = (3 * Number of closed triads) / (Number of open triads) 
```

### Transitivity VS. Average Clustering Coefficient

Both measure the tendency for edges to form triangles. 
Transitivity weights nodes with larger degree higher. 

<b>Distance Measures </b>

Measuring distance from one node to all other nodes:
-	Breadth First Search 
-	Depth First Search 

Measuring distance between all nodes of a graph:

-	Average Distance (between all pairs of nodes)
-	Diameter (maximum distance between a pair of nodes)
-	Eccentricity (of a node is the largest distance from that node to any other node in the network)
-	Radius (of a graph is the minimum eccentricity)
-	Periphery (of a graph is set of nodes with eccentricity = diameter) 
-	Center (of graph is set of nodes with eccentricity = radius)

### Connectivity

1. An <i>undirected graph</i> is connected if, for every pair of nodes, there is a path between them. 

   <b>Connected components</b> Subset of nodes where every node in subset has path to every other node, and no other node has a path to any node in the subset. 

2. A <i>directed graph</i> is strongly connected if, for every pair nodes u and v, there is a directed path from u to v and a directed path from v to u. 

3. A <i>directed graph</i> is weakly connected if replacing all directed edges with undirected edges produces a connected undirected graph. 

    <b>Strongly connected components </b> Every node in the subset has a directed path to every other node, and no node has a directed path to and from every node in the subset. 

    <b>Weakly connected components </b>

### Network Robustness 

Ability of a network to maintain its connectivity when it faces failures or attacks. 

<i>Types of attacks:</i> removal of nodes or edges. 

<i>Structural properties:</i> connectivity. 

<i>Examples:</i> airport closures, internet router failures, power lines failures. 

-	<b>Node connectivity:</b> minimum number of nodes needed to disconnect a graph
-	<b>Edge connectivity:</b> minimum number of edges needed to disconnect a graph 

Graphs with large edge and node connectivity are more robust. Higher number of minimum node or edge cuts required for network disconnectivity is desirable.  
