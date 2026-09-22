<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [morphism of schemes](../../../../../morphism-of-schemes.md) $f:X\to Y$ is a [flat morphism](../../../../../flat-morphism.md) when each [local ring](../../../../../local-ring.md) $\mathcal O_{X,x}$ is a [flat module](../../../../../flat-module.md) over $\mathcal O_{Y,f(x)}$: tensoring with it preserves [exact sequences](../../../../../exact-sequence.md). An [open immersion](../../../../../open-immersion.md) induces isomorphisms on the [local rings](../../../../../local-ring.md) at its points, so it is flat.

For a [closed immersion](../../../../../closed-immersion.md), the printed equivalence is valid with the additional hypothesis of finite presentation, for example over a locally Noetherian target, and with nonempty source. Here is the proof with that hypothesis. On an [affine chart](../../../../../affine-chart-of-a-variety.md) the map is $A\to A/I$, with $I$ finitely generated. If $\mathfrak p\supseteq I$, the flat cyclic [module](../../../../../module-mathematics.md) $A_{\mathfrak p}/I_{\mathfrak p}$ is free over the [local ring](../../../../../local-ring.md) $A_{\mathfrak p}$, and its residue-field [dimension](../../../../../dimension-vector-space.md) is one. Therefore its quotient map from $A_{\mathfrak p}$ is an [isomorphism](../../../../../isomorphism.md) and $I_{\mathfrak p}=0$. Finite generation gives a neighbourhood of $\mathfrak p$ on which $I$ vanishes. The closed image $V(I)$ is consequently open. A nonempty [clopen](../../../../../clopen-set.md) image in a connected target is the whole target; then $I$ vanishes at every prime and is zero. The immersion is an [isomorphism](../../../../../isomorphism.md). The converse is immediate. This proves the [flat closed immersion of finite presentation](../../../../../flat-closed-immersion-of-finite-presentation.md) assertion.

Without finite presentation, connectedness alone does not suffice. Take $A=C([0,1],\mathbb R)$ and let $\mathfrak m=\{a:a(0)=0\}$. Let $I$ consist of functions vanishing on some neighbourhood of zero. The map $A\to A_{\mathfrak m}$ has kernel $I$: multiplying such a function by a continuous cutoff equal to one at zero kills it, whereas $ga=0$ with $g(0)\ne0$ forces $a$ to vanish near zero. This map is surjective, because the reciprocal of any denominator nonzero at zero can be extended continuously from a small neighbourhood of zero to the whole interval. Thus

$$
A/I\cong A_{\mathfrak m}.
$$

