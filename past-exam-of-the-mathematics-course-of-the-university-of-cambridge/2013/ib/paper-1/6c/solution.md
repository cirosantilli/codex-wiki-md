<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

For [two-node Gaussian quadrature with linear weight](../../../../../two-node-gaussian-quadrature-with-linear-weight.md), the monic node [polynomial](../../../../../polynomial-split.md) $q(x)=x^2-sx+p$ must be orthogonal to $1$ and $x$ for weight $x$. Indeed, exactness through degree three makes the quadrature of $q$ and $xq$ vanish at its nodes. The moment equations are

$$
\frac14-\frac s3+\frac p2=0,\qquad
\frac15-\frac s4+\frac p3=0,
$$

so $s=6/5$ and $p=3/10$. Thus the [Gaussian quadrature](../../../../../gaussian-quadrature.md) nodes, labelled in increasing order, are

$$
\boxed{x_1=\frac{6-\sqrt6}{10},\qquad x_2=\frac{6+\sqrt6}{10}.}
$$

Integrating the linear [Lagrange interpolation](../../../../../lagrange-polynomial.md) cardinal functions gives the weights

$$
\boxed{a_1=\frac{x_2/2-1/3}{x_2-x_1},\qquad
a_2=\frac{1/3-x_1/2}{x_2-x_1}.}
$$

They are positive, sum to $1/2$, and reproduce the first moment $1/3$. Any cubic [polynomial](../../../../../polynomial-split.md) has remainder of degree at most one after division by $q$; orthogonality annihilates the other part both in the integral and at the nodes. This proves degree-three exactness, not merely the two moment conditions for the weights.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
