#The Algorithm
Depth-first search visits all vertices and edges that describe a connected component of a graph. The algorithm can be described as follows:

##Steps:
1. Visit the first node to be searched.
2. Visit an adjacent unvisited node.
3. If the current node has no unvisited nodes, backtrack until a node with adjacent unvisited nodes is found and go back to Step 2. If no unvisited nodes are found, you are done.

#Analysis
When implemented using linked lists, this algorithm will run in O(n) time where n is the number of nodes in the graph.

Whem implemented using an adjacency matrix, this algorithm will run in O(n_^2) time.

