used in [[AM-GM Inequality]] proof

also known as Cauchy induction

--> show that some condition is true for values larger than $n$ and that the same condition is true for values smaller than $n$

1. first prove a statement is true for a base case (using [[proof by induction|standard induction]]
2. show that $P(k)\Rightarrow P(2k)$ --> forward step
3. show that $P(k) \Rightarrow P(k-1)$ --> backwards step

this argument works because you show that it is true for any larger value, but also any value inbetween (because it works in the smaller step of $k-1$)