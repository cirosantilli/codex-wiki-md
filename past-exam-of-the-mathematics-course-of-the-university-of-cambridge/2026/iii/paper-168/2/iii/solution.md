<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We prove the [anticoncentration of a low-degree function](../../../../../../anticoncentration-of-a-low-degree-function.md) by induction on $n$. Write

$$
f(x_1,\ldots,x_n)=g(x_1,\ldots,x_{n-1})+x_nh(x_1,\ldots,x_{n-1}),
$$

where $\deg g\leq k$ and $\deg h\leq k-1$. If $h=0$, the induction hypothesis in dimension $n-1$ applies to $g$. If $h\ne0$, then whenever $h(x')\ne0$, at least one of $g(x')+h(x')$ and $g(x')-h(x')$ is nonzero. Therefore

$$
\mathbb P[f\ne0]
\geq\frac12\mathbb P[h\ne0]
\geq\frac12,2^{-(k-1)}=2^{-k}.
$$

The dimension-zero case is immediate, so the induction is complete.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
