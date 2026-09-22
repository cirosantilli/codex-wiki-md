<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [directed acyclic graph factorization](../../../../../../directed-acyclic-graph-factorization.md) is

$$
p(x_1,u,x_2,x_3,x_4)
=p(x_1)p(u)p(x_2\mid x_1,u)
p(x_3\mid x_1,x_2)p(x_4\mid x_3,u).
$$

The graph gives $U\perp X_1$ and $U\perp X_3\mid(X_1,X_2)$. Therefore [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
p(u\mid x_1,x_2,x_3)
=p(u\mid x_1,x_2)
=\frac{p(u)p(x_2\mid x_1,u)}{p(x_2\mid x_1)}.
$$

Consequently

$$
\begin{aligned}
&\sum_{x_2}p(x_4\mid x_1,x_2,x_3)p(x_2\mid x_1)\\
&=\sum_{x_2,u}p(x_4\mid x_3,u)p(u)p(x_2\mid x_1,u)\\
&=\sum_up(x_4\mid x_3,u)p(u),
\end{aligned}
$$

which contains no $x_1$. This observed equality is a [Verma constraint](../../../../../../verma-constraint.md): it is implied by the latent-variable causal graph even though it is not a conditional independence.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
