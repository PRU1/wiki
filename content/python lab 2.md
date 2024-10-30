# 1
## part a
```Python
# part a) nothing is outputted because there is no print statement

def my_sqrt(x):

sqr = x**0.5

return sqr

  

if __name__=="__main__":

res = my_sqrt(25)

print(res)
```
## part b
- produces an error because `sqr` is not defined
- to avoid error print out a variable value (i.e. `my_sqrt(34)`)
## part c
difference between `my_sqr` and `my_print_sqr`: `my_print_sqr` has no return value, so it cannot be treated like a variable, the way `my_sqr` can, i.e. running `print(my_print_sqr)` would return `None` or an error

`res = my_print_square(25) ; print(res)` returns `None`