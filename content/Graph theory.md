[[Competitive Programming]]
# Graph theory

- useful to think of problems as a graph
## Terminology

- graph consists of nodes (also called vertices)
- nodes are connected by edges
- length of path is the number of edges in it
- so 1 → 3 → 4 → 6 has a length of 3
- cycle is when first and last node are the same
- components: the connected parts of a graph
- a tree is a connected graph that contains no cycles
- directed graph (you can only travel in the direction of the arrow, can’t go backwards)
- weighted graph: you assign each edge a weight (you can interpret this as edge lengths)
- adjacent nodes/neighbour nodes: an edge between them
- Degree of node: the number of neighbours a node has
- the sum of degrees in a graph is always $2m$﻿ where $m$﻿ is the number of edges (each edge connects two nodes)

- graph is _regular_ if each node has an equal number of edges coming out (i.e. every node has the same degree)
- (below: for directed graphs) indegrees and outdegrees
- directed graph: _indegree of a node_→ the number of edges that end at the node. _outdegree_ _of a node_ number is the # of edges that start at a node
- bipartite graph: you can colour nodes using only two colours and no two adjacent nodes have the same colour

**graph representations in algorithms**

- several ways to represent graphs in algorithms. choice of data structure depends on the size of the graph

### **adjacency list**

- each node is assigned list. adjacency list contains nodes connected to one particular node. for example if we had a node named _x_, the adjacency list of _x_ consists of all the nodes connected to _x_.
- how to store adjacency lists? In a vector of vector!

![[images/Untitled 12.png|Untitled 12.png]]

```C++
// in vector of arrays
vector<int> adj[N];
// vector<vector<int>> adj;
adj[1].push_back(2);
adj[2].push_back(3);
adj[3].push_back(4);
adj[4].push_back(1);
```

- for undirected graphs, push back each edge in both directions
- for weighted graphs, initialize an array of vector pairs

```C++
vector<pair<int,int>> adj[N];
// a node A contains a pair (B,W), where B is connected to A by an edge, and W is the weight of that edge
adj[1].push_back({2,5});
adj[2].push_back({3,7}); 
adj[2].push_back({4,6}); 
adj[3].push_back({4,5}); 
adj[4].push_back({1,2});
```

- why use adjacency lists? efficiently find nodes that we can move to from some given node. i.e.

```C++
for (auto u : adj[s]){
	// process node u
}
```

### adjacency matrix

- indicates what edges a graph contains
- declare an array `int adj[N][N];`
- if `adj[a][b] = 1` then exists an edge between nodes `a` and `b` . `adj[a][b] = 0` if there is no node between `a` and `b` .

![[images/Untitled 13.png|Untitled 13.png]]

- **disadvantage of adjacency matrix:** contains $n^2$﻿ elements. you cannot use it for large graphs

### edge lists

- contains all edges in a graph in some order.
- convenient when you only need to process all edges, you don’t need to find an edge that starts at a particular node.

```C++
vector<pair<int,int>> edges;
edges.push_back({2,5}); // edge between 2 and 5
edges.push_back({2,3}); // edge between node 2 and 3
```

weighted graph:

```C++
vector<tuple<int,int,int>>> edges
edges.push_back({2,3,45}); // edge between 2 and 3 with weight 45
edges.push_back({1,2,4});
```

# Graph traversal

DFS and BFS. Both searches go to every node in a graph. the difference is in the order each algorithm visits each node.

## DFS
- begin at a starting node
- go to all nodes that you can reach from the starting node using the edges of the graph
- keep track of all visited node so you only visit each node once
### implementation
- assuming graph is stored as an adjacency list: `vector<vector<int>> adj;
- have a visited array : `vector<int> visited;`

```C++
void dfs(int s) { // s is index
	if (visited[s] == true) return; // you have visited all 

}
```
### BFS
- more difficult to implement than DFS
- at each step you explore nodes that are the same distance away from a starting node (i.e. 1 away, then 2 away) so you explore in the breadth of the graph
- visits at the node of the same level before continuing
```C++
queue<int> q;
bool visited[N];
int distance[N]; // distance from starting node to all node of the graph
```

![[Pasted image 20240220235915.png]]

```C++
visited[x] = true;
distance[x] = 0;
q.push(x);
while (!q.empty()) {
int s = q.front(); q.pop(); 
// process node s
for (auto u : adj[s]) {
	if (visited[u]) continue;
	visited[u] = true;
	distance[u] = distance[s] + 1; // at each step you only explore one node more
	q.push(u);
	}
}
```



































