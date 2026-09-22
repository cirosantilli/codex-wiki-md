<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The normalized Dirichlet [eigenfunctions](../../../../../eigenfunction.md) on $(-L,L)$ and their decay rates are

$$
\varphi_n(x)=\frac1{\sqrt L}\sin\frac{n\pi(x+L)}{2L},\qquad
E_n=D\left(\frac{n\pi}{2L}\right)^2,\quad n=1,2,\ldots.
$$

Their norms are one because the sine-squared integral is $L$. At the initial [position](../../../../../position.md) zero, $\varphi_n(0)=L^{-1/2}\sin(n\pi/2)$, so all even $n$ disappear. For $n=2j+1$, the two signs from $\varphi_n(x)$ and $\varphi_n(0)$ cancel, yielding

$$
\boxed{K_{|x|<L}(x,t|0,0)=\frac{\Theta(t)}L
\sum_{j=0}^{\infty}
\cos\frac{(2j+1)\pi x}{2L}
\exp\!\left[-\frac{(2j+1)^2\pi^2Dt}{4L^2}\right].}
$$

This holds for $|x|<L$ and is zero outside. The kernel is even in $x$, vanishes at both boundaries and tends weakly to the initial delta. The [eigenvalues](../../../../../eigenvalue.md) are decay rates rather than quantum energies unless one makes an additional unit convention.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
