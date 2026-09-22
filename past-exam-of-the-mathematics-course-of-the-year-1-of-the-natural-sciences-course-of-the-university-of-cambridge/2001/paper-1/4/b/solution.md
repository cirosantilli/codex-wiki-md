<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work first with $|k|<1$, so the real integrands and their parameter [derivatives](../../../../../derivative.md) are smooth on every finite amplitude interval. For the [elliptic integral of the second kind](../../../../../elliptic-integral-of-the-second-kind.md),

$$
E_k=-k\int_0^\theta\frac{\sin^2x}{\sqrt{1-k^2\sin^2x}}dx.
$$

On the other hand, subtracting the integrands of the second-kind and first-kind [elliptic integrals](../../../../../elliptic-integral.md) gives

$$
E-F=\int_0^\theta\frac{(1-k^2\sin^2x)-1}{\sqrt{1-k^2\sin^2x}}dx=-k^2\int_0^\theta\frac{\sin^2x}{\sqrt{1-k^2\sin^2x}}dx.
$$

Consequently

$$
\boxed{E_k=\frac{E-F}{k}\quad(k\ne0).}
$$

This is the [modulus derivative of the incomplete elliptic integral of the second kind](../../../../../modulus-derivative-of-the-incomplete-elliptic-integral-of-the-second-kind.md). At $k=0$ its right-hand side has a removable limit zero, agreeing with $E_k(\theta,0)=0$. Both $E$ and $F$ here use amplitude $\theta$ and modulus $k$; differentiating with respect to the alternative parameter $k^2$ would give a different prefactor.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