The map $\operatorname{Spec}(A/I)\to\operatorname{Spec}A$ is both a [closed immersion](../../../../../closed-immersion.md) and a flat [localization](../../../../../localization-of-a-ring.md). Its source is connected because its [ring](../../../../../ring.md) is local. Its target is connected because continuous [idempotent](../../../../../idempotent.md) functions on the connected interval can only be the constants zero and one. It is not an [isomorphism](../../../../../isomorphism.md): $I$ contains nonzero functions supported away from zero. This supplies a concrete counterexample to the unrestricted assertion. The kernel is a [pure ideal](../../../../../pure-ideal.md); this is the general mechanism behind such examples, as explained in [the Stacks Project's treatment of pure ideals](https://stacks.math.columbia.edu/tag/04PQ).

For the finite-flat fibre assertion, first note the local algebra fact that a finitely generated [flat module](../../../../../flat-module.md) $M$ over a [local ring](../../../../../local-ring.md) $(A,\mathfrak m)$ is free. Choose generators $m_1,\ldots,m_r$ whose residues form a [basis](../../../../../basis.md) of $M/\mathfrak mM$, using [Nakayama's lemma](../../../../../nakayama-lemma.md). If a row $a=(a_1,\ldots,a_r)$ gives a relation $\sum a_im_i=0$, the [equational criterion for flatness](../../../../../equational-criterion-for-flatness.md) supplies elements $n_j$ and a [matrix](../../../../../matrix.md) $B=(b_{ij})$ such that $m_i=\sum_jb_{ij}n_j$ and $aB=0$. Write each $n_j$ as a linear combination of the $m_i$, with coefficient [matrix](../../../../../matrix.md) $C$. Then $m=BCm$. Independence modulo $\mathfrak m$ makes $BC$ congruent to the identity. This square [matrix](../../../../../matrix.md) is invertible over the [local ring](../../../../../local-ring.md), and $aBC=0$ implies $a=0$. Thus the chosen generators are a [basis](../../../../../basis.md). This also justifies the cyclic-module step above; see [the finite-flat local lemma](https://stacks.math.columbia.edu/tag/00NV#lemma-finite-flat-local).

Now let $\mathcal A=f_*\mathcal O_X$ for the finite [flat morphism](../../../../../flat-morphism.md). On each [affine chart](../../../../../affine-chart-of-a-variety.md) this is the finite flat algebra defining its inverse image. Hence $\mathcal A_y$ is free over $\mathcal O_{Y,y}$, of some finite rank $r_y$. Let $\eta$ be the [generic point](../../../../../generic-point.md) of the irreducible target. Localizing that [free module](../../../../../free-module.md) at $\eta$ gives

$$
\mathcal A_\eta\cong\mathcal O_{Y,\eta}^{\oplus r_y}.
$$

Every point specializes from the same $\eta$, so every $r_y$ equals the fixed rank at $\eta$. This remains valid if the irreducible target is nonreduced: one compares free ranks over its nonzero generic [local ring](../../../../../local-ring.md), not necessarily over a [field](../../../../../field.md). The fibre is affine, and

$$
\Gamma(X_y,\mathcal O_{X_y})\cong\mathcal A_y\otimes_{\mathcal O_{Y,y}}\kappa(y).
$$

Consequently

$$
\boxed{\dim_{\kappa(y)}\Gamma(X_y,\mathcal O_{X_y})=r_\eta\quad\text{for every }y.}
$$

This is [finite flat rank over an irreducible scheme](../../../../../finite-flat-rank-over-an-irreducible-scheme.md). No unjustified replacement of finite flat by finite locally free on an arbitrary base is needed.

For an algebraic curve of finite type over a [field](../../../../../field.md), its [normalization of an integral scheme](../../../../../normalization-of-an-integral-scheme.md) is finite and birational. If flat, the preceding rank is one, since the generic fibre has the same [function field](../../../../../function-field-of-an-algebraic-variety.md). Locally its normalization algebra $B$ is therefore a free $A$-module of rank one. The element $1_B$ generates: its image cannot vanish in the one-dimensional fibre algebra, and [Nakayama's lemma](../../../../../nakayama-lemma.md) applies. Thus $A\to B$ is an [isomorphism](../../../../../isomorphism.md). Conversely the identity normalization is flat.

The parenthetical definition in the PDF does not explicitly impose finite type. One can prove the conclusion even in that broader setting without assuming a finite normalization. For any [affine chart](../../../../../affine-chart-of-a-variety.md), let $A\subseteq B\subseteq\operatorname{Frac}(A)$ describe its [normalization of an integral scheme](../../../../../normalization-of-an-integral-scheme.md). Integrality makes the map on spectra surjective; if $B$ is flat it is faithfully flat. Faithful flatness gives contraction of [ideals](../../../../../ideal.md), $vB\cap A=vA$. For $b=u/v\in B$, with $u,v\in A$ and $v\ne0$, one has $u=vb\in vB\cap A=vA$. Thus $u=va$ for some $a\in A$, so $b=a$. Therefore $B=A$ on every chart. We have proved the [flat normalization is an isomorphism](../../../../../flat-normalization-is-an-isomorphism.md) result and, in particular,

$$
\boxed{C'\to C\text{ is flat}\iff C'=C.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 89](../../paper-89-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
