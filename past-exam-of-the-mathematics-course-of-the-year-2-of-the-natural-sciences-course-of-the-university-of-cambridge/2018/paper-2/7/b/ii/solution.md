<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the stated parameters, the [mass](../../../../../../mass.md) and restoring [matrices](../../../../../../matrix.md) are

$$
A=\begin{pmatrix}2&1\\1&1\end{pmatrix},\qquad
B=\begin{pmatrix}2&0\\0&1\end{pmatrix}.
$$

The [generalized eigenvalue problem](../../../../../../generalized-eigenvalue-problem.md) gives

$$
\det(B-\omega^2A)=(2-2\omega^2)(1-\omega^2)-\omega^4
=\omega^4-4\omega^2+2=0.
$$

Therefore the two normal [angular frequencies](../../../../../../angular-frequency.md) are

$$
\boxed{\omega_{\mathrm{low}}=\sqrt{2-\sqrt2},\qquad
\omega_{\mathrm{high}}=\sqrt{2+\sqrt2}}.
$$

The second row of the modal equation is $-\omega^2x+(1-\omega^2)\phi=0$. It gives the [mode shapes](../../../../../../mode-shape.md)

$$
\boxed{\begin{aligned}
\omega_{\mathrm{low}}:&\quad (x,\phi)=a(1,\sqrt2)\cos(\omega_{\mathrm{low}}t+\delta),\\
\omega_{\mathrm{high}}:&\quad (x,\phi)=a(1,-\sqrt2)\cos(\omega_{\mathrm{high}}t+\delta).
\end{aligned}}
$$

Each [normal mode](../../../../../../normal-mode.md) has arbitrary small amplitude $a$ and phase $\delta$. The bob's horizontal displacement is $X=x+\phi$ to first order. Thus in the lower mode, bob and cart move in phase, with bob amplitude $1+\sqrt2$ times the cart amplitude. In the higher mode they move oppositely, because $X=(1-\sqrt2)x$; the bob amplitude is $\sqrt2-1$ times the cart amplitude. Its vertical displacement is quadratic in the angle and is absent at this order.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
