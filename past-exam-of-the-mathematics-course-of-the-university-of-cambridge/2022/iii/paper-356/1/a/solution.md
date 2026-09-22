<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $w_{ij}$ be the transition rate from $i$ to $j$ and define the probability current $J_{ij}=w_{ij}P_i-w_{ji}P_j=-J_{ji}$. The [master equation](../../../../../../master-equation.md) is $\dot P_i=-\sum_jJ_{ij}$. Differentiating the Shannon entropy $S_{\rm sys}=-\sum_iP_i\log P_i$ and symmetrizing gives

$$
\dot S_{\rm sys}=\frac12\sum_{i,j}J_{ij}\log\frac{P_i}{P_j}.
$$

Adding the entropy flow to the environment produces the nonnegative [entropy production rate of a Markov chain](../../../../../../entropy-production-rate-of-a-markov-chain.md)

$$
\boxed{\dot S_{\rm tot}=\frac12\sum_{i,j}J_{ij}
\log\frac{w_{ij}P_i}{w_{ji}P_j}\geq0.}
$$

The paper's displayed $\sum P\log P$ is the negative of the thermodynamic system entropy, so its derivative has the opposite sign before the environmental contribution is added.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
