<h1 id="17b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix a [continuous function](../../../../../../continuous-function.md) $f$ and $\varepsilon>0$. By the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md), choose a polynomial $p\in\mathcal P_m$ such that

$$
\lVert f-p\rVert_\infty<\varepsilon.
$$

For every $n\geq m$, exactness gives $I_n(p)=I(p)$. Positivity of the quadrature weights and exactness on the constant polynomial give

$$
\sum_{i=0}^na_i^{(n)}=I_n(1)=I(1)=\int_a^bw(x)\,dx.
$$

Consequently

$$
\begin{aligned}
|I_n(f)-I(f)|
&\leq |I_n(f-p)|+|I(f-p)|\\
&\leq \varepsilon\sum_{i=0}^na_i^{(n)}
+\varepsilon\int_a^bw(x)\,dx\\
&=2\varepsilon\int_a^bw(x)\,dx.
\end{aligned}
$$

Since $\varepsilon$ is arbitrary, $I_n(f)\to I(f)$. This is the [convergence of positive quadrature rules](../../../../../../convergence-of-positive-quadrature-rules.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
