<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A free [point vortex](../../../../../line-vortex.md) is advected by the regular part of the [velocity field](../../../../../velocity-field.md) at its position. Its own singular [complex velocity](../../../../../complex-velocity.md) $\Gamma/[2\pi i(z-c)]$ must first be subtracted. The image expression therefore gives

$$
\boxed{\dot x_c-i\dot y_c
=\lim_{z\to c}\left[w'(z)-\frac\Gamma{2\pi i(z-c)}\right]
=\frac\Gamma{2\pi i}
\left[\frac1{c-c^{-1}}-\frac1{c-\bar c}
-\frac1{c-\bar c^{-1}}\right]}.
$$

Equivalently, $\dot c$ is the [complex conjugate](../../../../../complex-conjugate.md) of the boxed expression. This is the instantaneous [velocity](../../../../../velocity.md), evaluated with the current value of $c$.

To see why mapping the image [velocity](../../../../../velocity.md) alone would miss a term, expand the mapped physical singularity:

$$
\frac{g'(z)}{g(z)-g(c)}
=\frac1{z-c}+\frac{g''(c)}{2g'(c)}+O(z-c).
$$

Thus the same [point-vortex drift under a conformal map](../../../../../point-vortex-drift-under-a-conformal-map.md) can be written

$$
\dot x_c-i\dot y_c
=\frac\Gamma{2\pi i}
\left[\frac{g''(c)}{2g'(c)}
-\frac{g'(c)}{g(c)-\overline{g(c)}}\right].
$$

The finite term involving $g''$ is part of the physical regular [velocity field](../../../../../velocity-field.md).

If $c=id$ with $d>1$, direct substitution into the image expression gives

$$
\begin{aligned}
\dot x_c-i\dot y_c
&=\frac\Gamma{2\pi}
\left[-\frac d{d^2+1}+\frac1{2d}+\frac d{d^2-1}\right]\\
&=\boxed{\frac\Gamma{2\pi}
\left[\frac1{2d}+\frac{2d}{d^4-1}\right]}.
\end{aligned}
$$

The bracket is strictly positive, and the result is real. Hence a positive [line vortex](../../../../../line-vortex.md) initially moves horizontally to the right, a negative [line vortex](../../../../../line-vortex.md) moves to the left, and the initial vertical [velocity](../../../../../velocity.md) is zero. As $d\to\infty$, the leading term $\Gamma/(4\pi d)$ is the familiar drift of a [point vortex](../../../../../line-vortex.md) above a straight wall.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
