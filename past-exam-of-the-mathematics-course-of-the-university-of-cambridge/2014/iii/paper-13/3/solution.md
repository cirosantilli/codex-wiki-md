<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [sheaf of modules](../../../../../sheaf-of-modules.md) $\mathcal F$ over $\mathcal O_X$ is [quasi-coherent](../../../../../quasi-coherent-sheaf.md) when locally it admits a presentation

$$
\mathcal O_X^{(J)}\longrightarrow\mathcal O_X^{(I)}\longrightarrow\mathcal F\longrightarrow0,
$$

with arbitrary indexing sets $I,J$. On an affine chart, sheafifying the corresponding [module](../../../../../module-mathematics.md) presentation and using [exactness of localization](../../../../../exactness-of-localization.md) identifies its cokernel with a [sheaf](../../../../../sheaf-mathematics.md) $\widetilde N$. Thus one may equivalently require that locally on affine charts $\mathcal F$ is associated with a [module](../../../../../module-mathematics.md). This does not impose finite generation, which belongs to the stronger coherent condition.

On the affine variety $X$ with [coordinate ring](../../../../../coordinate-ring.md) $A$, put $M=\Gamma(X,\mathcal F)$. Refine local [module](../../../../../module-mathematics.md) charts to a finite principal [open cover](../../../../../open-cover.md) $X=\bigcup_jD(g_j)$ such that $\mathcal F|_{D(g_j)}\cong\widetilde N_j$ for an $A_{g_j}$-module $N_j$. This is possible because principal opens form an [open basis](../../../../../basis-of-a-topology.md) and $X$ is [quasi-compact](../../../../../compact-space.md). On the overlap $D(g_jg_k)$ the sections are the corresponding further [localization](../../../../../localization-of-a-ring.md) of $N_j$ or $N_k$. The [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) gives an equalizer

$$
0\longrightarrow M\longrightarrow\prod_jN_j\longrightarrow\prod_{j,k}\mathcal F(D(g_jg_k)),
$$

where the last map is the difference of restrictions. For any $f\in A$, localize this sequence. [Exactness of localization](../../../../../exactness-of-localization.md) and commutation with finite products give exactly the equalizer for the cover $D(f)=\bigcup_jD(fg_j)$. Hence

$$
\boxed{M_f\cong\Gamma(D(f),\mathcal F).}
$$

The [isomorphisms](../../../../../isomorphism.md) are canonical and commute with all basic-open restrictions. Since the sections of $\widetilde M$ on these opens are $M_f$, they identify the two [sheaves](../../../../../sheaf-mathematics.md):

$$
\boxed{\mathcal F\cong\widetilde{\Gamma(X,\mathcal F)}.}
$$

Conversely $\widetilde M$ is quasi-coherent for every $A$-module $M$, since a free presentation of $M$ gives the required [sheaf](../../../../../sheaf-mathematics.md) presentation. Also $\Gamma(X,\widetilde M)=M$, and [module](../../../../../module-mathematics.md) homomorphisms sheafify, while a [sheaf](../../../../../sheaf-mathematics.md) morphism is determined on every $D(f)$ by the [localization](../../../../../localization-of-a-ring.md) of its map on [global sections](../../../../../global-section.md). This proves the [affine module-sheaf equivalence](../../../../../affine-module-sheaf-equivalence.md).

For a short exact sequence of [quasi-coherent sheaves](../../../../../quasi-coherent-sheaf.md), the sequence of their [stalks](../../../../../stalk-of-a-sheaf.md) is exact. Under this equivalence the [stalk](../../../../../stalk-of-a-sheaf.md) at $x$ is the [localization](../../../../../localization-of-a-ring.md) of the global-section [module](../../../../../module-mathematics.md) at $\mathfrak m_x$. Exactness of [module](../../../../../module-mathematics.md) sequences can be checked at all maximal ideals, by [localization detects zero elements](../../../../../localization-detects-zero-elements.md) applied to their homology, so the global-section [modules](../../../../../module-mathematics.md) also form a short exact sequence. Therefore **[global sections](../../../../../global-section.md) are exact on [quasi-coherent sheaves](../../../../../quasi-coherent-sheaf.md) over an affine variety**. This is stronger than the left exactness of the [global section functor](../../../../../global-section-functor.md) on arbitrary [sheaves](../../../../../sheaf-mathematics.md), and follows from [localization](../../../../../localization-of-a-ring.md), not from assuming the cohomology vanishing still to be proved.

For an open inclusion $j:U\hookrightarrow X$, the requested [sheaf](../../../../../sheaf-mathematics.md) is

