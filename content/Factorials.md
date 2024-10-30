Following this tutorial: [(1) Introduction to Recursion (Data Structures & Algorithms #6) - YouTube](https://www.youtube.com/watch?v=B0NtAFf4bvU&t=1s)

What is recursion: a function calls it self

## Factorials
Consider n!

We can say that n! = n $\times$ (n-1)!
There is a problem with this approach. Consider 0!
Using this definition, 0! = 0 $\times$ (-1)!, and (-1)! is not defined.

So we have to define n! as a piecewise function
![[Pasted image 20221229123445.png]]

Now that we have the n! function defined, we just have to translate that to our program.

There are two cases, so we can have an `if` and `else` statement in our function.

```
int fact(int n)
{
// assuming that n is 0 or a positive integer.
if (n>= 1)
	return n * fact(n-1)
else
	return 1
}
```