[[Neat C++ tips]][[Competitive Programming]]

# reference
tells you the location of a variable in memory. `&`
```C++
int x = 59;
auto y = &x;
```
# dereference operators
takes a location (of a variable in memory) and print out the value in that location. `*`
```C++
int x = 59;
auto y = &x;
auto z = *y; // prints out 59
```

