<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a nonnegative integer $m$, expand the [plane wave](../../../../../plane-wave.md) in powers of $\rho$:

$$
e^{i\rho\cos\theta}=\sum_{n=0}^{\infty}\frac{(i\rho)^n}{n!}
\left(\frac{e^{i\theta}+e^{-i\theta}}2\right)^n.
$$

The first contribution to the positive angular harmonic $e^{im\theta}$ occurs at $n=m$. Its coefficient is $(i\rho)^m/(2^m m!)$. Comparing this with $a_mJ_m(\rho)\sim a_m\rho^m/(2^m m!)$ gives $a_m=i^m$ for $m\geq0$.

The [plane wave](../../../../../plane-wave.md) is even in $\theta$, so its $m$ and $-m$ [Fourier coefficients](../../../../../fourier-coefficient.md) agree. Therefore $a_{-m}J_{-m}=a_mJ_m$, implying $a_{-m}=(-1)^mi^m=i^{-m}$. Hence

$$
\boxed{a_m=i^m\quad(m\in\mathbb Z),\qquad
e^{i\rho\cos\theta}=\sum_{m=-\infty}^{\infty}i^mJ_m(\rho)e^{im\theta}.}
$$

This is the cosine form of the [Jacobi-Anger expansion](../../../../../jacobi-anger-expansion.md). The factorial asymptotic stated in the source is used for nonnegative order; applying it literally to negative integers would introduce an undefined factorial. The [Integer-order Bessel reflection identity](../../../../../integer-order-bessel-reflection-identity.md) is the required extension, not a separate set of divergent radial solutions.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
