<h1 id="27k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $q_i=-g_{ii}$ for the total rate of leaving $i$. The [jump chain](../../../../../../jump-chain.md) of a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) $X$ is the discrete-time chain $Y=(Y_n)$ recording the states occupied after successive jumps. Its [transition probabilities](../../../../../../transition-probability.md) are

$$
p_{ij}=\frac{g_{ij}}{q_i}\quad(j\ne i),
\qquad p_{ii}=0,
$$

whenever $q_i>0$.

The chain $X$ is [irreducible](../../../../../../irreducible-markov-chain.md) if every state can be reached from every other state with positive probability. A state $i$ is [recurrent](../../../../../../recurrent-state.md) if, after leaving $i$, the process returns to $i$ with probability one; an irreducible chain is recurrent when one, and hence every, state is recurrent.

The [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) and its [jump chain](../../../../../../jump-chain.md) have exactly the same successive states. If $Y$ is transient, it visits each state only finitely often, so $X$ is transient. If $Y$ is recurrent, it visits a fixed state $i$ infinitely often. At those visits, $X$ has independent [exponential](../../../../../../exponential-distribution.md) holding times of rate $q_i<\infty$. Their sum diverges almost surely, so explosion cannot occur before all those returns. Hence $X$ returns to $i$ infinitely often and is recurrent. Thus, for an irreducible chain,

$$
\boxed{X\text{ is recurrent}\iff Y\text{ is recurrent}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
