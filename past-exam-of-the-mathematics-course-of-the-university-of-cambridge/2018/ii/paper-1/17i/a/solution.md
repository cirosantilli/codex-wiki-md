<h1 id="17i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
d_n(H)=\frac{\operatorname{ex}(n,H)}{\binom n2}.
$$

Let $G$ be an $H$-free [graph](../../../../../../graph-split.md) on $n$ vertices with $\operatorname{ex}(n,H)$ edges, and choose a uniformly random set of $m<n$ vertices. Its [induced subgraph](../../../../../../induced-subgraph.md) is still $H$-free, and each edge survives with probability $\binom m2/\binom n2$. Hence

$$
\operatorname{ex}(m,H)\geq
\operatorname{ex}(n,H)\frac{\binom m2}{\binom n2},
$$

so $d_m(H)\geq d_n(H)$. Thus the normalized [extremal number](../../../../../../extremal-number.md) is nonincreasing and bounded below by zero, proving that

$$
\boxed{\ \lim_{n\to\infty}\frac{\operatorname{ex}(n,H)}{\binom n2}\ \text{exists}.\ }
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17I](../../17i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
