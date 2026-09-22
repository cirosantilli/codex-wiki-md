<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathcal C^\infty_{\mathbb C}$ be the additive sheaf of complex-valued [smooth functions](../../../../../../smooth-function.md), and $\mathcal C^{\infty,*}_{\mathbb C}$ its multiplicative sheaf of nowhere-zero functions. The [smooth exponential sequence](../../../../../../smooth-exponential-sequence.md) is

$$
0\longrightarrow\underline{\mathbb Z}\longrightarrow\mathcal C^\infty_{\mathbb C}
\xrightarrow{f\mapsto e^{2\pi if}}\mathcal C^{\infty,*}_{\mathbb C}\longrightarrow1.
$$

Its kernel is the integer-valued locally constant functions, namely the integer [constant sheaf](../../../../../../constant-sheaf.md). It is surjective on stalks because a nowhere-zero smooth function has a smooth logarithm on a sufficiently small neighbourhood.

The additive smooth-function sheaf is a [fine sheaf](../../../../../../fine-sheaf.md), using a [partition of unity](../../../../../../partition-of-unity.md), and the [smooth manifold](../../../../../../smooth-manifold.md) is a [paracompact space](../../../../../../paracompact-space.md). Its positive-degree [sheaf cohomology](../../../../../../sheaf-cohomology.md) vanishes. The [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) consequently gives an isomorphism

$$
\delta:H^1(X,\mathcal C^{\infty,*}_{\mathbb C})\xrightarrow{\sim}H^2(X,\mathbb Z).
$$

To connect this with bundles, trivialize a smooth [complex line bundle](../../../../../../complex-line-bundle.md) over an open cover. Its transition functions $g_{ij}$ form a multiplicative [Čech cocycle](../../../../../../cech-cocycle-condition.md), satisfying $g_{ij}g_{jk}=g_{ik}$. Changing trivializations changes it by a [Čech coboundary](../../../../../../cech-coboundary.md). Conversely, any such cocycle glues trivial line bundles, and cohomologous cocycles give isomorphic bundles. Thus the isomorphism classes are $H^1(X,\mathcal C^{\infty,*}_{\mathbb C})$.

The connecting isomorphism is the [First Chern class](../../../../../../first-chern-class.md). Locally choose logarithms $g_{ij}=e^{2\pi if_{ij}}$; on triple intersections

$$
n_{ijk}=f_{ij}+f_{jk}-f_{ik}\in\mathbb Z
$$

represents that class. Combining the gluing classification with $\delta$ gives the requested bijection:

$$
\boxed{\{\text{smooth complex line bundles on }X\}/\cong\ \xrightarrow{\ c_1\ }\ H^2(X,\mathbb Z).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
