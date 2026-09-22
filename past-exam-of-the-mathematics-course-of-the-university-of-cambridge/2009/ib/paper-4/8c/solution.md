<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For distinct [Gaussian quadrature](../../../../../gaussian-quadrature.md) nodes, let $\ell_i$ be the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) with $\ell_i(x_j)=\delta_{ij}$. Since $\ell_i^2$ has degree $2n-2$, exactness gives

$$
\boxed{b_i=\sum_jb_j\ell_i(x_j)^2=\int_a^bw(x)\ell_i(x)^2\,dx>0.}
$$

The last inequality follows from $w>0$ on the interval and the nonzero polynomial $\ell_i$ being nonzero on a subinterval. It does not require prior knowledge of the signs of the weights.

For $n=2$, the nodes are the roots of the supplied [orthogonal polynomial](../../../../../orthogonal-polynomial.md) $p_2$:

$$
\boxed{x_1=-\sqrt{2/5},\qquad x_2=\sqrt{2/5},\qquad b_1=b_2=\frac43.}
$$

Indeed exactness for $1$ gives $b_1+b_2=\int_{-1}^1(1+x^2)\,dx=8/3$, and exactness for $x$ gives equality of the weights.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
