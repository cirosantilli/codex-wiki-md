<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At fixed radius, use spherical coordinates in velocity space with polar angle $\alpha$ measured from the radial direction:

$$
v_r=v\cos\alpha,
\qquad
v_t=v\sin\alpha,
\qquad
L=rv\sin\alpha.
$$

The [galactic distribution function](../../../../../../galactic-distribution-function.md) and volume element give angular weight

$$
L^{p-2}d^3v
\propto \sin^{p-1}\alpha\,d\alpha\,d\varphi.
$$

All dependence on $v$, $r$, and $g(E)$ cancels from ratios of second moments. Symmetry in the tangential plane gives

$$
\frac{\sigma_\theta^2}{\sigma_r^2}
=\frac{\sigma_\phi^2}{\sigma_r^2}
=\frac{\frac12\int_0^\pi\sin^{p+1}\alpha\,d\alpha}
{\int_0^\pi\cos^2\alpha\sin^{p-1}\alpha\,d\alpha}.
$$

Writing the angular integrals as [beta function](../../../../../../beta-function.md) integrals and using the [Gamma function recurrence](../../../../../../gamma-function-recurrence.md),

$$
\frac12
\frac{B((p+2)/2,1/2)}{B(p/2,3/2)}
=\frac p2.
$$

Therefore, for every admissible energy factor $g$,

$$
\boxed{\sigma_\theta^2=\sigma_\phi^2
=\frac p2\sigma_r^2}.
$$

Equivalently, the [velocity-anisotropy parameter](../../../../../../velocity-anisotropy-parameter.md) is the constant $\beta=1-p/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
