# 1. Introduction to Networks

A Network (or Graph) is a set of objects (nodes/vertices) with interconnections (edges/links/ties).

Applications of Networks:
* Social Networks
* Transportation and Mobility Networks 
* Information Networks 
* Biological Networks
* Financial Networks
* Trade Networks
* And more…

Many complex structures can be modeled by networks. Can understand a phenomenon better by studying its structural representation as a network.
Networks may be observed to detect subdomain clusters, influential nodes, connectivity between nodes. 

<b>Undirected (Bi-directional) graphs:</b> Symmetric relationships between nodes. 

<b>Directed (Uni-directional) graphs:</b> Asymmetric relationships between nodes.

<b>Weighted Networks:</b> Graph edges carry unequal weights, where the weight represents some meaning in the relationship between the nodes. 

<b>Signed Network:</b> Networks can carry information about friendship and antagonism based on conflict or disagreement - graph edges are assigned positive or negative signs.

<b>Multigraph:</b> A pair of nodes can have different types of relationships simultaneously. Network where multiple edges can connect the same nodes (parallel edges).

<b>Bipartite graphs:</b> A graph whose nodes can be split into two sets {L} and {R} and every edge connects a node in {L} with a node in {R}. Example- Sports fans {L} and basketball teams {R}.

** Bipartite graph cannot contain a cycle of an odd number of nodes. 

<b>Projection Graphs</b>
-	L- Bipartite graph projection: Network of nodes in group {L}, where a pair of nodes is connected if they have a common neighbor {R} in the bipartite graph.
Application example: Viral Marketing – if 2 people like the same team, they might like the same product.
-	Similar definition for R-Bipartite graph projection (Teams connected if they have at least 1 sports fan node in common).

<b>Weighted Projection Graphs</b>
Weights of edges are proportional to number of common neighbors between nodes.
-	Weighted L- Bipartite graph projection
-	Weighted R- Bipartite graph projection

