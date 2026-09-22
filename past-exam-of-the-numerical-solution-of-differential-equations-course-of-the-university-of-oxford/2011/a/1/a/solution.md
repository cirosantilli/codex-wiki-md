<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the normalized [local truncation error](../../../../../local-truncation-error.md)

$$
T_n=\frac{y(x_{n+1})-y(x_n)}h-\theta y'(x_{n+1})-(1-\theta)y'(x_n).
$$

The [Taylor theorem](../../../../../taylor-s-theorem.md) expansions about $x_n$ are

$$
\frac{y(x_n+h)-y(x_n)}h=y'(x_n)+\frac h2y''(x_n)+\frac{h^2}6y'''(\xi_n),\qquad
y'(x_n+h)=y'(x_n)+hy''(x_n)+\frac{h^2}2y'''(\eta_n).
$$

Substitution gives exactly

$$
\boxed{T_n=\frac h2(1-2\theta)y''(x_n)+\frac{h^2}6[y'''(\xi_n)-3\theta y'''(\eta_n)]}.
$$

Thus the [theta method](../../../../../theta-method.md) has **order two exactly for $\theta=1/2$**, and otherwise order one, as a statement about the method on a sufficiently smooth class of problems. The leading term vanishes at one half, and a function with nonzero third [derivative](../../../../../derivative.md) shows that the next term does not vanish universally. As usual, a uniform order estimate assumes bounded relevant [derivatives](../../../../../derivative.md); mere existence of $y'''$ on the open interval gives the stated pointwise remainders but not, by itself, a uniform bound. Special exact solutions can of course have zero truncation error even for a first-order method.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
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