$$
\boxed{{}_U\mathcal F=j_*(\mathcal F|_U),\qquad({}_U\mathcal F)(V)=\mathcal F(V\cap U).}
$$

Restriction gives $\mathcal F\to{}_U\mathcal F$. This [direct image from an open restriction](../../../../../direct-image-from-an-open-restriction.md) is not extension by zero: its [stalks](../../../../../stalk-of-a-sheaf.md) outside $U$ may be nonzero.

The [locally vanishing principle for sheaf cohomology](../../../../../locally-vanishing-principle-for-sheaf-cohomology.md) says that a class $\xi\in H^i(X,\mathcal F)$, $i>0$, is killed on a suitable neighbourhood of every point. Under the stated hypothesis that basis opens and their finite intersections have zero cohomology in degrees $1,\ldots,i-1$, these neighbourhoods can be chosen in that basis so that the image of $\xi$ under

$$
H^i(X,\mathcal F)\longrightarrow H^i(X,{}_U\mathcal F)
$$

is zero. In particular its restriction in $H^i(U,\mathcal F|_U)$ is zero. This is a statement about individual classes; it does not assert that every locally vanishing class is already globally zero.

Here is a noncircular proof of [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md), applied to the variety. Induct on $i>0$, simultaneously for every affine variety and [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md). Assume all lower positive degrees vanish. The principal-open basis is closed under finite intersections, so it satisfies the principle's hypothesis. Given $\xi\in H^i(X,\mathcal F)$, choose a finite principal cover $\mathcal U=(D(f_j))$ on which it restricts to zero.

Applying the [Čech cochain complex](../../../../../cech-cochain-complex.md) to a [flasque resolution](../../../../../flasque-resolution.md) gives the [Čech lifting below the first possible local cohomology degree](../../../../../cech-lifting-below-the-first-possible-local-cohomology-degree.md) comparison segment, under lower-degree vanishing on all intersections

$$
0\longrightarrow\check H^i(\mathcal U,\mathcal F)\longrightarrow H^i(X,\mathcal F)\longrightarrow\prod_jH^i(D(f_j),\mathcal F).
$$

For completeness, the double complex has terms $\check C^p(\mathcal U,\mathcal I^q)$. Its augmented rows are exact because each $\mathcal I^q$ is flasque, so its total cohomology is the cohomology of [global sections](../../../../../global-section.md) of the resolution. The vertical cohomology on intersections in degrees $0<q<i$ is zero. Equivalently, start with local primitives of a cocycle representing $\xi$, take their differences on pairwise overlaps, and solve successively for primitives of those differences in degrees $i-1,i-2,\ldots,1$. The last difference is a Čech $i$-cocycle with values in $\mathcal F$. This identifies the kernel of the restriction map with the displayed Čech group. No vanishing in degree $i$ on the intersections has been assumed.

It remains a [module](../../../../../module-mathematics.md) calculation. Write $\mathcal F=\widetilde M$. The augmented Čech complex is

$$
0\longrightarrow M\longrightarrow\prod_jM_{f_j}\longrightarrow\prod_{j<k}M_{f_jf_k}\longrightarrow\cdots.
$$

Since the $D(f_j)$ cover $X$, the $f_j$ generate the [unit ideal](../../../../../unit-ideal.md). This complex is exact. To see it algebraically, use alternating cochains, with repeated indices giving zero. For a cocycle $c$, choose $N$ large enough to clear every $f_j$-denominator in $f_j^Nc_{jI}$, as well as the finitely many cocycle relations; [vanishing criterion in a module localization](../../../../../vanishing-criterion-in-a-module-localization.md) allows a further power to clear relations which initially hold only after [localization](../../../../../localization-of-a-ring.md). Since the ideal $(f_j^N)$ is still the [unit ideal](../../../../../unit-ideal.md), choose $a_j$ with $\sum_ja_jf_j^N=1$. Define

$$
b_I=\sum_j a_jf_j^Nc_{jI},
$$

using those cleared representatives in $M_{f_I}$. The cocycle identity gives $\delta b=(\sum_ja_jf_j^N)c=c$. The same argument with the augmentation gives gluing and uniqueness in degree zero. This is [exactness of the unit-ideal localization Čech complex](../../../../../exactness-of-the-unit-ideal-localization-cech-complex.md).

Thus $\check H^i(\mathcal U,\mathcal F)=0$, so the class $\xi$, whose restrictions were zero, is zero. The induction starts at $i=1$, when the lower-degree condition is empty. We have proved

$$
\boxed{H^i(X,\mathcal F)=0\quad\text{for every }i>0\text{ and every affine quasi-coherent }\mathcal F.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
