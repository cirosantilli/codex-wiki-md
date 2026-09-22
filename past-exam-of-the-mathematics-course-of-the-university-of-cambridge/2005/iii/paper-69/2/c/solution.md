<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), write $z=h\lambda$. The amplification roots solve

$$
(7-4z)\zeta^2-12\zeta+5+2z=0.
$$

A root on $|\zeta|=1$ would require the boundary-locus value

$$
z=\frac{7\zeta^2-12\zeta+5}{4\zeta^2-2}.
$$

Its denominator cannot vanish on that circle. Setting $\zeta=e^{i\theta}$ and simplifying the real part gives

$$
\operatorname{Re}z=\frac{3(1-\cos\theta)^2}{9-8\cos^2\theta}\geq0.
$$

Thus no amplification root can cross the unit circle while $\operatorname{Re}z<0$. The leading coefficient is also nonzero throughout that half-plane. At $z=-1$, the roots are $(6\pm\sqrt3)/11$, both strictly inside the unit disk. Connect any other left-half-plane point to $-1$: continuity of the roots, without a boundary crossing or a root escaping through infinity, keeps both roots inside.

On the imaginary axis a boundary root can occur only at $\theta=0$, which gives $z=0$; there the roots $1$ and $5/7$ satisfy the simple-unit-root condition. Hence **$\boxed{\text{the method is A-stable}}$**, including the usual boundary root convention at zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
