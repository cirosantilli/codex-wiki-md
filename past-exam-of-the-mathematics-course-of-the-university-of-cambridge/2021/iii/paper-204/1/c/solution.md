<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider walks assembled from blocks $E$, $EN^k$, and $ES^k$ with $k\geq1$. Their horizontal coordinate increases once in every block, and within each vertical line they move monotonically, so every such walk is self-avoiding. If $c_n$ counts these walks by total length, its [ordinary generating function](../../../../../../ordinary-generating-function.md) is

$$
\sum_{n\geq0}c_nz^n
=\frac1{1-\left(z+2\sum_{k\geq1}z^{k+1}\right)}
=\frac{1-z}{1-2z-z^2}.
$$

Its positive dominant singularity is $z=\sqrt2-1$, so $\lim_nc_n^{1/n}=1+\sqrt2$. Since $b_n\geq c_n$,

$$
\boxed{\kappa\geq1+\sqrt2>2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
