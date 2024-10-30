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