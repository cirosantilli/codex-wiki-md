<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The intersection hypothesis says that $X$ is a [semi-separated scheme](../../../../../semi-separated-scheme.md). For an [affine open subscheme](../../../../../affine-open-subscheme.md) $V\subseteq X$, the intersection $V\cap U$ is affine. Restricting the given [short exact sequence of sheaves](../../../../../short-exact-sequence-of-sheaves.md) to it and applying the [affine module-sheaf equivalence](../../../../../affine-module-sheaf-equivalence.md) gives an [exact sequence](../../../../../exact-sequence.md) of [global sections](../../../../../global-section.md):

$$
0\longrightarrow\Gamma(V\cap U,\mathcal M')
\longrightarrow\Gamma(V\cap U,\mathcal M)
\longrightarrow\Gamma(V\cap U,\mathcal M'')\longrightarrow0.
$$

These are exactly the sections on $V$ of the three [direct image sheaves](../../../../../direct-image-sheaf.md). Affine opens form a basis, and every section of the last sheaf on such a basis open lifts to the middle sheaf. This proves surjectivity as a [sheaf morphism](../../../../../morphism-of-sheaves.md); left exactness of [direct image](../../../../../direct-image-sheaf.md) supplies the other positions. Hence **direct image preserves this short exact sequence**. The crucial ingredient is exactness of sections of [quasi-coherent sheaves](../../../../../quasi-coherent-sheaf.md) on an affine intersection; arbitrary [open immersions](../../../../../open-immersion.md) need not have this property.

For the cohomology comparison, every nonempty finite intersection

$$
U_{i_0\cdots i_p}=U_{i_0}\cap\cdots\cap U_{i_p}
$$

is affine. This follows by [mathematical induction](../../../../../mathematical-induction.md), intersecting the affine intersection already obtained with the next affine open. The restriction of $\mathcal F$ to it is quasi-coherent, so [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md) gives

$$
H^q(U_{i_0\cdots i_p},\mathcal F)=0\qquad(q>0).
$$

We now prove why this local vanishing gives the [acyclic cover theorem](../../../../../leray-s-theorem.md), rather than identifying the two sorts of cohomology without a comparison.

Take a [flasque resolution](../../../../../flasque-resolution.md) $0\to\mathcal F\to\mathcal I^0\to\mathcal I^1\to\cdots$. Here a [flabby sheaf](../../../../../flasque-sheaf.md) has surjective restriction maps; its restrictions to open subsets are still flabby and have zero higher [sheaf cohomology](../../../../../sheaf-cohomology.md). Form the [double complex](../../../../../double-complex.md)

$$
C^{p,q}=\prod_{i_0<\cdots<i_p}
\Gamma(U_{i_0\cdots i_p},\mathcal I^q).
$$

The horizontal differential is the alternating restriction map $d_{\mathrm C}$; the vertical one $d_{\mathrm I}$ is induced by the resolution. They commute, so the total differential in bidegree $(p,q)$ is $d_{\mathrm C}+(-1)^p d_{\mathrm I}$ and has square zero. The [Čech resolution on a semi-separated scheme](../../../../../cech-resolution-on-a-semi-separated-scheme.md) uses precisely these intersections.

A [flabby sheaf](../../../../../flasque-sheaf.md) has zero positive [Čech cohomology](../../../../../cech-cohomology.md) for a finite [open cover](../../../../../open-cover.md), and its degree-zero [Čech cohomology](../../../../../cech-cohomology.md) is its [global sections](../../../../../global-section.md). One way to establish this auxiliary fact is to use the exact augmented two-open complex

$$
0\to\Gamma(V\cup W,\mathcal I)
\to\Gamma(V,\mathcal I)\oplus\Gamma(W,\mathcal I)
\to\Gamma(V\cap W,\mathcal I)\to0.
$$

Exactness at the first two terms is the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md); the last map is onto because a section on the intersection extends to $V$. For the induction step, write $V$ for the union of all but the last open and $W$ for the last open. Separate Čech cochains according to whether their index list contains the last index. The resulting two-block complex compares the smaller cover of $V$ with its restricted cover of $V\cap W$, together with $\Gamma(W,\mathcal I)$ in degree zero. By induction those two smaller cover complexes have cohomology only in degree zero, where they give $\Gamma(V,\mathcal I)$ and $\Gamma(V\cap W,\mathcal I)$. The displayed two-open exact sequence then gives zero positive-degree cohomology for the full cover. This proves the auxiliary fact by induction on the number of opens. Thus horizontal cohomology of $C^{\bullet,q}$ consists only of $\Gamma(X,\mathcal I^q)$ in degree zero. Computing the cohomology of the total complex first horizontally therefore gives $H^n(X,\mathcal F)$, by the [resolution principle for sheaf cohomology](../../../../../resolution-principle-for-sheaf-cohomology.md).

On the other hand, vertical cohomology is

$$
H^q(C^{p,\bullet})
=\prod_{i_0<\cdots<i_p}H^q(U_{i_0\cdots i_p},\mathcal F),
$$

since the restricted [flasque resolutions](../../../../../flasque-resolution.md) compute cohomology on each intersection. The already established affine vanishing makes all rows with $q>0$ zero. The surviving row $q=0$ is exactly the [Čech cochain complex](../../../../../cech-cochain-complex.md) $\check C^\bullet(\mathcal U,\mathcal F)$. Computing total cohomology first vertically therefore gives $\check H^n(\mathcal U,\mathcal F)$. These two computations are justified by the two filtrations of the first-quadrant [double complex](../../../../../double-complex.md): in every total degree only finitely many terms occur, and the cover also bounds the horizontal degree. Their edge maps give the natural identification

$$
\boxed{\check H^p(\mathcal U,\mathcal F)\cong H^p(X,\mathcal F)\quad(p\geq0).}
$$

For negative degrees both groups are zero by convention. In particular, degree zero is the usual identification by the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md), not merely a comparison of dimensions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
