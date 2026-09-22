<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the following normalization of the [local truncation error](../../../../local-truncation-error.md), also called the [consistency error](../../../../normalized-local-truncation-error.md): insert a smooth exact solution into the [linear multistep method](../../../../linear-multistep-method-split.md) and divide the residual by $h$,

$$
T_n(h)=\frac1h\sum_{j=0}^k\alpha_jy(x_n+jh)-\sum_{j=0}^k\beta_jy'(x_n+jh).
$$

Thus the unscaled defect is $hT_n(h)$. [Consistency of a numerical method](../../../../consistency-of-a-numerical-method.md) means that $T_n(h)\to0$ uniformly over mesh points in each fixed interval for every sufficiently smooth exact solution. Write the [characteristic polynomials of a linear multistep method](../../../../characteristic-polynomials-of-a-linear-multistep-method.md) as

$$
\rho(z)=\sum_{j=0}^k\alpha_jz^j,\qquad \sigma(z)=\sum_{j=0}^k\beta_jz^j.
$$

By [Taylor's theorem](../../../../taylor-s-theorem.md), [consistency of a numerical method](../../../../consistency-of-a-numerical-method.md) is equivalent to

$$
\sum_j\alpha_j=0,\qquad \sum_jj\alpha_j=\sum_j\beta_j,
$$

or $\rho(1)=0$ and $\rho'(1)=\sigma(1)$.

Second-order accuracy means $T_n(h)=O(h^2)$ for smooth solutions, equivalently an unscaled [local truncation error](../../../../local-truncation-error.md) $O(h^3)$. In addition to the two consistency conditions, its order conditions require

$$
\sum_jj^2\alpha_j=2\sum_jj\beta_j.
$$

An [order of a numerical method](../../../../order-of-a-numerical-method.md) of exactly two additionally requires that the next order condition fails. These statements concern the local defect; a second-order [global error](../../../../global-discretization-error.md) requires stability and suitably accurate starting values as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and numerical solution of differential equations course of the University of Oxford](../../../../numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [MSc in mathematical modelling and scientific computing course of the University of Oxford](../../../../msc-in-mathematical-modelling-and-scientific-computing-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
