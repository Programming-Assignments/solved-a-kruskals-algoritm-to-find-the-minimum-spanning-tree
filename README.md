Download Link: https://assignmentchef.com/product/solved-a-kruskals-algoritm-to-find-the-minimum-spanning-tree
<br>
A Kruskal’s algoritm to find the minimum spanning tree

The idea behind Prim’s algorithm is simple, a spanning tree means all vertices must be connected. So the two disjoint subsets (discussed above) of vertices must be connected to make a Spanning Tree. And they must be connected with the minimum weight edge to make it a Minimum Spanning Tree.

Algorithm1) Create a set mstSet that keeps track of vertices already included in MST.2) Assign a key value to all vertices in the input graph. Initialize all key values as INFINITE. Assign key value as 0 for the first vertex so that it is picked first.3) While mstSet doesn’t include all vertices….a) Pick a vertex u which is not there in mstSet and has minimum key value.….b) Include u to mstSet.….c) Update key value of all adjacent vertices of u. To update the key values, iterate through all adjacent vertices. For every adjacent vertex v, if weight of edge u-v is less than the previous key value of v, update the key value as weight of u-v

The idea of using key values is to pick the minimum weight edge from cut. The key values are used only for vertices which are not yet included in MST, the key value for these vertices indicate the minimum weight edges connecting them to the set of vertices included in MST.