<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With an [absorbing boundary condition for a diffusion](../../../../../../absorbing-boundary-condition-for-a-diffusion.md) on each vertical side, the [splitting probability](../../../../../../splitting-probability.md) $u(x)$ of hitting the left side before the right is harmonic for the [Kolmogorov backward equation](../../../../../../kolmogorov-backward-equation.md):

$$
u''+a_1u'=0,\qquad
u(-1)=1,\quad u(1)=0.
$$

For $a_1\neq0$,

$$
u(x)=\frac{e^{-a_1x}-e^{-a_1}}
{e^{a_1}-e^{-a_1}}.
$$

The particle starts at $x=0$, so

$$
\boxed{
g(a_1)=u(0)
=\frac{1-e^{-a_1}}{e^{a_1}-e^{-a_1}}
=\frac1{1+e^{a_1}}.
}
$$

The continuous limit at zero is $g(0)=1/2$, as required by reflection symmetry. A large positive drift drives the particle toward the right and gives $g(a_1)\to0$; a large negative drift drives it toward the left and gives $g(a_1)\to1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
