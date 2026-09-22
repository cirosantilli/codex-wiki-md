<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix a non-Archimedean [local field](../../../../../local-field.md) $K$, write $Q=|k_K|$, and use the **arithmetic Frobenius normalization** throughout: a [uniformizer](../../../../../uniformizer.md) maps to the automorphism inducing $a\mapsto a^Q$ on the [maximal unramified extension](../../../../../maximal-unramified-extension.md). The [Local Artin map](../../../../../local-artin-map.md), or [local reciprocity map](../../../../../local-artin-map.md), is the canonical continuous [group homomorphism](../../../../../group-homomorphism.md)

$$
\operatorname{Art}_K:K^\times\longrightarrow\operatorname{Gal}(K^{\mathrm{ab}}/K),
$$

where $K^{\mathrm{ab}}$ is the [maximal abelian extension](../../../../../maximal-abelian-extension.md) inside a fixed [algebraic closure](../../../../../algebraic-closure.md) with its separable part understood. Its finite projection to every finite abelian extension $L/K$ is onto and has kernel exactly the [norm subgroup of a local field extension](../../../../../norm-subgroup-of-a-local-field-extension.md):

$$
\boxed{K^\times/N_{L/K}(L^\times)\xrightarrow{\sim}\operatorname{Gal}(L/K).}
$$

In particular, the quotient has order $[L:K]$. This is how [local class field theory](../../../../../local-class-field-theory.md) turns abelian extension problems into computations inside a multiplicative group.

One precise definition of the finite reciprocity map uses the [cup-product construction of local reciprocity](../../../../../cup-product-construction-of-local-reciprocity.md). For a finite [Galois extension](../../../../../finite-galois-extension.md) with group $G$, the [local fundamental class](../../../../../local-fundamental-class.md) $u_{L/K}\in H^2(G,L^\times)$ is specified by [local Brauer invariant](../../../../../local-brauer-invariant.md) $1/[L:K]$. [Cup product](../../../../../cup-product.md) gives an isomorphism

$$
\widehat H^{-2}(G,\mathbb Z)=G^{\mathrm{ab}}
\xrightarrow{\ \smile u_{L/K}\ }
\widehat H^0(G,L^\times)=K^\times/N_{L/K}(L^\times).
$$

The finite [Local Artin map](../../../../../local-artin-map.md) is its inverse, composed with the quotient map from $K^\times$. For abelian $G$ the target is $G$ itself. Taking the compatible [inverse limit](../../../../../inverse-limit.md) over finite abelian extensions defines $\operatorname{Art}_K$.

The essential inputs to this cohomological construction have concrete arithmetic content. The [local Brauer invariant](../../../../../local-brauer-invariant.md) identifies $\operatorname{Br}(K)$ with $\mathbb Q/\mathbb Z$; restriction to $L$ multiplies the invariant by $[L:K]$, so its kernel is cyclic of that order and has the distinguished generator $u_{L/K}$. For every subgroup $H\subseteq G$, [Hilbert theorem 90](../../../../../hilbert-s-theorem-90.md) gives $H^1(H,L^\times)=0$, while the same invariant calculation over the fixed field gives $H^2(H,L^\times)$ cyclic of order $|H|$. These are the hypotheses of the algebraic cup-product isomorphism in [Tate cohomology of a finite group](../../../../../tate-cohomology-of-a-finite-group.md). It is obtained by [dimension shifting in group cohomology](../../../../../dimension-shifting-in-group-cohomology.md) with a [projective resolution](../../../../../projective-resolution.md) of the trivial module and the extension representing the fundamental class. Thus the norm-kernel statement comes from the degree-zero definition of [Tate cohomology of a finite group](../../../../../tate-cohomology-of-a-finite-group.md), rather than from an arbitrary assignment of an automorphism to each element. In an [unramified extension](../../../../../unramified-extension.md) of degree $d$, the fundamental class is the [cyclic algebra](../../../../../cyclic-algebra.md) with [arithmetic Frobenius](../../../../../frobenius-automorphism.md) generator and parameter a [uniformizer](../../../../../uniformizer.md); the isomorphism sends that Frobenius to the class of the uniformizer. This explains the chosen sign of reciprocity.

