<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Wirtinger derivatives](../../../../../../wirtinger-derivatives.md) $\partial_z=(\partial_x-i\partial_y)/2$ and $\partial_{\bar z}=(\partial_x+i\partial_y)/2$, and area measure $dA=dx\,dy=(i/2)dz\wedge d\bar z$. The supplied boundary-integral identity is the planar [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md); the usual [Poincaré lemma](../../../../../../poincare-lemma.md) is a different local exactness result.

Let $f\in C^1(\overline D)$ and $z\in D$. Remove a disk of radius $\epsilon$ around $z$, and apply [Generalized Stokes theorem](../../../../../../generalized-stokes-theorem.md) to the [one-form](../../../../../../one-form.md) $f(\zeta)d\zeta/(\zeta-z)$ on the punctured domain. Away from the puncture,

$$
d\left(\frac{f(\zeta)}{\zeta-z}d\zeta\right)
=\frac{f_{\bar\zeta}(\zeta)}{\zeta-z}\,d\bar\zeta\wedge d\zeta
=2i\frac{f_{\bar\zeta}(\zeta)}{\zeta-z}\,dA(\zeta).
$$

The outer boundary is counterclockwise and the small inner circle clockwise. Its counterclockwise integral tends to $2\pi i f(z)$. Passing to the limit gives the [Cauchy-Pompeiu formula](../../../../../../cauchy-pompeiu-formula.md)

$$
\boxed{f(z)=\frac1{2\pi i}\int_{\partial D}\frac{f(\zeta)}{\zeta-z}\,d\zeta
-\frac1\pi\int_D\frac{f_{\bar\zeta}(\zeta)}{\zeta-z}\,dA(\zeta).}
$$

The weak $1/|\zeta-z|$ singularity is locally integrable. If the boundary term vanishes on expanding $D$ to the whole plane, the formula becomes $f(z)=\pi^{-1}\int_{\mathbb C}f_{\bar\zeta}(\zeta)/(z-\zeta)\,dA(\zeta)$. In particular it yields the distributional normalization $\partial_{\bar z}[1/(\pi z)]=\delta_0$. For [holomorphic functions](../../../../../../holomorphic-function.md) the area term vanishes and one recovers the [Cauchy integral formula](../../../../../../cauchy-integral-formula.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
