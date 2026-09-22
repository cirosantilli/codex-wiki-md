<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

Each coordinate lies in $[0,1]$. Since $0<c<1$, $x_i^c\geq x_i$, with equality exactly when $x_i=0$ or $1$. Summing gives $f(\mathbf x)\geq1$. Equality under the simplex constraint forces exactly one coordinate to be one. Thus **the minimum is $1$, attained exactly at the vertices** of the [probability simplex](../../../../../probability-simplex.md).

For the maximum, $t\mapsto t^c$ is strictly concave on $[0,\infty)$. The [Jensen inequality](../../../../../jensen-s-inequality.md) gives

$$
\frac1n\sum_{i=1}^nx_i^c\leq\left(\frac1n\sum_{i=1}^nx_i\right)^c=n^{-c}.
$$

Strict concavity makes equality possible exactly when all coordinates agree. Hence the [extrema of a concave power sum on a simplex](../../../../../extrema-of-a-concave-power-sum-on-a-simplex.md) are

$$
\boxed{\min f=1,\qquad \max f=n^{1-c},\quad x_1=\cdots=x_n=1/n\ \text{at the maximum}.}
$$

For $n=1$ the simplex is a single point, and both descriptions coincide.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
