<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $P=\mathbb P^2_k$ and $S=k[t_0,t_1,t_2]$. A homogeneous polynomial $F$ of positive degree $d$ is nonzero, and $S$ is an [integral domain](../../../../../../integral-domain.md). Multiplication by $F$ therefore gives an exact sequence of [coherent sheaves](../../../../../../coherent-sheaf.md)

$$
0\longrightarrow\mathcal O_P(-d)\xrightarrow{\ F\ }\mathcal O_P\longrightarrow i_*\mathcal O_X\longrightarrow0,
$$

where $i:X\hookrightarrow P$ is the [closed immersion](../../../../../../closed-immersion.md).

We compute the necessary [cohomology of twisting sheaves on projective space](../../../../../../cohomology-of-twisting-sheaves-on-projective-space.md). The standard three [affine open subsets](../../../../../../affine-open-subscheme.md) $D_+(t_i)$ and all their intersections are [affine schemes](../../../../../../affine-scheme.md). For a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md), [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) and the [acyclic cover theorem](../../../../../../leray-s-theorem.md) identify its [sheaf cohomology](../../../../../../sheaf-cohomology.md) with the [Čech cohomology](../../../../../../cech-cohomology.md) of this cover. In degree $m$, the [Čech cochain complex](../../../../../../cech-cochain-complex.md) is

$$
\bigoplus_i(S_{t_i})_m\longrightarrow\bigoplus_{i<j}(S_{t_it_j})_m\longrightarrow(S_{t_0t_1t_2})_m.
$$

Decompose it into subcomplexes indexed by Laurent monomials $t_0^{a_0}t_1^{a_1}t_2^{a_2}$ with $a_0+a_1+a_2=m$. Let $N=\{i:a_i<0\}$. Such a monomial occurs in the summand for a nonempty index set $J$ precisely when $N\subseteq J$, since only the variables in $J$ are inverted.

If $N$ is empty, the monomial contributes the cochain complex of a full two-simplex: its degree-zero cohomology is $k$ and its higher cohomology vanishes. If $|N|=1$, the dimensions in degrees $0,1,2$ are $1,2,1$; the first map has rank one and the second map has rank one with the same kernel as the first map's image. If $|N|=2$, there is one copy of $k$ in each of degrees $1$ and $2$ and the map between them is an isomorphism. These two cases are acyclic over every [field](../../../../../../field.md), including characteristic two. If $N=\{0,1,2\}$, only the degree-two term occurs, contributing one copy of $k$. It follows that

$$
H^1(P,\mathcal O_P(m))=0\quad\text{for every }m,
$$

and that $H^0(P,\mathcal O_P)=k$, $H^0(P,\mathcal O_P(-d))=0$, and $H^2(P,\mathcal O_P)=0$. Moreover the [Laurent-monomial description of top cohomology on projective space](../../../../../../laurent-monomial-description-of-top-cohomology-on-projective-space.md) gives a basis of $H^2(P,\mathcal O_P(-d))$ consisting of

$$
t_0^{-b_0}t_1^{-b_1}t_2^{-b_2},\qquad b_i\geq1,\quad b_0+b_1+b_2=d.
$$

For $d\geq3$, subtracting one from each $b_i$ counts these as $\binom{d-1}{2}$. For $d=1,2$ there are no such triples, and the formula $(d-1)(d-2)/2$ is also zero.

Use the [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) of the initial sequence, and [cohomology under a closed immersion](../../../../../../cohomology-under-a-closed-immersion.md) to identify the terms for $i_*\mathcal O_X$. The vanishings just proved give

$$
H^0(X,\mathcal O_X)\simeq k,\qquad H^1(X,\mathcal O_X)\simeq H^2(P,\mathcal O_P(-d)).
$$

Therefore

$$
\boxed{\dim_kH^0(X,\mathcal O_X)=1,\qquad\dim_kH^1(X,\mathcal O_X)=\frac{(d-1)(d-2)}2.}
$$

This proves the [cohomology of a projective plane hypersurface](../../../../../../cohomology-of-a-projective-plane-hypersurface.md) without imposing smoothness, irreducibility or reducedness. In particular, the second number is an [arithmetic genus](../../../../../../arithmetic-genus.md), not a claim about the genus of a normalization.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
