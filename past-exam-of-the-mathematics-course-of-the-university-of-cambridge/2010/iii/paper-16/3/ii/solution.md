<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the local-presentation definition of a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md): locally it admits a presentation $\mathcal O^{(I)}\to\mathcal O^{(J)}\to\mathcal F\to0$ by direct sums of copies of the [structure sheaf](../../../../../../structure-sheaf-of-a-scheme.md), with no finiteness requirement on the index sets. If $M$ is an $A$-[module](../../../../../../module-mathematics.md), choose a free [module](../../../../../../module-mathematics.md) presentation $A^{(I)}\to A^{(J)}\to M\to0$. Exactness of [localization of a module](../../../../../../localization-of-a-module.md) gives the corresponding local presentation of $\widetilde M$. Hence a [sheaf](../../../../../../sheaf-mathematics.md) which is associated with a [module](../../../../../../module-mathematics.md) on every [affine open subset](../../../../../../affine-open-subscheme.md) is a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md).

For the converse, begin with a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md) and a local presentation on an [affine open subset](../../../../../../affine-open-subscheme.md) $V=\operatorname{Spec}R$. The free [sheaves](../../../../../../sheaf-mathematics.md) have [global sections](../../../../../../global-section.md) $R^{(I)}$ and $R^{(J)}$: a section has locally finite support, and quasi-compactness of $V$ makes its support finite globally. Part (i) identifies the presentation map with an $R$-[module homomorphism](../../../../../../module-homomorphism.md). Exactness of [localization](../../../../../../localization-of-a-ring.md) then identifies its [cokernel sheaf](../../../../../../cokernel-sheaf.md) with $\widetilde M_V$ for the [module](../../../../../../module-mathematics.md) cokernel $M_V$. Thus there is an [affine open cover](../../../../../../affine-open-cover.md) on which $\mathcal F$ is associated with [modules](../../../../../../module-mathematics.md).

It remains to show this on an arbitrary [affine open subset](../../../../../../affine-open-subscheme.md) $U=\operatorname{Spec}A$, rather than only the selected cover. Around each point of $U$, choose an affine neighborhood contained in $U$ with such a local presentation. Choose a finite cover $U=\bigcup_{i=1}^rD(s_i)$ refining these neighborhoods. On each $D(s_i)$ the restriction is associated with a [module](../../../../../../module-mathematics.md). Its restriction to $D(s_is_j)$ is therefore the corresponding [localization](../../../../../../localization-of-a-ring.md), and the same is true after intersecting with $D(a)$. Put $M=\Gamma(U,\mathcal F)$. The [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md) gives

$$
M=\ker\left(\prod_i\Gamma(D(s_i),\mathcal F)\longrightarrow\prod_{i,j}\Gamma(D(s_is_j),\mathcal F)\right),
$$

where the arrow is the difference of the two restriction maps. [Localization of a module](../../../../../../localization-of-a-module.md) commutes with kernels and finite products. Localizing this formula at $a$ therefore gives exactly the gluing formula for $D(a)$, covered by the $D(as_i)$. Consequently

$$
M_a\simeq\Gamma(D(a),\mathcal F),
$$

compatibly with restriction. These isomorphisms on the [principal open subsets](../../../../../../principal-open-subscheme.md) identify $\widetilde M$ with $\mathcal F|_U$. We have proved the [global-section localization for quasi-coherent sheaves](../../../../../../global-section-localization-for-quasi-coherent-sheaves.md) and, in particular,

$$
\boxed{\mathcal F|_U\simeq\widetilde{\Gamma(U,\mathcal F)}\quad\text{for every affine open }U.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
