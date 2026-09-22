<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

An [average-reward optimal policy](../../../../../average-reward-optimal-policy.md) maximizes the limiting expected reward per epoch, $\liminf_{n\to\infty}n^{-1}\mathbb E\sum_{t=1}^nr_t$, from each initial state. Here the state is the score modulo three. Under the coin policy the state moves to itself or its successor with probability one half. Its unique [stationary distribution](../../../../../stationary-distribution.md) is uniform, so the reward for reaching state zero has average **$g=1/3$ per toss**.

The reward vector for that policy is $(1/2,0,1/2)$. Solving its [Poisson equations](../../../../../poisson-equation.md) $g+h_i=r_i+\frac12h_i+\frac12h_{i+1}$, with cyclic indices and $h_0=0$, gives $h=(0,-1/3,1/3)$. Telescoping the equations gives $F_s(i)=s/3+h_i-\mathbb E_i h(X_s)$. The chain is irreducible and aperiodic, so its last [expectation](../../../../../expected-value.md) converges to its stationary mean, independent of the starting state. Therefore

$$
\boxed{\lim_{s\to\infty}[F_s(x)-F_s(0)]=\begin{cases}0,&x\equiv0,\\-1/3,&x\equiv1,\\1/3,&x\equiv2\pmod3.\end{cases}}
$$

For policy improvement, a die gives a uniform next residue, so its reward-plus-old-bias value is $1/3+(h_0+h_1+h_2)/3=1/3$. Coin values are $g+h_i=(1/3,0,2/3)$. Switch to the die at residue one and retain the coin at the others. The new [stationary distribution](../../../../../stationary-distribution.md) is $(4/9,1/3,2/9)$ and its average reward is $4/9$, strictly better.

This improved policy is already optimal. Its bias is $h=(0,-1/9,1/9)$ and $g=4/9$. Die values are again $1/3$, whereas coin values are $(4/9,0,5/9)$. They satisfy the [average-reward Bellman equation](../../../../../average-reward-bellman-equation.md) $g+h_i=\max_a\{r_i(a)+\mathbb E_a h(X_{t+1})\}$. Summing the Bellman inequalities under any policy bounds its expected total reward by $ng$ plus a bounded bias difference; the proposed policy achieves equality. Hence

$$
\boxed{\text{use the die at residue }1\text{ and the coin at residues }0,2;\quad g_*=4/9.}
$$

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
