<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Harnack inequality on the unit disk](../../../../../../harnack-inequality-on-the-unit-disk.md) states that a nonnegative [harmonic function](../../../../../../harmonic-function.md) satisfies

$$
\frac{1-|z|}{1+|z|}u(0)\le u(z)\le\frac{1+|z|}{1-|z|}u(0).
$$

One proof applies the [Poisson integral on the unit disk](../../../../../../poisson-integral-on-the-unit-disk.md) on a circle of radius $R>|z|$: the [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md) lies between $(R-|z|)/(R+|z|)$ and its reciprocal. The [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) identifies the mean boundary value with $u(0)$; let $R\uparrow1$.

A [harmonic conjugate](../../../../../../harmonic-conjugate.md) on the [simply connected](../../../../../../simply-connected-space.md) [unit disc](../../../../../../unit-disc.md) makes $H=u+iv$ [holomorphic](../../../../../../complex-differentiability-at-a-point.md). The [Carathéodory derivative bound for the right half-plane](../../../../../../caratheodory-derivative-bound-for-the-right-half-plane.md) gives $|H'(0)|\le2u(0)$. The [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) give $|H'|=|\nabla u|$, so $|\nabla u(0)|\le2u(0)$. For a fixed $z$, use the [disk automorphism](../../../../../../automorphism-of-the-unit-disk.md)

$$
\psi(\zeta)=\frac{z+\zeta}{1+\overline z\zeta},\qquad \psi(0)=z,\qquad |\psi'(0)|=1-|z|^2.
$$

The [chain rule](../../../../../../chain-rule.md) and [conformality](../../../../../../conformality.md) multiply the [gradient](../../../../../../gradient.md) length by $|\psi'(0)|$. Applying the estimate at zero to $u\circ\psi$ proves the [sharp gradient bound for positive harmonic functions](../../../../../../sharp-gradient-bound-for-positive-harmonic-functions.md):

$$
\boxed{|\nabla u(z)|\le\frac{2}{1-|z|^2}u(z),\qquad c_{\rm best}(z)=\frac{2}{1-|z|^2}.}
$$

Sharpness follows from $u(\zeta)=\operatorname{Re}[(1+\zeta)/(1-\zeta)]$, which has equality at zero, and then composing with $\psi^{-1}$. These extremizers are positive multiples of the [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md) with its boundary pole fixed at one point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
