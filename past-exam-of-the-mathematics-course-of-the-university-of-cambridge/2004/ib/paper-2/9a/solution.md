<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Use the weighted [inner product](../../../../../inner-product.md) $\langle u,v\rangle=\int_0^1u(x)v(x)x\,dx$. A monic quadratic [orthogonal polynomial](../../../../../orthogonal-polynomial.md) $\pi_2(x)=x^2+ax+b$, orthogonal to 1 and $x$, satisfies

$$
\frac14+\frac a3+\frac b2=0,\qquad \frac15+\frac a4+\frac b3=0.
$$

Thus $a=-6/5$, $b=3/10$, and its two zeros are $x_-=(6-\sqrt6)/10$ and $x_+=(6+\sqrt6)/10$. Matching the first two weighted moments gives

$$
w_-+w_+=\frac12,\qquad w_-x_-+w_+x_+=\frac13,
$$

so $w_-=(9-\sqrt6)/36$ and $w_+=(9+\sqrt6)/36$. The [two-node Gaussian quadrature with linear weight](../../../../../two-node-gaussian-quadrature-with-linear-weight.md) is therefore

$$
\boxed{\int_0^1f(x)x\,dx\ \approx\ \frac{9-\sqrt6}{36}f\!\left(\frac{6-\sqrt6}{10}\right)+\frac{9+\sqrt6}{36}f\!\left(\frac{6+\sqrt6}{10}\right).}
$$

For completeness, a [polynomial](../../../../../polynomial-split.md) $P$ of degree at most three can be divided as $P=q\pi_2+r$, where both $q$ and $r$ have degree at most one. Orthogonality makes the weighted [integral](../../../../../integral.md) of $q\pi_2$ zero, and this term vanishes at both nodes. The two moment equations integrate $r$ exactly. Thus the [Gaussian quadrature](../../../../../gaussian-quadrature.md) is exact for every cubic [polynomial](../../../../../polynomial-split.md). No two-node rule can integrate every quartic: the square of its nodal polynomial has quadrature value zero and strictly positive weighted [integral](../../../../../integral.md).

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
