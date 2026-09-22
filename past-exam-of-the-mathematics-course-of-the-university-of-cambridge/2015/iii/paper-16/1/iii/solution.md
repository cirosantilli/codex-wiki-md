<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First form the [inverse image sheaf](../../../../../../inverse-image-sheaf.md) $\phi^{-1}\mathcal H$ by applying [sheafification](../../../../../../sheafification.md) to

$$
U\longmapsto\varinjlim_{V\supseteq\phi(U)}\mathcal H(V).
$$

It is a [sheaf of modules](../../../../../../sheaf-of-modules.md) over $\phi^{-1}\mathcal O_Y$. The [morphism of ringed spaces](../../../../../../morphism-of-ringed-spaces.md) gives a ring map $\phi^{-1}\mathcal O_Y\to\mathcal O_X$, so the [pullback of a sheaf of modules](../../../../../../pullback-of-a-sheaf-of-modules.md) is

$$
\boxed{\phi^*\mathcal H=\mathcal O_X\otimes_{\phi^{-1}\mathcal O_Y}\phi^{-1}\mathcal H.}
$$

At $x\in X$, writing $y=\phi(x)$, its [stalk](../../../../../../stalk-of-a-sheaf.md) is $\mathcal O_{X,x}\otimes_{\mathcal O_{Y,y}}\mathcal H_y$. The tensor construction makes the action of the [structure sheaf](../../../../../../structure-sheaf-of-a-scheme.md) explicit; taking the inverse image alone would not give the requested $\mathcal O_X$-module.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
