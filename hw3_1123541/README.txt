Question: 1
Given an undirected graph with V nodes and E edges, create and return an adjacency list of the graph. 0-based indexing is followed everywhere.
Examples: (Should not use the examples to submit your code. These examples are for your understanding)
Input:
V = 4, E = 5
edges = {{0, 1}, {0, 2}, {1, 2}, {1, 3}, {2, 3}}

Output: 
0: 1 2 
1: 0 2 3 
2: 0 1 3 
3: 1 2 
Explanation:
Node 0 is connected to 1 and 2.
Node 1 is connected to 0,2 and 3.
Node 2 is connected to 0, 1 and 3.
Node 3 is connected to 1 and 2.

 
Question: 2
Given a connected undirected graph represented by an adjacency list adj, which is a vector of vectors where each adj[i] represents the list of vertices connected to vertex i. Perform a Breadth First Traversal (BFS) starting from vertex 0, visiting vertices from left to right according to the adjacency list, and return a list containing the BFS traversal of the graph.
Note: Do traverse in the same order as they are in the adjacency list.
Examples: (Should not use the examples to submit your code. These examples are for your understanding)
Input: adj = {{1, 3}, {0, 2, 3}, {1, 4}, {0, 1, 4}, {2, 3}}

Output: [0, 1, 3, 2, 4]
Explanation: 
Starting from 0, the BFS traversal will follow these steps: 
Visit 0 → Output: 0 
Visit 2 (first neighbor of 0) → Output: 0, 1
Visit 3 (next neighbor of 0) → Output: 0, 1, 3
Visit 1 (next neighbor of 0) → Output: 0, 1, 3, 2
Visit 4 (neighbor of 2) → Final Output: 0, 1, 3, 2, 4



Question: 3
Given a connected undirected graph represented by an adjacency list adj, which is a vector of vectors where each adj[i] represents the list of vertices connected to vertex i. Perform a Depth First Traversal (DFS) starting from vertex 0, visiting vertices from left to right as per the adjacency list, and return a list containing the DFS traversal of the graph.
Note: Do traverse in the same order as they are in the adjacency list.
Examples: (Should not use the examples to submit your code. These examples are for your understanding)
Input: adj = {{1, 3}, {0, 2}, {1, 4}, {0, 4}, {2, 3}}

Output: [0, 1, 2, 4, 3]
Explanation: 
Starting from 0, the DFS traversal proceeds as follows: 
Visit 0 → Output: 0 
Visit 1 (the first neighbor of 0) → Output: 0, 1 
Visit 2 (the first neighbor of 1) → Output: 0, 1, 2 
Visit 3 (the first neighbor of 2) → Output: 0, 1, 2, 4 
Backtrack to 2 and visit 4 → Final Output: 0, 1, 2, 4, 3




Question: 4
Given a weighted, undirected, and connected graph with V vertices and E edges, your task is to find the sum of the weights of the edges in the Minimum Spanning Tree (MST) of the graph. The graph is represented by an adjacency list, where each element adj[i] is a vector containing vector of integers. Each vector represents an edge, with the first integer denoting the endpoint of the edge and the second integer denoting the weight of the edge.
Examples: (Should not use the examples to submit your code. These examples are for your understanding)
Input:
V = 4, E = 5
0 1 10
0 2 6
0 3 5
1 3 15
2 3 4

Output:
19