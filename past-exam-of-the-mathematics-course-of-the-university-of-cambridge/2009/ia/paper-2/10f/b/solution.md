<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Galton-Watson extinction fixed point](../../../../../../galton-watson-extinction-fixed-point.md) equation is

$$
(1+2q)^3=27q,\qquad
8q^3+12q^2-21q+1=(q-1)(8q^2+20q-1)=0.
$$

Its smallest root in $[0,1]$ is $q=(3\sqrt3-5)/4$, not the other allowed fixed point $1$. Consequently the large-depth escape probability is

$$
\boxed{1-q=\frac{9-3\sqrt3}{4}\approx0.95096.}
$$

For finite $N$, the exact escape probability is $1-q_N$ and is slightly larger. Indeed $\phi'(q)=2-\sqrt3<1$, and the [mean value theorem](../../../../../../mean-value-theorem.md) on $[q_N,q]$ gives $0\leq q-q_N\leq q(2-\sqrt3)^N$. This also quantifies how quickly the finite-depth answer approaches the displayed limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
