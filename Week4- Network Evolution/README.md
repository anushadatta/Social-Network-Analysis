# 4. Network Evolution 

## Degree Distributions 
It is the probability distribution of the degrees over the entire network. For a directed graph, consider in-degrees or out-degrees of nodes.

### Power Law
A power law degree distribution is one that looks like a straight line when one a log-log scale.

<b>P(k) = Ck<sup>-α</sup>,</b> where α and C are constants

For these distributions, most nodes have very small degree and only few nodes have very large degree.

### Preferential Attachment Model (PAM)

This model produces networks with degree distributions similar to power-law, with smallest shortest paths but small clustering coefficient. 

* Start with two nodes connected by an edge.
* At each time step, add a new node with an edge connecting it to an existing node. 
* Choose the node to connect to at random with probability proportional to each node’s degree.
* The probability of connecting to a node u for degree k<sub>u</sub> is ( k<sub>u</sub>/ Σ<sub>j</sub>k<sub>j</sub> )

As the number of nodes increases, the degree distribution of the network under the PAM approaches the power law P(k) = Ck<sup>-3</sup> with constant C. 

## Small World Network Phenomena
* Milgram Small World Experiment (Median path length = 6)
* Microsoft Instant Messenger (Median path length = 7)
* Facebook Network (Median path length = 5.28 in 2008, 4.74 in 2011)

Real social networks tend to have high clustering coefficient and small average path length. 

### Small World Model
This model produces networks similar to real networks.

* Start with a ring lattice of n nodes, where each node is connected to its k nearest neighbors
* Consider each edge (u,v). With probability p ∈ [0,1], select a node w at random and rewire the edge (u,v) so it becomes (u,w)

<b>1. Regular Lattice (p = 0):</b> no edge is rewired

<b>2. Random Network (p = 1):</b> all edges are rewired 

<b>3. Small World Network (0 < p < 1):</b> some edges are required, network conserves some local structure but has randomness too

## Link Prediction

Given a network, predict the edges that will be formed in the future. (Applications: Social media recommendation algorithm)

<b>Measures for Link Prediction:</b>
1.	Number of Common Neighbors
2.	Jaccard Coefficient 
3.	Research Allocation Index
4.	Adamic-Adar Index
5.	Preferential Attachment Score
6.	Community Common Neighbors: Common Neighbor Soundarajan-Hopcroft score
7.	Community Resource Allocation: Resource Allocation Soundarajan-Hopcroft score

