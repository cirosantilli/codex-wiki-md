<h1 id="15b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With [Hamilton's equations](../../../../../../hamilton-s-equations.md) $\dot q_j=H_{p_j}$ and $\dot p_j=-H_{q_j}$, the chain rule gives

$$
\boxed{\frac{dF}{dt}=\sum_j(F_{q_j}H_{p_j}-F_{p_j}H_{q_j})=[F,H].}
$$

For the vortex problem, combine the two ordered terms for each unordered pair, writing $D_{ij}=(p_i-p_j)^2+(q_i-q_j)^2$ and $H=-(\kappa/2)\sum_{i<j}\log D_{ij}$. Since $F_{q_j}=2q_j$, $F_{p_j}=2p_j$, its pairwise contribution to the [Poisson bracket](../../../../../../poisson-bracket.md) is

$$
-\frac{2\kappa}{D_{ij}}
\bigl[(q_i-q_j)(p_i-p_j)-(p_i-p_j)(q_i-q_j)\bigr]=0.
$$

Every pair cancels, so $[F,H]=0$ and **$\sum_j(q_j^2+p_j^2)$ is conserved** along any collision-free solution. The logarithmic [Hamiltonian](../../../../../../hamiltonian.md) is undefined at coinciding vortices, so the derivation applies on its natural domain.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15B](../../15b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
