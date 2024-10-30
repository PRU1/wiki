# Resources

- [https://cses.fi/book/index.php](https://cses.fi/book/index.php) → By Antti Laaksonen
- [https://cdn.discordapp.com/attachments/773688766543560754/812510600164933649/Steven_Halim_-_Competitive_Programming_3__The_New_Lower_Bound_of_Programming_Contests_2013.pdf](https://cdn.discordapp.com/attachments/773688766543560754/812510600164933649/Steven_Halim_-_Competitive_Programming_3__The_New_Lower_Bound_of_Programming_Contests_2013.pdf) → Good book
- C++ cheat sheet:

https://github.com/mortennobel/cpp-cheatsheet

- [Set Theory for Programmers | Skerritt.blog](https://skerritt.blog/sets/) → Good summary of set theory

# Tips - C++

1. FASTER input and output

```C++
ios::sync_with_stdio(0);
cin.tie(0);
```

1. Don’t use `<< endl` for line breaks, use `"\n"` ; it’s faster
2. Don’t do this:

```C++
int a = 123456789;
long long b = a*a;
cout << b << "\n"; // -1757895751 
// Code copied from Competitive Programmer's Handbook by Antti Laaksonen
```

Instead change `int a` to `long long` or do:

```C++
long long b = (long long)a*a;
```

1. Write your program faster by using `typedef`

```C++
typedef long long ll // Whenever you use ll in the program, it refers to long long

ll a = 5034059340; // Means long long a = 5034059340;
```

1. Convert `int` to `string` and vice versa

```C++
// int to string
#include<string>
int x = 23984;
string yay = to_string(x);

// string to int
string testing = "2342"; // String should be a number
int yay = stoi(testing); // Convert to int
```

1. Convert a **number digit** `char` to `int`

```C++
char x = '8'; // a number digit
int y = x - 48; // The value 8 is now stored in y
```

# Tips - Data Structures (C++)

Source: images are screenshots from the book

Guide to Competitive Programming: Learning and Improving Algorithms Through Contests  
by Antti Laaksonen  

### Stacks

Last in, First out: LIFO (like a stack of plates)

![[images/Untitled.png|Untitled.png]]

### Queues

First in, First out FIFO (like an ice cream truck line up)

![[images/Untitled 1.png|Untitled 1.png]]

### Iterators

An iterator points to a value in a data structure. For example, if we have a vector, `v`,

![[images/Untitled 2.png|Untitled 2.png]]

Notice that `v.end()` points outside the last element in `v`

Use `*v.begin()` to print out the value an iterator points (change code `v.begin()` to an iterator name)

## Sets

### Intro

There are `set` and `unordered_set` that have the same operations. Note that all elements in sets are distinct. So inserting the same element again won’t change the set

*Use `\#include<iterator> #include<set>` or `#include<`

- `set` operations are in $O(\log n)$﻿
- `unordered_set` is based on a hash table, operations are on average $O(1)$﻿ time

![[images/Untitled 3.png|Untitled 3.png]]

### Accessing elements in a set

Use the function `find(x)` NOT `set_name[]` to access values in a set. Note `find(x)` returns an iterator that points to the element `x` .

```C++
// check if element exists in a set
set<int> yay = {1,2,3,4};
auto it = yay.find(x);
if (it == yay.end(){
// x does not exist in the set yay
}
```

## Maps

A map is a pair: a key and it’s corresponding value (analogy: a key unlocks a unique door, and a door can represent a value)

You can think an array as a key-value pair. The index of the array corresponds to a unique value. You can use

- `map` ”based an a balanced binary search tree and accessing elements takes $O(\log n)$﻿ time” (section 5.2.2 of Guide to Competitive Programming)
- `unordered_map` ”uses hashing and accessing elements takes $O(1)$﻿ time on average” (section 5.2.2 of Guide to Competitive Programming)
- Remember to include `#include<map>` or `#include<unordered_map>`

Here’s the syntax:

![[images/Untitled 4.png|Untitled 4.png]]

You can also initialize a map like this:

```C++
unordered_map<string,int> testing {
  {"testing", 5}, {"yellow", 6}, {"Hello", 2}
  };
// Note uniform initialization is used here
// Uniform initialization: initialize variables using {value} instead of = value
```

And check if a key exists using:

```C++
if (testing.count("somekey")) {
// The key exists
}
```

To list out keys and values, you can do this:

```C++
for (auto x : testing){
	cout << x.first << " " << x.second << "\n";
}
// x.first is the key
// x.second is the corresponding value
// note we use x.first NOT testing.first
```

Or in C++ 17 onwards, you can use this: (called structure bindings)

```C++
for(const auto& [key, value] : testing) {
  cout << key << ": " << value << "\n"; 
}
```

# Tips - Misc.

## Split array into 2

```C++
#include <iostream>
#include <vector>
using namespace std;

void print(vector<int> arr){
  for (auto x: arr){
    cout << x << " ";
  }
}
int main() {
  vector<int> test = {1,2,3,4,5};
  int mid = test.size()/2;
  vector<int> left(test.begin(), test.begin()+ mid);
  vector<int> right(test.begin()+mid, test.end());
  print(left);
  cout << "\n----------------\n";
  print(right);
  
}
```

## Arithmetic series

An arithmetic series is when the difference between any 2 consecutive terms is the same. For example, $\{1,2,3,4,5,6,7\}$﻿ and $ \{-5, -3, -1, 1, 3, 5, 7 … \} $﻿ are arithmetic series because they have a common difference between terms.

> [!important]  
> @import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')SnS_n Sn​﻿ represents the sum of a series with @import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')nnn﻿ terms@import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')aaa﻿ represents the first term in a series@import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')ddd﻿ represents the common difference in an arithmetic series@import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')rrr﻿ represents the ratio between any two terms in a geometric series@import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')tnt_ntn​﻿ represents @import url('https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.16.9/katex.min.css')nthn^{th}nth﻿ term in a series  

  

