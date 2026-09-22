<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First form the [inverse image sheaf](../../../../../../inverse-image-sheaf.md) $\phi^{-1}\mathcal H$ by sheafifying the presheaf

$$
V\longmapsto\varinjlim_{U\supseteq\phi(V)}\mathcal H(U),
$$

where $U$ runs through [open subsets](../../../../../../open-set.md) of $X$. It is naturally a [module](../../../../../../module-mathematics.md) over $\phi^{-1}\mathcal O_X$, not yet over $\mathcal O_Y$. The structure morphism $\phi^{-1}\mathcal O_X\to\mathcal O_Y$ allows extension of scalars, giving the [pullback of a sheaf of modules](../../../../../../pullback-of-a-sheaf-of-modules.md):

$$
\boxed{\phi^*\mathcal H
=\mathcal O_Y\otimes_{\phi^{-1}\mathcal O_X}\phi^{-1}\mathcal H}.
$$

The [tensor product of sheaves](../../../../../../tensor-product-of-sheaves.md) includes its own [sheafification](../../../../../../sheafification.md). At $Q\in Y$ the construction becomes

$$
(\phi^*\mathcal H)_Q
=\mathcal O_{Y,Q}\otimes_{\mathcal O_{X,\phi(Q)}}\mathcal H_{\phi(Q)}.
$$

This adjustment of the coefficient ring distinguishes the pullback from the underlying [inverse image sheaf](../../../../../../inverse-image-sheaf.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
