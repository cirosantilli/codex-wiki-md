<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [axis-angle composition of orthogonal spin rotations](../../../../../axis-angle-composition-of-orthogonal-spin-rotations.md), set $A=\Omega T/2$ and $B=\Phi/2$. Multiplication, including $\sigma_z\sigma_x=i\sigma_y$, gives

$$
U_\Omega U_\Phi=C I-i\mathbf v\cdot\boldsymbol\sigma,
\quad C=\cos A\cos B,
\quad\mathbf v=(\cos A\sin B,\ \sin A\sin B,\ \sin A\cos B).
$$

One checks that $C^2+|\mathbf v|^2=1$. For $s=|\mathbf v|\ne0$, choose

$$
\boxed{\vartheta=2\operatorname{atan2}(s,C),\qquad
\hat{\mathbf n}=\frac1s(\cos A\sin B,\ \sin A\sin B,\ \sin A\cos B).}
$$

This choice retains the full [spinor](../../../../../spinor.md) sign and gives $U_\Omega U_\Phi=e^{-i\vartheta\hat{\mathbf n}\cdot\mathbf S}$. Repeated periods have the same axis:

$$
\boxed{U(NT-0^+,-0^+)=e^{-iN\vartheta\hat{\mathbf n}\cdot\mathbf S}.}
$$

Thus the [spin](../../../../../spin.md) expectation [vector](../../../../../vector.md) rotates through $N\vartheta$, interpreted modulo $2\pi$ as a spatial [rotation](../../../../../rotation-mathematics.md). The positive $y$ component comes from the stated ordering; reversing the two [rotations](../../../../../rotation-mathematics.md) changes that component's sign.

When $s=0$, the one-period operator is $+I$ or $-I$, and no unique [rotation](../../../../../rotation-mathematics.md) axis exists. The latter is a $2\pi$ spatial [rotation](../../../../../rotation-mathematics.md) with a minus sign on a spin-$1/2$ state. It is safer to retain this central group element than to replace the angle by zero in a [spinor](../../../../../spinor.md) calculation.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [1](../../1.md)
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
