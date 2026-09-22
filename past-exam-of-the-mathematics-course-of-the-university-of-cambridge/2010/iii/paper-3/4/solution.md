<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $K=Q(A)$ be the [fraction field](../../../../../field-of-fractions.md) of the [integral domain](../../../../../integral-domain.md) $A$. The [Picard group of a ring](../../../../../picard-group-of-a-ring.md) consists of isomorphism classes of finitely generated [projective modules](../../../../../projective-module.md) that have rank one after localization at every [prime ideal](../../../../../prime-ideal.md). Its product is induced by the [tensor product of modules](../../../../../tensor-product-of-modules.md), its identity is $[A]$, and the inverse of $[L]$ is $[L^\vee]$, where $L^\vee=\operatorname{Hom}_A(L,A)$. Evaluation $L\otimes_AL^\vee\to A$ is an isomorphism: after localization it is evaluation on a free rank-one module, and a map whose kernel and cokernel vanish at every prime is an isomorphism.

An [invertible fractional ideal](../../../../../invertible-fractional-ideal.md) is a nonzero finitely generated $A$-submodule $I\subseteq K$ admitting another fractional ideal $J$ with $IJ=A$. The [Cartier divisors](../../../../../cartier-divisor-split.md) of $\operatorname{Spec}A$ can be represented by these ideals. Concretely a [Cartier divisor](../../../../../cartier-divisor-split.md) has local nonzero rational equations $f_i$ on a cover by distinguished open sets, with $f_i/f_j$ a regular unit on each overlap. We use the convention assigning to it $\mathcal O(-D)$, whose local fractional ideals are $f_iA_{s_i}$. Their unit ratios make these modules agree on overlaps. Thus the [Cartier divisor](../../../../../cartier-divisor-split.md) group $\operatorname{Cart}(A)$ is realized by [invertible fractional ideals](../../../../../invertible-fractional-ideal.md) with multiplication. The identity is $A$ and a [principal Cartier divisor](../../../../../principal-cartier-divisor.md) of $f\in K^\times$ corresponds to $fA$.

To check explicitly that local divisor data give an [invertible fractional ideal](../../../../../invertible-fractional-ideal.md), set $I=\bigcap_i f_iA_{s_i}\subseteq K$. Take a finite distinguished-open cover; this is possible because an affine spectrum is quasi-compact. On an overlap, $f_i/f_j\in A_{s_is_j}$. For each fixed $i$, clear the powers of $s_i$ in these finitely many expressions: there is $N_i$ with $s_i^{N_i}f_i\in f_jA_{s_j}$ for every $j$. Thus $t_i=s_i^{N_i}f_i$ belongs to $I$, and $I_{s_i}=f_iA_{s_i}$. The finite module $J=\sum_iAt_i$ has the same localizations, so $I/J$ vanishes on the cover and $I=J$. Repeating with $f_i^{-1}$ gives a finitely generated fractional ideal $I'$ with $I'_{s_i}=f_i^{-1}A_{s_i}$. Therefore $II'$ is contained in $A$ and equals $A$ after localization on the cover, whence $II'=A$. These conclusions use the elementary localization test proved below. Conversely, the next argument constructs precisely such a finite principal cover from an inverse ideal. Thus the local-divisor and ideal descriptions agree, without assuming that $A$ is Noetherian.

Here is the algebra underlying that realization and the map to the [Picard group](../../../../../picard-group.md). If $IJ=A$, write $1=\sum_{i=1}^r u_iv_i$, with $u_i\in I$ and $v_i\in J$. On the distinguished open where $s_i=u_iv_i$ is invertible, $I_{s_i}=u_iA_{s_i}$: for any $x\in I$, the expression

$$
\frac{x}{u_i}=\frac{xv_i}{u_iv_i}
$$

is in $A_{s_i}$. These open sets cover the spectrum because $\sum s_i=1$. The generators on overlaps differ by units. Moreover the maps $\phi_i:I\to A$, $\phi_i(x)=v_ix$, satisfy $x=\sum u_i\phi_i(x)$. Consequently the composite

$$
I\xrightarrow{x\mapsto(\phi_i(x))}A^r
\xrightarrow{(a_i)\mapsto\sum a_iu_i}I
$$

is the identity. This explicitly makes $I$ a direct summand of a finite [free module](../../../../../free-module.md), and hence a [projective module](../../../../../projective-module.md), with rank one locally.

Its inverse is

$$
I^{-1}=\{v\in K:vI\subseteq A\}=J.
$$

The inclusion $J\subseteq I^{-1}$ follows from $IJ=A$. For the other inclusion, $v\in I^{-1}$ gives $v=\sum(vu_i)v_i\in J$. Local multiplication is an isomorphism between free rank-one modules, so multiplication $I\otimes_AJ\to IJ$ is an isomorphism. In particular $I\mapsto[I]$ respects the group laws.

Conversely, suppose $L$ is a finitely generated [projective module](../../../../../projective-module.md) of rank one. It is a direct summand of a finite [free module](../../../../../free-module.md), so it is torsion-free and injects into $L\otimes_AK$. The latter is a one-dimensional $K$-space. Choose a basis to identify it with $K$, and let $I$ be the image of $L$. Its finitely many generators have a common nonzero denominator, making $I$ a fractional ideal. Every $A$-linear map $I\to A$ extends to a $K$-linear map $K\to K$, which is multiplication by some $v\in K$. Thus $I^\vee$ identifies with $I^{-1}$. Evaluation is an isomorphism locally, so its image ideal $II^{-1}$ localizes to $A_{\mathfrak p}$ at every prime. A proper ideal would be contained in a maximal ideal, contradicting that localization; hence $II^{-1}=A$. This proves that every [Picard group](../../../../../picard-group.md) class has an [invertible fractional ideal](../../../../../invertible-fractional-ideal.md) representative, and also that locally principal fractional ideals on a finite open cover are invertible.

For completeness, these local tests do detect a zero module without a finite-generation assumption. If $0\ne x\in N$, its annihilator is proper; choose a maximal ideal containing it. Then $x/1$ is nonzero in that localization, since any denominator killing $x$ would belong to its annihilator. Applying this observation to a kernel and cokernel justifies the local isomorphism tests above.

The natural maps in the [Cartier divisor exact sequence for an integral domain](../../../../../cartier-divisor-exact-sequence-for-an-integral-domain.md) are now

$$
A^\times\hookrightarrow K^\times,\qquad
K^\times\longrightarrow\operatorname{Cart}(A),\quad f\longmapsto fA,
\qquad \operatorname{Cart}(A)\longrightarrow\operatorname{Pic}(A),\quad I\longmapsto[I].
$$

The first map is injective. The ideal $fA$ is the identity divisor $A$ precisely when $f$ and $f^{-1}$ lie in $A$, that is, precisely when $f\in A^\times$. Next $[I]=[A]$ precisely when some isomorphism $A\to I$ sends $1$ to an element $f\in K^\times$ generating $I$, so $I=fA$. Finally the construction from $L$ proves surjectivity onto the [Picard group](../../../../../picard-group.md). We have therefore checked exactness at every term:

$$
\boxed{1\longrightarrow A^\times\longrightarrow K^\times
\longrightarrow\operatorname{Cart}(A)\longrightarrow\operatorname{Pic}(A)\longrightarrow0.}
$$

No Noetherian, normality or factoriality hypothesis is required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
