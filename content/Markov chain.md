# Introduction
You're in state A, and you can transition to state B.
There is some probability of you transitioning to state B.
In a Markov chain, the probability of transitioning to state B depends only on your current state and (time elapsed??). 
![[state space]]


# More details:
- stochastic process (not deterministic, you can only find a probability of something ocurring)
- "memory-less": next state only depends on current state


**time homogenous Markov chains**  --> probability of any state transition does not depend on time. You'll see this visualized in directed graphs
![[Pasted image 20240314212022.png]] image source: [Markov Chains | Brilliant Math & Science Wiki](https://brilliant.org/wiki/markov-chains/)

**The Markov Property** *a definition*
For any positive integer $n$ and possible states $i_{0,}i1,...,i_n$ of the random variables,
$$P(X_n=i_{n}\mid X_{n-1}=i_{n-1})=P(X_n=i_{n}\mid X_0=i_{0,}X_1=i_{1,...,}X_{n-1}=i_{n-1})$$
--> this says the previous state is all you need to know to determine the probability distribution of the current state. 

## Transition Matrices
- has information on probability of transitioning between states (sort of like an adjacency matrix)
- For some state space $S$, the ($i,j)^{th}$ element in a probability matrix $P_{t}$ is given by:
$$ (P_t)_{i,j}=\mathbb{P}(X_{t+1}=j \mid X_{t}=i)$$
this means that each row of the matrix is a probability vector. The sum of all values in the matrix is 1