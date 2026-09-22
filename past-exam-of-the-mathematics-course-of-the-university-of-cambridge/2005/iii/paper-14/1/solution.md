<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $V\subseteq U$ be open subsets, and let $s\in\mathcal F_3(V)$. The assumed [flasque-kernel section-lifting lemma](../../../../../flasque-kernel-section-lifting-lemma.md) lifts $s$ to $\widetilde s\in\mathcal F_2(V)$. Since $\mathcal F_2$ is a [flabby sheaf](../../../../../flasque-sheaf.md), extend $\widetilde s$ to a section on $U$, then project to $\mathcal F_3(U)$. Its restriction is $s$. Thus every restriction map of $\mathcal F_3$ is [surjective](../../../../../surjective-function.md), proving that **the quotient of two [flabby sheaves](../../../../../flasque-sheaf.md) in a short exact sequence is flabby**.

For the construction of [sheaf cohomology](../../../../../sheaf-cohomology.md), embed a [sheaf of abelian groups](../../../../../sheaf-of-abelian-groups.md) $\mathcal F$ into the [sheaf](../../../../../sheaf-mathematics.md)

$$
C(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P
$$

by sending a section to all its [germs](../../../../../germ-of-a-sheaf-section.md). This is [injective](../../../../../injective-function.md) because a section with every germ zero is zero. Arbitrary families of stalk elements glue point by point, and restriction maps are projections; hence $C(\mathcal F)$ is a [flabby sheaf](../../../../../flasque-sheaf.md). Set $\mathcal Q^0=\mathcal F$, $\mathcal I^j=C(\mathcal Q^j)$ and $\mathcal Q^{j+1}=\mathcal I^j/\mathcal Q^j$. Compose the quotient map with the next embedding to obtain the [flasque resolution](../../../../../flasque-resolution.md)

$$
0\longrightarrow\mathcal F\longrightarrow\mathcal I^0
\longrightarrow\mathcal I^1\longrightarrow\cdots.
$$

The [sheaf cohomology](../../../../../sheaf-cohomology.md) groups are the [cohomology groups](../../../../../cohomology-group.md) of the resulting [cochain complex](../../../../../cochain-complex.md) of [global sections](../../../../../global-section.md):

$$
H^j(X,\mathcal F)=
\frac{\ker\bigl(\Gamma(X,\mathcal I^j)\to\Gamma(X,\mathcal I^{j+1})\bigr)}
{\operatorname{im}\bigl(\Gamma(X,\mathcal I^{j-1})\to\Gamma(X,\mathcal I^j)\bigr)}
\quad(j>0),
\qquad H^0(X,\mathcal F)=\Gamma(X,\mathcal F).
$$

The usual comparison of resolutions identifies this construction with the right derived functors of [global sections](../../../../../global-section.md); the construction above is the [Godement resolution](../../../../../godement-resolution.md).

If $\mathcal F$ is itself a [flabby sheaf](../../../../../flasque-sheaf.md), the quotient argument shows inductively that every $\mathcal Q^j$ is flabby. The assumed lifting result therefore makes

$$
0\to\Gamma(X,\mathcal Q^j)\to\Gamma(X,\mathcal I^j)
\to\Gamma(X,\mathcal Q^{j+1})\to0
$$

an [exact sequence](../../../../../exact-sequence.md) for every $j$. The global-section complex is consequently exact in every positive degree. In particular,

$$
\boxed{H^j(X,\mathcal F)=0\quad(j>0)\qquad\text{if }\mathcal F\text{ is flabby}.}
$$

This establishes the vanishing from the section-lifting property rather than assuming it in advance.

For the [smooth algebraic curve](../../../../../smooth-algebraic-curve.md) $X$, a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) is a finite formal sum $D=\sum_P n_PP$ of closed points with integer coefficients. At each closed point, the [local ring of a smooth algebraic curve](../../../../../local-ring-of-a-smooth-algebraic-curve.md) is a [discrete valuation ring](../../../../../discrete-valuation-ring.md); write its normalized [discrete valuation](../../../../../discrete-valuation.md) as $v_P$. For $f\in k(X)^*$ the [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) is $\operatorname{div}(f)=\sum_Pv_P(f)P$. Only finitely many coefficients are nonzero: zeros and poles are proper closed subsets in the [Noetherian Zariski topology](../../../../../noetherian-zariski-topology.md) of a curve. The [divisor class group](../../../../../divisor-class-group.md) is the [abelian group](../../../../../abelian-group.md)

$$
\boxed{\operatorname{Cl}(X)=
\operatorname{Div}(X)/\{\operatorname{div}(f):f\in k(X)^*\}.}
$$

Equivalently, its elements are [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) modulo [linear equivalence of divisors](../../../../../linear-equivalence-of-divisors.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
