![[Getting info from user screen in Python]]
[An Introduction to Caching in Python (aaronnotes.com)](https://aaronnotes.com/2023/04/caching-in-python/#:~:text=Caching%20is%20a%20powerful%20technique,and%20more%20efficient%20Python%20applications.)

CACHING : store frequently accessed data in memory. 

## Caching in Python - hashmap!
Slow version; repeat operation for every function call 
```Python
import time

def get_sum_slowly(a,b):
	time.sleep(2)
	return a +b
print(get_sum_slowly(1,2))
```
Memoized version (DP!!)
```Python
cache = {}

def get_sum_cached(a,b):
	if (a,b) in cache:
		return cache[(a,b)]
		
	result = get_sum_slowly(a,b)
	cache[(a,b)] = result
	return result

print(get_sum_cached(1,2)) # first time it runs, takes 2 seconds
print(get_sum_cached(1,2)) # second time it runs, returns value instantly
```

**COOL PYTHON WAY**
```Python
import time
import functools

@functools.cache
def  get_sum_cached(a,b):
	time.sleep(2) # mimic lengthy computation
	return a+b

print(get_sum_cached(1,2)) # first time it runs, takes 2 seconds
print(get_sum_cached(1,2)) # second time it runs, returns value instantly
```
- `@functools.cache` is something added to Python 3.9. Automatically caches results from a function (that's crazy!)

## Cache strategies
- if you cache all operations you will run out of memory. Got to set cache size and decide what to store in the cache
Main caching strategies
1. LRU (least recently used): most recently used are kept in cache
2. LFU: (least frequently used): not used often are removed
3. Random
4. FIFO (first in first ouh)
5. Time based: discard items based on expiration time.

for DEETS - use time based caching! 