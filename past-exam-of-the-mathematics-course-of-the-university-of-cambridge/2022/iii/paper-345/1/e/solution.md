<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The incident [internal-wave ray](../../../../../../internal-wave-ray-tracing.md) has equation $z=-rx$. Intersecting it with the bottom $z=-H_0+sx$ gives

$$
x_1=\frac{H_0}{r+s}.
$$

Its distance to the slope is consequently

$$
\boxed{\ell=\frac{x_1}{\cos\theta}
=\frac{H_0}{\sin\theta+s\cos\theta}.}
$$

The subcritically reflected ray rises through the same vertical distance at angle $\theta$, so its next free-surface reflection is at

$$
\boxed{x_2=2x_1=\frac{2H_0}{r+s}.}
$$

On the first leg, [viscous attenuation of an internal-wave beam](../../../../../../viscous-attenuation-of-an-internal-wave-beam.md) multiplies the [energy density](../../../../../../energy-density.md) by $e^{-2k\ell/\operatorname{Re}}$. The bottom reflection multiplies it by $\gamma^2$ and changes the [wavenumber](../../../../../../wavenumber.md) to $\gamma k$. Since the corresponding [Reynolds number](../../../../../../reynolds-number.md) is $\operatorname{Re}/\gamma^2$, attenuation on the second leg contributes $e^{-2\gamma^3k\ell/\operatorname{Re}}$. Ignoring boundary-layer enhancement as requested,

$$
\boxed{\overline E_2=\gamma^2\overline E_0
\exp\left[-\frac{2k\ell}{\operatorname{Re}}(1+\gamma^3)\right].}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