Several properties follow immediately from this construction. If $L\supseteq E\supseteq K$ are finite abelian extensions, restricting $\operatorname{Art}_{L/K}(a)$ to $E$ gives $\operatorname{Art}_{E/K}(a)$. The [Local Artin map](../../../../../local-artin-map.md) is therefore compatible with the finite projections defining its infinite target. For any finite separable extension $E/K$ and $a\in E^\times$, its norm compatibility is

$$
\operatorname{Art}_K(N_{E/K}a)=\operatorname{Art}_E(a)|_{K^{\mathrm{ab}}}.
$$

Here $K^{\mathrm{ab}}E/E$ is abelian, so the displayed restriction makes sense. An outline of the compatibility proof is to use the [corestriction map in group cohomology](../../../../../corestriction-map-in-group-cohomology.md): on multiplicative coefficients its degree-zero map is the norm. The cup-product projection formula, together with restriction and corestriction of the [local fundamental class](../../../../../local-fundamental-class.md), gives exactly the commuting reciprocity diagram. The compatibility is an arithmetic instance of the functoriality of the cohomological definition.

The [Local Artin map](../../../../../local-artin-map.md) has dense image, because every finite abelian quotient receives a surjective map. Its kernel is trivial, and it extends to an isomorphism

$$
\boxed{\widehat{K^\times}\simeq\operatorname{Gal}(K^{\mathrm{ab}}/K),}
$$

where this [profinite completion](../../../../../profinite-completion.md) uses the open finite-index subgroups of the topological multiplicative group. The original map is generally not onto: on the unramified quotient it sends the integer valuation into $\widehat{\mathbb Z}$, rather than producing every profinite integer. Its units map onto the abelian [inertia group](../../../../../inertia-group.md). For a finite abelian extension, the corresponding unit image is its [inertia group](../../../../../inertia-group.md), while the valuation accounts for its residue extension. Indeed $v_K(Nz)=f(L/K)v_L(z)$, so the valuation quotient has order $f$; the full norm quotient has order $ef$, leaving unit image of order $e$. Since unit images act trivially on the residue field, they give precisely the [inertia group](../../../../../inertia-group.md). More finely, the image of the [higher principal-unit group](../../../../../higher-principal-unit-group.md) $1+\mathfrak m_K^r$ in a finite abelian extension is its rth upper [ramification group](../../../../../ramification-group.md), for each integer $r\geq1$. The use of [upper ramification numbering](../../../../../upper-ramification-numbering.md) is essential for compatibility with quotients.

The [existence theorem of local class field theory](../../../../../existence-theorem-of-local-class-field-theory.md) states that every open finite-index subgroup $H\subseteq K^\times$ is $N_{L/K}(L^\times)$ for a unique finite abelian extension $L/K$. Inclusions are reversed: larger extensions have smaller norm subgroups. In the established reciprocity isomorphism, the proof is simply to take the fixed field of the open subgroup corresponding to $H$. Conversely a finite extension gives an open kernel of a finite continuous projection. Uniqueness follows because that kernel specifies its fixed field. The substantive existence problem is therefore to prove that the reciprocity isomorphism realizes all open finite-index subgroups; it is not just this final fixed-field argument.

The [Lubin–Tate description of local reciprocity](../../../../../lubin-tate-description-of-local-reciprocity.md) provides an explicit route to that existence problem. Choose a [uniformizer](../../../../../uniformizer.md) $\pi$ and a [Lubin–Tate series](../../../../../lubin-tate-series.md) $f(T)=\pi T+T^Q$, with its associated [Lubin–Tate formal group](../../../../../lubin-tate-formal-group.md) $F$. Solving $f(F(X,Y))=F(f(X),f(Y))$ successively by total degree constructs the law with linear part $X+Y$; the analogous equations construct the endomorphisms $[a]$ with linear coefficient $a$. The congruence $f(T)\equiv T^Q\pmod\pi$ supplies the divisibility needed at each step. These endomorphisms satisfy $[a][b]=[ab]$ and make the torsion an $\mathcal O_K$-module.

