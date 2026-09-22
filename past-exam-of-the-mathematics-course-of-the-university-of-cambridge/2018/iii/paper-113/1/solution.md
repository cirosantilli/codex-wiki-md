<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [tensor product of sheaves](../../../../../tensor-product-of-sheaves.md) is the [sheafification](../../../../../sheafification.md) of the presheaf

$$
U\longmapsto\mathcal F(U)\otimes_{\mathcal O_X(U)}\mathcal G(U),
$$

with restriction maps induced by those of $\mathcal F$, $\mathcal G$, and the [structure sheaf of a scheme](../../../../../structure-sheaf-of-a-scheme.md). Sending the germ of $f\otimes g$ to $f_P\otimes g_P$ gives a canonical map

$$
(\mathcal F\otimes_{\mathcal O_X}\mathcal G)_P
\longrightarrow\mathcal F_P\otimes_{\mathcal O_{X,P}}\mathcal G_P.
$$

It is surjective because a finite sum of tensors of germs has representatives on one common neighborhood. It is injective because an equality in a [tensor product of modules](../../../../../tensor-product-of-modules.md) is witnessed by finitely many additive and balancing relations; all their germs, including the scalars in $\mathcal O_{X,P}$, can be represented and their equalities made valid on a common smaller neighborhood. Equivalently, a [filtered colimit of modules](../../../../../filtered-colimit-of-modules.md) commutes with these tensor products. Since [sheafification](../../../../../sheafification.md) preserves the [stalk of a sheaf](../../../../../stalk-of-a-sheaf.md), this proves the asserted isomorphism.

For the [pullback of a sheaf of modules](../../../../../pullback-of-a-sheaf-of-modules.md), first form the [inverse image sheaf](../../../../../inverse-image-sheaf.md) $\phi^{-1}\mathcal F$: sheafify $U\mapsto\operatorname*{colim}_{V\supseteq\phi(U)}\mathcal F(V)$. The morphism of [sheaves of rings](../../../../../sheaf-of-rings.md) $\phi^{-1}\mathcal O_Y\to\mathcal O_X$ then defines

$$
\phi^*\mathcal F=\mathcal O_X\otimes_{\phi^{-1}\mathcal O_Y}\phi^{-1}\mathcal F,
\qquad
(\phi^*\mathcal F)_P\cong\mathcal O_{X,P}\otimes_{\mathcal O_{Y,\phi(P)}}\mathcal F_{\phi(P)}.
$$

Exactness of a sequence of [sheaf of modules](../../../../../sheaf-of-modules.md) morphisms is checked on every [stalk of a sheaf](../../../../../stalk-of-a-sheaf.md). Applying the right exactness of the [tensor product of modules](../../../../../tensor-product-of-modules.md) to the stalk sequence over $\mathcal O_{Y,\phi(P)}$ gives the exact stalk sequence of the pullbacks. Thus $\phi^*$ preserves sequences ending in zero, as required.

A [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) is a [sheaf of modules](../../../../../sheaf-of-modules.md) locally of the form $\widetilde N$ for a module $N$ over the [coordinate ring](../../../../../coordinate-ring.md) of an affine neighborhood. On an [affine variety](../../../../../affine-algebraic-set.md) $V$ with ring $B$, this associated sheaf is characterized on principal opens by $\widetilde N(D(b))=N_b$, using [localization of a module](../../../../../localization-of-a-module.md). Suppose $\mathcal F|_V\cong\widetilde N$ and $U\subseteq\phi^{-1}V$ is affine, with ring $C$. The induced algebra map $B\to C$ gives a canonical map

$$
\widetilde{C\otimes_BN}\longrightarrow(\phi^*\mathcal F)|_U.
$$

At a point $P\in U$, both sides identify with $\mathcal O_{X,P}\otimes_BN$: on the right use $\mathcal F_{\phi(P)}\cong\mathcal O_{Y,\phi(P)}\otimes_BN$ and associativity of the [tensor product of modules](../../../../../tensor-product-of-modules.md). The map is therefore an isomorphism on every [stalk of a sheaf](../../../../../stalk-of-a-sheaf.md), hence an isomorphism of sheaves. Such $U$ cover $X$, proving that the pullback is a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md).

Finally, on an affine open $V\subseteq Y$ with ring $B$, the presheaf defining $M_Y$ has, on $D(b)\subseteq V$, the value

$$
M\otimes_R B_b\cong(M\otimes_RB)_b.
$$

Consequently $M_Y|_V\cong\widetilde{M\otimes_RB}$, so $M_Y$ is a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md). The algebra map for $M_X$ is the composite $R\to\Gamma(Y,\mathcal O_Y)\to\Gamma(X,\mathcal O_X)$. Restriction of functions and the tensor-product construction give a canonical sheaf morphism $\phi^*M_Y\to M_X$. At $P$, it is the associativity isomorphism

$$
\mathcal O_{X,P}\otimes_{\mathcal O_{Y,\phi(P)}}
\bigl(M\otimes_R\mathcal O_{Y,\phi(P)}\bigr)
\cong M\otimes_R\mathcal O_{X,P}.
$$

It is therefore a [sheaf of modules](../../../../../sheaf-of-modules.md) isomorphism. In particular,

$$
\boxed{(\mathcal F\otimes\mathcal G)_P\cong\mathcal F_P\otimes_{\mathcal O_{X,P}}\mathcal G_P,\qquad M_X\cong\phi^*M_Y.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 113](../../paper-113-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
