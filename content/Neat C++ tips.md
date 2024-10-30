[[Competitive Programming]]

1. Maximum or minimum value of integer
```
#include<limits>
int imax = numeric_limits<int>::max();
int imin = numeric_limits<int>::min();
```

2. check if key exists in hashmap
```C++
if (my_map.count(x) == 0)
	// do something
```
3. initialize vector of vectors
```
vector<vector<int>> spiral(row, vector<int>(column,0));
```