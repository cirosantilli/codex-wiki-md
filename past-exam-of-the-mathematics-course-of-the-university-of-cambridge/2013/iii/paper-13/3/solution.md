<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The point to retain in the direct-image theorem is [quasi-compactness](../../../../../compact-space.md) of inverse images of affine opens and of overlaps; no separation assumption has been supplied. The underlying space of a [Noetherian scheme](../../../../../noetherian-scheme.md) is Noetherian, so every [open subset](../../../../../open-set.md) of $X$ is [quasi-compact](../../../../../compact-space.md). Fix an [affine open subscheme](../../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A$ of $Y$, put $W=f^{-1}V$, and choose a finite [open cover](../../../../../open-cover.md) by [affine open subschemes](../../../../../affine-open-subscheme.md) $W=\bigcup_i U_i$. For each pair $i,j$, choose a finite affine cover $(W_{ij\ell})_\ell$ of $U_i\cap U_j$. Empty overlaps contribute no terms.

Write $M=\Gamma(W,\mathcal F)$. The [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) gives the [exact sequence](../../../../../exact-sequence.md)

$$
0\longrightarrow M\longrightarrow
\prod_i\Gamma(U_i,\mathcal F)
\xrightarrow{\delta}
\prod_{i,j,\ell}\Gamma(W_{ij\ell},\mathcal F),
$$

where $\delta$ is the difference of the two restrictions to each overlap chart. All terms are $A$-[modules](../../../../../module-mathematics.md) through $f$. For $a\in A$, the inverse image of $D(a)$ cuts each $U_i$ and $W_{ij\ell}$ by a [principal open subscheme](../../../../../principal-open-subscheme.md). Because $\mathcal F$ is a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md), sections on these smaller affine charts are the corresponding [module localizations](../../../../../localization-of-a-module.md) at $a$. [Exactness of localization](../../../../../exactness-of-localization.md) and its commutation with finite products now identify the localized equalizer with the equalizer for the restricted cover. Thus

$$
\Gamma(f^{-1}D(a),\mathcal F)\cong M_a.
$$

The isomorphisms respect restrictions, proving $(f_*\mathcal F)|_V\cong\widetilde M$ on the basis of [principal open subschemes](../../../../../principal-open-subscheme.md). Since $V$ was arbitrary, **$f_*\mathcal F$ is a quasi-coherent sheaf**. The finite covers of overlaps are what allow the proof to work for nonseparated [Noetherian schemes](../../../../../noetherian-scheme.md); this is the [quasi-coherence of direct image under a quasi-compact quasi-separated morphism](../../../../../quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism.md).

For a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) which is not coherent but has coherent [direct image](../../../../../direct-image-sheaf.md), use $f:\mathbb P^1_k\to\operatorname{Spec}k$ and

$$
\mathcal F=\bigoplus_{n=1}^{\infty}\mathcal O_{\mathbb P^1}(-1).
$$

This [infinite negative-twist sum with zero global sections](../../../../../infinite-negative-twist-sum-with-zero-global-sections.md) is quasi-coherent: on each standard [affine chart](../../../../../affine-chart-of-a-variety.md) it is the sheaf associated with a direct sum of free rank-one [modules](../../../../../module-mathematics.md). Its [stalk](../../../../../stalk-of-a-sheaf.md) at every point, modulo the [maximal ideal](../../../../../maximal-ideal.md), is an infinite-dimensional [vector space](../../../../../vector-space-split.md). A finitely generated [module](../../../../../module-mathematics.md) would have a finite-dimensional quotient, so $\mathcal F$ is not a [coherent sheaf](../../../../../coherent-sheaf.md).

Nevertheless, $\Gamma(\mathbb P^1,\mathcal O(-1))=0$. This follows from [cohomology of twisting sheaves on projective space](../../../../../cohomology-of-twisting-sheaves-on-projective-space.md), or directly by gluing on the two standard affine charts: if $z=t_1/t_0$, a section is a polynomial $p(z)$ on the first chart and $q(z^{-1})$ on the second with $p(z)=z^{-1}q(z^{-1})$, which forces both to vanish. [Global sections](../../../../../global-section.md) commute with this direct sum: they are the kernel of the difference map for the two-chart cover, and [direct sums](../../../../../direct-sum.md) commute with that finite equalizer of [modules](../../../../../module-mathematics.md). Hence

$$
\boxed{f_*\mathcal F=0,}
$$

which is coherent on $\operatorname{Spec}k$. Both [schemes](../../../../../scheme.md) in this example are Noetherian.

For a [finite morphism](../../../../../finite-morphism.md), such an example is impossible. On an [affine open subscheme](../../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A$ of the target, its inverse image is $\operatorname{Spec}B$, with $B$ a finite $A$-[module](../../../../../module-mathematics.md). Write $\mathcal F|_{f^{-1}V}=\widetilde M$. Its [direct image](../../../../../direct-image-sheaf.md) corresponds to $M$ considered as an $A$-[module](../../../../../module-mathematics.md). If the [direct image](../../../../../direct-image-sheaf.md) is coherent, $M$ is finitely generated over $A$. The same generators also generate it over $B$, because $A$ acts through $B$. Since $B$ is Noetherian, $\widetilde M$ is coherent. Conversely, a finite set of $B$-generators combined with a finite set of $A$-generators of $B$ gives finitely many $A$-generators of $M$. Thus [coherence reflected by finite direct image](../../../../../coherence-reflected-by-finite-direct-image.md) gives the stronger equivalence

$$
\boxed{\mathcal F\text{ coherent}\iff f_*\mathcal F\text{ coherent}
\quad(f\text{ finite}).}
$$

Finally, let $Y=\operatorname{Spec}k[x,y]$, let $X=Y\setminus\{(x,y)\}$ be the [punctured affine plane](../../../../../punctured-affine-plane.md), and let $j:X\hookrightarrow Y$ be the [open immersion](../../../../../open-immersion.md). Both are [integral schemes](../../../../../integral-scheme.md), but $j$ is not an [isomorphism of schemes](../../../../../isomorphism-of-schemes.md) because it omits a point. The cover $X=D(x)\cup D(y)$ gives

$$
\Gamma(X,\mathcal O_X)
=k[x,y]_x\cap k[x,y]_y=k[x,y]
$$

inside the [field of fractions](../../../../../field-of-fractions.md) $k(x,y)$. Indeed, in a reduced fraction, membership in the first [localization](../../../../../localization-of-a-ring.md) forces every denominator factor to be associated to $x$, while membership in the second forces it to be associated to $y$. [Unique factorization](../../../../../unique-factorization-in-an-integral-domain.md) and coprimality force the denominator to be a [unit](../../../../../unit-in-a-ring.md). By the theorem just proved, $j_*\mathcal O_X$ is quasi-coherent on the affine $Y$, hence determined by this [module](../../../../../module-mathematics.md) of [global sections](../../../../../global-section.md). The natural map $\mathcal O_Y\to j_*\mathcal O_X$ corresponds to the identity of $k[x,y]$, so

$$
\boxed{j_*\mathcal O_X\cong\mathcal O_Y,}
$$

a [coherent sheaf](../../../../../coherent-sheaf.md). This is a concrete case of [codimension-two extension of regular functions on a normal variety](../../../../../codimension-two-extension-of-regular-functions-on-a-normal-variety.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
