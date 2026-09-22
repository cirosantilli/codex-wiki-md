<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [supremum norm barrier for an elliptic Dirichlet problem](../../../../../../supremum-norm-barrier-for-an-elliptic-dirichlet-problem.md) to obtain a domain-only constant $C_\Omega=e^{2d}$. Split the coefficient as $c=c_-+c_+$, where $c_-\leq0$ and $c_+=\max(c,0)$. Both parts are [Hölder continuous functions](../../../../../../holder-condition.md). Choose

$$
\boxed{\epsilon(\Omega)=\frac1{2C_\Omega}>0.}
$$

If $u$ solves the homogeneous zero-boundary problem for $\Delta+c$, then

$$
(\Delta+c_-)u=-c_+u.
$$

Part (a), applied to this nonpositive zeroth-order coefficient, gives

$$
\|u\|_\infty\leq C_\Omega\|c_+u\|_\infty
\leq C_\Omega\epsilon\|u\|_\infty=\tfrac12\|u\|_\infty.
$$

Hence $u=0$. The [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md) now gives existence and uniqueness for every forcing and boundary datum in the stated [Hölder spaces](../../../../../../holder-space.md). This proves the [small positive zeroth-order perturbation of a Dirichlet problem](../../../../../../small-positive-zeroth-order-perturbation-of-a-dirichlet-problem.md) without imposing a bound on the negative part of $c$. The value of $\epsilon$ need not be optimal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