If $f_r$ denotes the rfold iterate, the primitive level-r [Lubin–Tate torsion](../../../../../lubin-tate-torsion.md) points are roots of

$$
\frac{f_r(T)}{f_{r-1}(T)}=\pi+f_{r-1}(T)^{Q-1}.
$$

Reduction modulo $\pi$ is $T^{Q^{r-1}(Q-1)}$, and the constant term is $\pi$, so this is an [Eisenstein polynomial](../../../../../eisenstein-polynomial.md). Its roots therefore generate a [totally ramified extension](../../../../../totally-ramified-extension.md) $K_{\pi,r}$ of degree $(Q-1)Q^{r-1}$. A primitive point generates the entire torsion module, and all points are its images under the integral convergent endomorphisms $[a]$. The torsion field is therefore a [Galois extension](../../../../../finite-galois-extension.md) of $K$. The action map into $(\mathcal O_K/\pi^r)^\times$ is injective, and the computed degree equals the order of this unit group, proving it is an isomorphism. Passing to the [inverse limit](../../../../../inverse-limit.md) gives $\operatorname{Gal}(K_\pi/K)\simeq\mathcal O_K^\times$ for the [Lubin–Tate tower](../../../../../lubin-tate-tower.md) $K_\pi$.

The unramified tower and $K_\pi$ are [linearly disjoint field extensions](../../../../../linear-disjointness.md): a finite common subextension would be both unramified and totally ramified, hence trivial. The [Lubin–Tate description of local reciprocity](../../../../../lubin-tate-description-of-local-reciprocity.md) on their compositum is

$$
\operatorname{Art}_K(\pi^m u)|_{K^{\mathrm{nr}}}=\operatorname{Frob}_K^m,\qquad
\operatorname{Art}_K(\pi^m u)(\lambda)=[u^{-1}](\lambda)\quad(\lambda\in F[\pi^r]).
$$

The inverse on the unit action goes with the arithmetic Frobenius convention; changing to geometric Frobenius inverts the whole reciprocity map. The reciprocity theorem identifies this explicit action with the finite cup-product maps, independently of the chosen uniformizer. Its proof compares the fundamental class with the norm relations between consecutive torsion fields. The construction makes the possible finite kernels concrete: on the compositum of the degree-d unramified field with $K_{\pi,r}$ the kernel is

$$
\pi^{d\mathbb Z}(1+\pi^r\mathcal O_K).
$$

These subgroups are cofinal among open finite-index subgroups. Indeed any such $H$ contains $1+\pi^r\mathcal O_K$ for sufficiently large $r$, and contains $\pi^d$ for some positive $d$, since the class of $\pi$ in $K^\times/H$ has finite order. Taking the appropriate fixed subgroup in this explicit finite compositum realizes $H$. This proves the open-subgroup part of existence once the norm compatibility of the explicit and cohomological constructions is established. Together with the finite reciprocity maps it also shows that $K^{\mathrm{ab}}=K^{\mathrm{nr}}K_\pi$.

As a direct check, on a finite unramified extension the construction reduces to

$$
\operatorname{Art}_{L/K}(a)=\phi_{L/K}^{\,v_K(a)}.
$$

The earlier elementary unit-norm proof shows its kernel is exactly $\pi^{d\mathbb Z}\mathcal O_K^\times$. At $K=\mathbb Q_p$, the [Lubin–Tate cyclotomic example](../../../../../lubin-tate-cyclotomic-example.md) takes $[p](T)=(1+T)^p-1$ and $F(X,Y)=X+Y+XY$. Its torsion is $\zeta-1$, so a unit $u$ acts by $\zeta\mapsto\zeta^{u^{-1}}$. These examples exhibit both the valuation and unit parts of local reciprocity with consistent signs.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
