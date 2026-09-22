<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [proper convex function](../../../../../../proper-convex-function.md) $E$ on a real [Hilbert space](../../../../../../hilbert-space-split.md), its [subdifferential](../../../../../../subdifferential.md) at $y$ is

$$
\partial E(y)=\{p:E(x)\geq E(y)+\langle p,x-y\rangle\text{ for every }x\}.
$$

In a [Banach space](../../../../../../banach-space-split.md), interpret the pairing with an element of the [dual space](../../../../../../dual-space.md). For a chosen [subgradient](../../../../../../subgradient.md) $p\in\partial E(y)$, the [Bregman distance](../../../../../../bregman-divergence.md) is

$$
\boxed{D_E^p(x,y)=E(x)-E(y)-\langle p,x-y\rangle\geq0.}
$$

If also $q\in\partial E(x)$, its [symmetric Bregman distance](../../../../../../symmetric-bregman-distance.md) is

$$
\boxed{D_E^p(x,y)+D_E^q(y,x)=\langle q-p,x-y\rangle.}
$$

The [subgradient inequality](../../../../../../subgradient-inequality.md) proves nonnegativity. These quantities depend on the chosen [subgradients](../../../../../../subgradient.md) and generally are not [metrics](../../../../../../metric.md): they need not distinguish different points or obey the [triangle inequality](../../../../../../triangle-inequality.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
