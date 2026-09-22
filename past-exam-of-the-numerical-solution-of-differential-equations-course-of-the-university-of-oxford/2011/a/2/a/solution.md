<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the normalization used by the supplied coefficient expansion, the [local truncation error](../../../../../local-truncation-error.md) of the [linear multistep method](../../../../../linear-multistep-method-split.md) is

$$
\boxed{T_n=\frac{\sum_{j=0}^k\alpha_jy(x_{n+j})-h\sum_{j=0}^k\beta_jy'(x_{n+j})}{h\sum_{j=0}^k\beta_j}.}
$$

The nonzero sum in the denominator is an explicit hypothesis. [Consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) requires $T_n\to0$ uniformly on a fixed finite time interval for every sufficiently smooth exact solution as $h\to0$. Equivalently, the two [polynomial](../../../../../polynomial-split.md) identities are

$$
\boxed{\rho(1)=0,\qquad\rho'(1)=\sigma(1),\quad
\rho(\zeta)=\sum_j\alpha_j\zeta^j,\quad\sigma(\zeta)=\sum_j\beta_j\zeta^j.}
$$

These follow by inserting constant and affine functions, or by setting the first two Taylor coefficients $C_0,C_1$ to zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
