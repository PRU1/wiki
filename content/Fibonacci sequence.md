Consider the fibonacci sequence:

`1,1,2,3,5,8,13,21,34,55`

To find the $n$th term in a fibonacci sequence, we can write it as:

$t_n = t_{n-1}+t_{n-2}$ ... the $n$th term is the sum of the two previous terms.

Note that this general formula only works in $n \geq 3$. Because if $n = 2$
$t_2 = t_1 + t_0$ and $t_1 = t_0 + t_{-1}$. $t_0$ and $t_{-1}$ are not defined.

Since we know $t_1$ and $t_2$ are both 1, we can define our recursive function as such:

$$ t_n = \begin{cases} t_{n-1}+t_{n-2} &\text{if $n \geq 3$} \\ 1 & n=1 \text{ or } n=2 \end{cases}$$
Putting that into C++ gives us the following program

```
int fib(int n) {
	if (n >= 3) {
		return fib(n - 1) + fib(n - 2); // return sum of two previous terms
	}
	else { // if n = 1 or n = 2
		return 1;
	}
}
```

Fun fact: the condition where a recursive function doesn't call itself is called the base case. The other condition is call the recursive case