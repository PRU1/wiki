source: [Introduction | CS324 (stanford-cs324.github.io)](https://stanford-cs324.github.io/winter2022/lectures/introduction/)
the classic definition: a **probability distribution over sequences of tokens.**

Let's say we have a vocabulary $\nu$, which is just a set of tokens $\{x_1,x_2,x_3,...x_{n}\in \}\hspace{4pt}\nu$ . We can assign probability distributions based on the combinations of the tokens, $p(x_1,x_2,x_3,...x_n)$. 

For example, say we had $\nu=\{\text{based, probability, the, combinations, distributions, on}\}$.

A sample probability distribution:
$p(\text{probability, distributions, based, on, the, combinations}) = 0.3$
$p(\text{on, distributions, the, probability, based, combinations}) = 0.03$
etc. 

this distribution has syntactic information (grammar must make sense)

