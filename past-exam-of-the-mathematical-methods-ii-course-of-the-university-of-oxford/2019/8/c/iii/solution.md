<h1 id="8/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $n=1$, the [azimuthal unit vector](../../../../../azimuthal-unit-vector.md) is $\hat\theta=(-\sin\theta,\cos\theta,0)$, so

$$
\boxed{F=\frac1r\hat\theta.}
$$

On a counterclockwise circle $C_r$ at fixed height, $dr=r\hat\theta\,d\theta$. Hence

$$
\boxed{\oint_{C_r}F\cdot dr=\int_0^{2\pi}\frac1r\,r\,d\theta=2\pi,}
$$

independent of the positive radius. Clockwise orientation reverses the sign.

There is no contradiction with the zero [curl](../../../../../curl.md) found in [solution](../i/solution.md). The [vector field](../../../../../vector-field.md) is undefined on the axis, so it is not continuously differentiable on a disc spanning $C_r$; the hypotheses of [Stokes theorem](../../../../../stokes-theorem.md) fail for that disc. It is smooth on a planar annulus excluding the axis, where [Stokes theorem](../../../../../stokes-theorem.md) correctly gives zero: the two boundary [line integrals](../../../../../line-integral.md) cancel, $2\pi-2\pi=0$.

The same check works for general $n$. A counterclockwise circle has circulation $\Gamma(r)=2\pi r^{2-2n}$. Integrating the [curl](../../../../../curl.md) over an annulus $a\leq r\leq R$ gives, for $n\ne1$,

$$
\int_a^R2(1-n)r^{-2n}\,2\pi r\,dr
=2\pi\big(R^{2-2n}-a^{2-2n}\big)=\Gamma(R)-\Gamma(a).
$$

For $n=1$, both sides are zero. Thus all three preceding results are consistent with [Stokes theorem](../../../../../stokes-theorem.md); the necessary distinctions are the regularity of the [vector field](../../../../../vector-field.md) and inclusion of every oriented boundary component.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
