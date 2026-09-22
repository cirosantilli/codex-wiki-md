<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Vary the [scalar field](../../../../../../scalar-field.md) with compactly supported variation, leaving the [metric tensor](../../../../../../metric-tensor.md) fixed. The [action](../../../../../../action.md) variation is

$$
\delta S_M=\int d^4x\sqrt{-g}
\left[-g^{\mu\nu}\partial_\mu\phi\,\partial_\nu\delta\phi-V_{,\phi}\delta\phi\right].
$$

[Integration by parts](../../../../../../integration-by-parts.md) moves the derivative from $\delta\phi$ and gives the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
\Box_g\phi-V_{,\phi}=0,\qquad
\Box_g\phi=\frac1{\sqrt{-g}}\partial_\mu\left(\sqrt{-g}\,g^{\mu\nu}\partial_\nu\phi\right).
$$

For the [FRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md), $\sqrt{-g}=a^3$, so the [covariant wave operator](../../../../../../covariant-wave-operator.md) becomes

$$
\Box_g\phi=-a^{-3}\partial_t(a^3\dot\phi)+a^{-2}\nabla^2\phi
=-\ddot\phi-3H\dot\phi+a^{-2}\nabla^2\phi.
$$

Rearranging gives the requested [scalar field](../../../../../../scalar-field.md) evolution:

$$
\boxed{\ddot\phi+3\frac{\dot a}{a}\dot\phi-a^{-2}\nabla^2\phi=-V_{,\phi}.}
$$

The damping term is [Hubble friction](../../../../../../hubble-friction.md); it comes from the expanding volume factor $a^3$, not from a microscopic dissipative force.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
