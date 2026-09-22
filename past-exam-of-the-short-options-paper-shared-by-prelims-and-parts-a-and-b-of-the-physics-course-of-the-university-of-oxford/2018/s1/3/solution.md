<h1 id="s1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At a regular point, $f(z_0+\zeta)-f(z_0)=f'(z_0)\zeta+O(\zeta^2)$. Multiplication by a nonzero [complex number](../../../../complex-number.md) rotates every tangent by the same angle and multiplies every [length](../../../../length.md) by the same positive factor. Oriented angles are preserved. If the first [derivative](../../../../derivative.md) vanishes but the second does not, the leading term is $f''(z_0)\zeta^2/2$: tangent arguments are doubled, so angles are doubled, modulo the identification of rays. This is a local statement; [holomorphy](../../../../holomorphic-function-split.md) alone does not imply global [injectivity](../../../../injective-function.md).

Write $z=x+iy$. Then

$$
w=\sin\frac{\pi x}{2}\cosh\frac{\pi y}{2}
+i\cos\frac{\pi x}{2}\sinh\frac{\pi y}{2}.
$$

For $-1<x<1$ and $y>0$, the imaginary part is positive. The bottom edge maps monotonically to $[-1,1]$; the left and right vertical edges map to $(-\infty,-1]$ and $[1,\infty)$ respectively. The inverse below establishes that every point of the open upper half-plane occurs exactly once. At fixed $y=a$, putting $u=\operatorname{Re}w$, $v=\operatorname{Im}w$, one obtains

$$
\boxed{\frac{u^2}{\cosh^2(\pi a/2)}+
\frac{v^2}{\sinh^2(\pi a/2)}=1,\qquad v\ge0.}
$$

This is the upper half of an [ellipse](../../../../ellipse.md), traversed from its left endpoint to its right endpoint.

Choose the branch $s(w)=\sqrt{1-w^2}$ analytic in the upper half-plane and positive on the boundary interval $(-1,1)$. Then the inverse branch into the strip is

$$
\boxed{z=-\frac{2i}{\pi}\log\bigl(iw+s(w)\bigr).}
$$

The [logarithm](../../../../logarithm.md) is chosen continuously so that $-1<\operatorname{Re}z<1$ and $\operatorname{Im}z>0$; for instance $w=iv$, $v>0$, gives $z=(2i/\pi)\operatorname{arsinh}v$. Differentiation gives $dz/dw=2/(\pi\sqrt{1-w^2})$. The only zeros of the original [derivative](../../../../derivative.md) in the closed strip are $z=\pm1$, with images $w=\pm1$. The inverse has square-root [branch points](../../../../branch-point.md) there, and cannot extend holomorphically across them. At either corner the original map doubles the right angle to a straight angle; a holomorphic inverse with nonzero [derivative](../../../../derivative.md) could not halve it. The open strip interior has no such failure.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [S1](../../s1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
