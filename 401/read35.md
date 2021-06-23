# Graphs
## Graphs
### A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges
### Graphs common terminology:
- Vertex
- Edge
- Neighbor
- Degree
## Directed vs Undirected
### An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction while in Directed Graph also called a Digraph is a graph where every edge is directed.
## Complete vs Connected vs Disconnected
### `Complete Graphs` is when all nodes are connected to all other nodes.
### `Connected Graph` is graph that has all of vertices/nodes have at least one edge.
### `Disconnected Graph` is a graph where some vertices may not have edges.
## Acyclic vs Cyclic
1. An acyclic graph is a directed graph without cycles. A cycle is when a node can be traversed through and potentially end up back at itself.
2. A Cyclic graph is a graph that has cycles. A cycle is defined as a path of a positive length that starts and ends at the same vertex.
## Graph Representation
- Adjacency Matrix:
    - An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix. Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.
- Adjacency List:
    - An adjacency list is the most common way to represent graphs. it is a collection of linked lists or array that lists all of the other vertices that are connected. it makes it easy to view if one vertices connects to another.
## Traversals
* Breadth First
* Depth First
## applications
- GPS and Mapping
- Driving Directions
- Social Networks
- Airline Traffic