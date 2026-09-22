<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Neither [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) nor fast convergence follows from [detailed balance](../../../../../detailed-balance.md).** On two states, the identity [transition matrix](../../../../../stochastic-matrix.md) satisfies [detailed balance](../../../../../detailed-balance.md) for the uniform [probability distribution](../../../../../probability-distribution-split.md), but neither state can reach the other.

Even after imposing [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) and [aperiodicity](../../../../../aperiodic-markov-chain.md), consider

$$
P_\varepsilon=\begin{pmatrix}1-\varepsilon&\varepsilon\\\varepsilon&1-\varepsilon\end{pmatrix},\qquad 0<\varepsilon<\tfrac12.
$$

It satisfies [detailed balance](../../../../../detailed-balance.md) for $\pi=(1/2,1/2)$. Its nontrivial [eigenvalue](../../../../../eigenvalue.md) is $1-2\varepsilon$, and, from state zero, its [total variation distance](../../../../../total-variation-distance.md) from $\pi$ after $n$ steps is $\tfrac12(1-2\varepsilon)^n$. This approaches zero arbitrarily slowly as $\varepsilon$ decreases. [Detailed balance without rapid convergence](../../../../../detailed-balance-without-rapid-convergence.md) separates correctness of a [stationary distribution](../../../../../stationary-distribution.md) from reachability and speed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
