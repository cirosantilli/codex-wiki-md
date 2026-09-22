<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define

$$
F_+(t)=\frac12\{\Phi(t)+\Phi(t-2b_1)\},
\qquad
F_-(t)=F_+(t+2b_1)
=\frac12\{\Phi(t)+\Phi(t+2b_1)\}.
$$

Thus $F_+$ is the equal mixture of $N(0,1)$ and $N(2b_1,1)$, while $F_-$ is the equal mixture of $N(0,1)$ and $N(-2b_1,1)$. They have finite variance and everywhere positive densities. Normal symmetry shows that $F_+$ is symmetric about $b_1$ and $F_-$ about $-b_1$.

For every $t$,

$$
0\leq\Phi(t)-\Phi(t-2b_1)
\leq\Phi(b_1)-\Phi(-b_1)=2\varepsilon,
$$

where the maximum occurs at $t=b_1$. Consequently

$$
|F_+(t)-\Phi(t)|
=\frac12|\Phi(t-2b_1)-\Phi(t)|
\leq\varepsilon.
$$

The same argument, shifted and reflected, applies to $F_-$. Hence both distributions belong to $\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M$ and satisfy the required translation relation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
