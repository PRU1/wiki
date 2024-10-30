A proof is a set of statements that are derived from a set of statements agreed to be true (called [[axioms]]). 
# Implications
if one statement is shown to be true, then another one must be true.
Suppose $n>3$ is statement $P$ and $n>0$ is statement Q. We can say $P\implies Q$. $P$ is called the **hypothesis** or **antecedent**; $Q$ is called the **conclusion** or **consequent**. 

Consider $P \implies Q$, then the converse is $Q \implies P$. If both the statement and its converse are true, then the two statements are equivalent: $P\Leftrightarrow Q$.

## proof by cases
it's hard to consider all the different cases at once. So you split your proof into cases, and show that a statement is true for all the cases
## proof using implication
*Prove that 101 is even*
___
An integer $n$ is even if $2$ divides into it.
This means that $n = 2k$, where $k$ is some integer. Since $k$ is an integer, $k \leq 50$ or $k \geq 51$, which means

$k\leq 50$ $\implies$ $2k \leq 100$[^1]
$k \geq 51$ $\implies$ $2k \geq 102$, and $2k \neq 101$.

Hence $101$ is not even

[^1]: you can replace the implies symbol with "if... then" statements 
___
# Types of Proof
[[proof by induction]]
[[proof by infinite descent]]