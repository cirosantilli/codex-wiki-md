<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $0<|z|<R$, set $w=R^2/\bar z$, which lies outside the [closed disk](../../../../../closed-disc.md). On $|\zeta|=R$, direct algebra gives the [Poisson kernel](../../../../../poisson-kernel.md) identity

$$
\operatorname{Re}\frac{\zeta+z}{\zeta-z}=\frac{\zeta}{\zeta-z}-\frac{\zeta}{\zeta-w}.
$$

Using $d\theta=d\zeta/(i\zeta)$, the proposed [Poisson formula for a holomorphic function](../../../../../poisson-formula-for-a-holomorphic-function.md) becomes

$$
\frac1{2\pi i}\oint_{|\zeta|=R}f(\zeta)\left[\frac1{\zeta-z}-\frac1{\zeta-w}\right]d\zeta=f(z).
$$

The first term is $f(z)$ by the [Cauchy integral formula](../../../../../cauchy-integral-formula.md); the second vanishes by the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), since its pole lies outside the disk. At $z=0$ the kernel is one, and the same identity is the [mean value property for holomorphic functions](../../../../../mean-value-property-for-holomorphic-functions.md). Therefore

$$
\boxed{f(z)=\frac1{2\pi}\int_0^{2\pi}f(Re^{i\theta})\operatorname{Re}\frac{Re^{i\theta}+z}{Re^{i\theta}-z}\,d\theta\qquad(|z|<R)}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../../split.md)
6. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
