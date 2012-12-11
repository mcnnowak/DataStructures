#The Algorithm
Breadth-first search describes a connected component of the graph G consisting of the edges and vertices it traverses or visits.
The algorithm can be described as follows:

##Steps:
1. Visit the first node to be searched.
2. Visit all unvisited adjacent nodes.
3. Visit the nodes adjacent to the previously visited nodes until there are no more unvisited nodes.

#Analysis
When implemented using linked lists, this algorithm will run in O(n) time where n is the number of nodes in the graph. 

Whem implemented using an adjacency matrix, this algorithm will run in O(n_^2) time.