> Sum of arithmetic series: $S_n = \frac{n}{2} \cdot (a + a + (n-1)(d))$﻿ or $S_n=\frac{n}{2} \cdot (t_1+t_n)$﻿

> $t_n = a + (n-1)(d)$﻿

  

If you need to find the sum numbers like 1+2+3+4+5…., don’t use a `for` loop. Apply the formula or alternatively use the formula $\displaystyle\sum_{t=0}^{n}1+2+3+ ... +n = \frac{1}{2}\cdot (n)(n+1)$﻿

```C++
// Don't do this:
int sum{}; int n = 100;
for (int i = 0; i < n; ++i){
sum += i;
}
// Do this, it's faster
int sum{}; int n = 100;
sum = n*(n+1)/2
```

## Geometric series

To get the next term, you multiply by the same number each time. A geometric series is when the ratio between two consecutive terms is the same.

  

> Sum of a geometric series: $\displaystyle \frac{a(r^n-1)}{r-1} $﻿

> $t_n = ar^{(n-1)}$﻿

  

## Set theory

A set is a collection of objects (objects can be numbers, strings, etc.). For example, $X=\{1,2,3,4,5\}$﻿ is an example of a set. Note **sets are unordered and each object is distinct.**

  

- [ ] Add use in competitive programming

### Set operations

