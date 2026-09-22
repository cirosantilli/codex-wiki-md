<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First apply [Lebesgue decomposition](../../../../../../lebesgue-decomposition-theorem.md) to the [derivative](../../../../../../derivative.md) [measure](../../../../../../measure.md) relative to $\mathcal L^n$:

$$
Du=D^au+D^su,\qquad D^au=\nabla u\,\mathcal L^n,\qquad D^su\perp\mathcal L^n.
$$

Here $\nabla u$ is the almost-everywhere [approximate gradient](../../../../../../approximate-gradient.md), rather than an assertion that $u$ belongs to $W^{1,1}$. Split the singular part into its [jump part of a BV derivative](../../../../../../jump-part-of-a-bv-derivative.md) and [Cantor part of a BV derivative](../../../../../../cantor-part-of-a-bounded-variation-derivative.md):

$$
\boxed{Du=\nabla u\,\mathcal L^n+(u^+-u^-)\nu_u\,\mathcal H^{n-1}\!\lfloor J_u+D^cu.}
$$

An [approximate jump point](../../../../../../approximate-jump-point.md) has a unit normal $\nu_u$ and distinct finite [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md) $u^+,u^-$, obtained as mean limits on the corresponding two half-balls. Their set $J_u$ is the [jump set of a BV function](../../../../../../jump-set-of-a-bounded-variation-function.md), countably $(n-1)$-rectifiable. Reversing the normal swaps the [BV traces on a hypersurface](../../../../../../bv-trace-on-a-hypersurface.md) and leaves the displayed [measure](../../../../../../measure.md) unchanged. The [approximate discontinuity set](../../../../../../approximate-discontinuity-set.md) $S_u$ differs from $J_u$ only by an $\mathcal H^{n-1}$-null set.

The remaining $D^cu=D^su-D^ju$ is singular to [Lebesgue measure](../../../../../../lebesgue-measure.md) and gives zero mass to every set with sigma-finite $\mathcal H^{n-1}$ [measure](../../../../../../measure.md). It is diffuse rather than a second jump contribution. In one dimension the three parts are illustrated by an [affine function](../../../../../../affine-function.md), a [step function](../../../../../../step-function.md) and the [Cantor function](../../../../../../cantor-function.md), respectively. Countably many jumps therefore do not imply that the singular [derivative](../../../../../../derivative.md) has no [Cantor part of a BV derivative](../../../../../../cantor-part-of-a-bounded-variation-derivative.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
