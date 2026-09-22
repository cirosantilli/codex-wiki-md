<h1 id="a/3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The standard [conjugate gradient convergence bound](../../../../../conjugate-gradient-convergence-bound.md) is

$$
\|e_k\|_A\leq2\left(\frac{\sqrt\kappa-1}{\sqrt\kappa+1}\right)^k\|e_0\|_A.
$$

Here $\kappa\leq5$, so the factor in parentheses is at most $q=(3-\sqrt5)/2\simeq0.381966$. Since $2q^{25}<10^{-10}$, **25 iterations suffice to reduce the energy-norm error by a factor exceeding $10^{10}$**.

There are at most $m/20$ nonzero entries of $t$, and each contributes to at most two off-diagonals. Thus $A-I$ has at most $m^2/10$ nonzero entries. Initialize a matrix-vector product with the diagonal contribution $p$, which costs no arithmetic because the diagonal is one. Each off-diagonal term needs one multiplication and one addition, giving at most $m^2/5$ [floating-point operations](../../../../../floating-point-operation.md) per product.

A standard [conjugate gradient](../../../../../conjugate-gradient-method.md) step adds two inner products, three vector updates and two scalar divisions, at most $10m$ further operations. Starting from $x_0=0$ makes $r_0=b$ and avoids an initial matrix-vector product; its squared norm needs $2m-1$ operations. The total for 25 steps is at most

$$
\boxed{25(m^2/5+10m)+2m-1=5m^2+252m-1<8m^2\quad(m\geq84).}
$$

This supplies an explicit meaning of the paper's large-$m$ qualification. The quoted [conjugate gradient convergence bound](../../../../../conjugate-gradient-convergence-bound.md) is the usual exact-arithmetic result.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