- **Intersection** $A \cap B$﻿: The elements two sets have in common. i.e. if $A=\{2,4,6,8\}$﻿ and $B=\{4,8\}$﻿, then $A \cap B = \{4,8\}$﻿
- **Union** $A \cup B$﻿: Combine elements of $A$﻿ and $B$﻿ into one set
- **Complement** $\bar{A}$﻿: Every element NOT in $A$﻿. Depends on a _universal set_, which tells every possible element that could be in a set. So if a universal set was $\{1,2,3,4,5,6,7,8,9,10\}$﻿ and $A = \{1,2,3\}$﻿, then $\bar{A}=\{4,5,6,7,8,9,10\}$﻿
- **Difference** $A \setminus B$﻿**:** Every element in $A$﻿ but not in $B$﻿, like $A$﻿ minus $B$﻿. See the following [image](https://www.math-only-math.com/difference-of-sets-using-Venn-diagram.html):

![[images/Untitled 5.png|Untitled 5.png]]

### Set notation

|   |   |
|---|---|
|**Symbol**|**Meaning**|
|$\|A\|$|The size of a set (the number of elements). Also called cardinality|
|$A \subset B$|$A$﻿ is a subset of $B$﻿: each element of A is also in B|
|$\emptyset$|Means set is empty|
|$4 \in \R$|4 is in the real number set|
|$4 \notin \R$|4 is NOT in the real number set|
|$\mathfrak{P}(A)$﻿ or $P(A)$|Refers to all subsets of a set (in this case, a set called $A$﻿). There are $2^{\|A\|}$﻿ subsets if you include the original set and an empty set as a subset|

## Recursive algorithms

- call a function inside a function
- add more later

## Backtracking

- start with an empty solution set
- Extend solution set at each step of your algorithm
- For example, consider finding all the ways to place 4 queens on a 4x4 chessboard, so that no queen can attack another queen.
- Begin by placing a queen on the first row. This tells you where you can place the next queen

![[images/Untitled 6.png|Untitled 6.png]]

- You get a partial solution; continue this until you find all the solutions
- Implementation (taken from Guide to Competitive Programming by Anti L)

```C++
void search(int y) { 
if (y == n) {
 count++; 
return;
}
for (int x=0;x<n; x++) {
 if (col[x] || diag1[x+y] || diag2[x-y+n-1]) continue; 
col[x] = diag1[x+y] = diag2[x-y+n-1] = 1;
 search(y+1); 
col[x] = diag1[x+y] = diag2[x-y+n-1] = 0;
}
}
```

$n$﻿ is size of board  
code assumes rows and columns are numbered from 0 to  
$n-1$﻿  
place a queen on row  
$y$﻿

`col`stores the columns containing a queen. `diag1` and `diag2` keep track of the diagonals (queen on next row cannot be on diagonal

## Bit operations

- `int` are stored as 32 bits in memory
- `&` operator is cool

![[images/Untitled 7.png|Untitled 7.png]]

- You can check if numbers are even/odd using this. `if x&1 = 0` the number is even, and `x&1=1` if x is odd (think of last digit in binary representation)
- There are other bit operations (i.e. XOR, or bit shifts) but I don’t think they’re relevant for CCC so I’m going to skip those.

## Time Complexity

- Time complexity estimates how long a program will take to execute for some given inputs
- Calculating time complexity is useful to find out whether your program will TLE without having to write the program. It helps you explore the fastest solutions
- “Asymptotic upper bound” is used with Big O notation
    - means the worst possible performance of your algorithm
    - Labelled as O(…), where … is some function

### Big O notation rules

- Single commands have time complexity of O(n)

i.e.

```C++
a++;
b--;
int c = a+b;
b = 5;
// this program runs in O(1) time complexity.
// In other words, there are no inputs so the computation 
// time is always the same when you run this program
```

- O(n): a loop! if a loop runs n times, it has time complexity of O(n)
- If you have a loop inside a loop, then your time complexity is O($n^2$﻿). This is because it takes $n^2$﻿ steps to execute the for loop.
- Similarly, for $i$﻿ nested loops iterating $n$﻿ times each, the time complexity is O($n^i$﻿)
- If you have a program of many steps i.e.:

```C++
for (int i = 0; i < n; ++i){
// do something
}
for (int i = 0; i < n; ++i){
// do something
}
for (int i = 0; i < n; ++i){
	for (int (i = 0; i < n; ++i){
		for (int i = 0; i < n; ++i) {
				// 3 nested loops
		}
	}
// do something
}
```

- The time complexity of the algorithm is the biggest one. So in the program above, the time complexity is O($n^3$﻿) since the step of the program that takes the longest is the triple-nested for loop
- Sometimes your time complexity depends on many variables. i.e. consider the nested loop below:

```C++
for (int i = 0; i < n; ++i){
	for (int j = 0; j < m; ++j){
		// do something
	}
}
```

- In this case, the time complexity is O(nm)

### Time complexity in recursive functions

- Depends on how many times recursive function is called
- … and time complexity of a single call

i.e.

```C++
void f(int n) {
	if (n == 1) return;
	f(n-1)
}
```

- A single call of the function `void f` is O(1). But you end up calling it recursively $n$﻿ times. So the time complexity is O(n)
- Here’s another example (a bit more difficult)

```C++
void g(int n) {
  if (n == 1) return;
	g(n-1);
	g(n-1);
}
```

- Each function call has time complexity of O(1).
- The first function call for some $n$﻿ puts $n-1$﻿ and $n-1$﻿ in the execution stack. Then, you have 4 ($n-2$﻿) in the execution stack. Then 8 ($n-3$﻿) in the executation stack, and so on.
- So we see that the time complexity is O($2^n$﻿)

### Common time complexities

[Big-O Algorithm Complexity Cheat Sheet (Know Thy Complexities!) @ericdrowell (bigocheatsheet.com)](https://www.bigocheatsheet.com/)

### Estimating time complexities

- Use this to decide what type of algorithm is appropriate to solve CCC problems. For Junior problems, brute force probably works for J1-J3 and maybe J4.

![[images/Untitled 8.png|Untitled 8.png]]

- $n \log n$﻿ is time complexity for sorting algorithms
    - or maybe a recursive function, of $n$﻿ function calls with each function call with a time complexity of $\log n$﻿

### Maximum Subarray Sum

- Suppose you have an array of $n$﻿ elements
- Find the maximum sum of consecutive elements (called subarray)
- You can do it brute force, by checking each combination.
- Or you can do it O(n)

## Sorting Algorithms

- Rearrange an array so all the elements are in increasing order

### Bubble sort

- Check two elements at a time. If they are out of order swap them. Repeat until array is sorted

```C++
#include<iostream>
#include<vector>
using namespace std;
int main() {
	vector<int> unsorted = { 1,23,4,9,10,10,230,30 };
	for (int i = 0; i < unsorted.size(); ++i) {
		for (int j = 0; j < unsorted.size() - 1; ++j) {
			if (unsorted[j] > unsorted[j + 1]) {
				swap(unsorted[j], unsorted[j + 1]);
			}
		}
	}
	for (auto x : unsorted) {
		cout << x << " "; 
	}
	return 0;
}
```

- Worst case scenario: you need to make n^2 swaps (i.e. the array is initially ordered greatest to least)
    - technically n(n-1)/2 but that’s O($n^2$﻿)

### Merge sort

- [Merge sort in 3 minutes - YouTube](https://www.youtube.com/watch?v=4VqmGXwpLqc)

![[images/Untitled 9.png|Untitled 9.png]]

- (video and image since I’m a bit lazy right now)
- Search article for algorithm
    - I tried to make a new, “improved” implementation of merge sort. Didn’t work, so for code for this algorithm check out progamiz or geekcode

## How you should probably sort

- you don’t have time to implement your own sorting algorithm.
- use `sort(arr.begin(), arr.end());`
- This sorts in O($n \log n$﻿). How it’s sorted depends on compiler, but probably quicksort or merge sort.
- Also useful for arrange characters in a string alphabetically
- And if you are using a `pair` data structure it sorts by first element

```C++
vector<pair<int,int>> yay = { {1,3}, {2,4}, {1,2} }
sort(yay.begin(), yay.end());
// order after sort: {1,2}, {1,3}, {2,4}
```

# DP

Consider this problem:

you have a set of coins, `coins` = $\{c_1,c_2,…c_k\}$﻿ and a target sum of money, $n$﻿. Find what arrangement of coins gets you to the some $n$﻿ and uses the least number of coins.

- Suppose `coins`= {1,2,5}. Then the greedy solution would take the biggest coin values first. i.e. 5 + 5 + 2 = 12
- But the greedy solution is not always the optimal solution
    - i.e. $n$﻿ = 6 and `coins` = {1,3,4}. Greed solution: 4 + 1 + 1. Optimal solution: 3 + 3
- My implementation of the greedy approach (not tested on any grader. It assumes you can make the target sum):

```C++
#include<iostream>
#include<string>
#include<vector>
#include<unordered_map>
#include<utility>
#include<algorithm>
#include<cmath>
using namespace std;
int main() {
	int coinCount{};
	coinCount = 3;
	vector<int> coins(5);
	coins = { 1,3,4 };
	int target{};
	target = 6;
	// sort coins array
	sort(coins.begin(), coins.end());
	int i = 1;
	while (i <= coinCount){
		if (coins[coinCount - i] <= target) {
			// for debugging
			cout << "before: " << target << " | After ";
			target -= coins[coinCount - i];
			cout << target << " | coin used is: ";
			cout << coins[coinCount - i] << endl;
		}
		else
			++i;
	}
	return 0;
}
```

- So greedy approach is not the best approach
- You could brute force it but that’s too slow for large inputs
- So there’s something called DP - dynamic programming - which you can use.

- Start off by framing it as a recursive problem
    - we frame the solution to the problem as a solution to smaller subproblems
- Coin problem recursive solution: have a function `solve(x)`, which outputs the minimum number of coins to hit the target sum
- Recursive solution:
    - pick a coin start off with. Then run `solve(x-c)` where $x$﻿ is the target sum, and $c$﻿ is the coin you selected

![[images/Untitled 10.png|Untitled 10.png]]

  

![[images/Untitled 11.png|Untitled 11.png]]

  

The recursive solution:

```C++
// preamble not included
// this code is not tested!! Writing it in Notion.
int inf = 10000;
vector<int> coins = {1,3,4};
int target = 6;
int solve( int x ) {
	int best = inf;
	// x = 0
	if (x == 0)
		return 0;
	// x < 0
	if (x < 0) // using else if should also work
		return inf;
	// cycle through each coin. Subproblem: solve(x-c), where c is the coin value
	for (auto c : coins) {
			best = min (best, solve(x-c)+1);
	}
	return best;
}

int main () {
	cout << solve (target);
return 0;
}
```

- The recursive solution is slow for big inputs!! Try `target = 1005`, does not load.
- There’s a lot of repeating computations in the step `best = min(best, solve(x-c)+1)`. What if we store the output of the recursive function the first time it runs, and have an if statement to check if we’ve calculated it before.
- Storing the result of prior recursive calls is called memoization
    - Here’s my solution to CCC 2000 S4, using memoization.

```C++
#include<iostream>
#include<string>
#include<vector>
#include<unordered_map>
#include<utility>
#include<algorithm>
#include<cmath>
using namespace std;
// dp solution :D

#define inf 10000
vector<int> strokes;
vector<bool> visited;
vector<int> visited_ans;

int Count(int target) {
	// target = 0
	int best = inf;
	if (target == 0)
		return 0;
	// target < 0
	else if (target < 0)
		return inf;
	if (visited[target]) {
		return visited_ans[target];
	}
// recursive call
	for (auto n : strokes) {
		best = min(best, Count(target - n) + 1);
	}
	visited[target] = true;
	visited_ans[target] = best;
	return best;
}
int main() {
	int distance;
	cin >> distance;
	int clubs;
	cin >> clubs;
	strokes = vector<int>(clubs, 0);
	visited = vector<bool>(distance+1, false);
	visited_ans = vector<int>(distance+1, 0);
	for (int i = 0; i < clubs; ++i) {
		cin >> strokes[i];
	}
	int temp = Count(distance);
	if (temp == inf)
		cout << "Roberta acknowledges defeat.";
	else
		cout << "Roberta wins in " << temp << " strokes.";
	return 0;
}
```

- Would be a bit more efficientif we removed the visited bool vector. Instead, an unvisited recursive call is a negative number by default, since there is no way the recursive function outpus a negative number.
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

## Graph traversal

DFS and BFS. Both searches go to every node in a graph. the difference is in the order each algorithm visits each node.


