<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Denote the [damped free-transport evolution](../../../../../../damped-free-transport-evolution.md) from time $s$ to time $t$ by

$$
(U_a(t,s)g)(x,v)=
e^{-\int_s^t a(r,x-v(t-r),v)\,dr}g(x-v(t-s),v).
$$

By the argument in (b), $\|U_a(t,s)g\|_2\leq\|g\|_2$. The integral operator is the [Boltzmann Volterra operator](../../../../../../boltzmann-volterra-operator.md)

$$
\tau f(t)=\int_0^tU_a(t,s)K_sf(s)\,ds.
$$

The [Minkowski integral inequality](../../../../../../minkowski-integral-inequality.md) and (a) give the useful stronger pointwise bound

$$
\|\tau f(t)\|_2\leq C\int_0^t\|f(s)\|_2\,ds.
$$

Therefore **the requested estimate is**

$$
\boxed{\|\tau f(t)\|_2\leq Ct\,\sup_{0\leq s\leq t}\|f(s)\|_2.}
$$

For strongly measurable bounded $L^2$-valued $f$, these are [Bochner integrals](../../../../../../bochner-integral.md); their finite norm bounds establish existence of the integrals.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
