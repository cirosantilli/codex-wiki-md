<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [localic geometric morphism](../../../../../localic-geometric-morphism.md) $p:\mathcal D\to\mathcal F$ presents $\mathcal D$, over $\mathcal F$, as sheaves on an internal [locale](../../../../../locale.md) of $\mathcal F$. Equivalently, [subobjects](../../../../../subobject.md) of inverse images $p^*X$ form a separating family. A [hyperconnected geometric morphism](../../../../../hyperconnected-geometric-morphism.md) $h$ has a full faithful inverse image $h^*$ whose essential image is closed under [subobjects](../../../../../subobject.md). In particular, it induces bijections

$$
\operatorname{Sub}_{\mathcal F}(X)\cong\operatorname{Sub}_{\mathcal D}(h^*X).
$$

For this definition, subobject-closed means every [subobject](../../../../../subobject.md) of $h^*X$ is isomorphic, over $h^*X$, to the inverse image of a [subobject](../../../../../subobject.md) of $X$.

Here is the construction and proof of the [hyperconnected-localic factorization](../../../../../hyperconnected-localic-factorization.md). Given $f:\mathcal E\to\mathcal F$, its right adjoint gives natural bijections

$$
\mathcal F(X,f_*\Omega_{\mathcal E})\cong\mathcal E(f^*X,\Omega_{\mathcal E})\cong\operatorname{Sub}_{\mathcal E}(f^*X).
$$

Let $L$ be the internal locale whose frame of opens is $f_*\Omega_{\mathcal E}$. The frame operations are determined by these bijections: intersections are intersections of represented [subobjects](../../../../../subobject.md); the join of a family is its image under the projection from the parameter-indexed family. For an internal index object $I$, evaluation of the family over $X\times I$ becomes a [subobject](../../../../../subobject.md) of $f^*X\times f^*I$, and its direct image to $f^*X$ represents the join. Pullback stability of images makes this natural in $X$, and distributivity follows from the corresponding [subobject](../../../../../subobject.md) identity in $\mathcal E$. This explicitly constructs the internal frame rather than asserting it from the existence of $f_*$ alone.

Set $\mathcal D=\operatorname{Sh}_{\mathcal F}(L)$, with its localic projection $p$ to $\mathcal F$. We construct $h^*:\mathcal D\to\mathcal E$. A basic open family is a map $u:X\to f_*\Omega_{\mathcal E}$; its represented object in $\mathcal E$ is the [subobject](../../../../../subobject.md) $A_u\hookrightarrow f^*X$ corresponding to $u$. Meets and covering joins of open families become intersections and jointly epic families of these [subobjects](../../../../../subobject.md).

An internal sheaf on $L$ is presented by its local sections with their open domains and restrictions. Pull these domains back to the corresponding $A_u$ and identify two sections wherever their restrictions agree. This is an effective equivalence relation in $\mathcal E$, so its quotient defines $h^*$ of the sheaf. More concretely, if $S$ is the object of sections and $d:S\to\mathcal O(L)$ gives their domains, start with $A_d\subseteq f^*S$. For two sections, the join of the opens on which they agree gives an $L$-valued relation on $S\times S$, hence a [subobject](../../../../../subobject.md) of $f^*(S\times S)$. Restricted to $A_d\times A_d$, this is the germ equivalence relation used for the quotient. The restriction and sheaf axioms guarantee reflexivity, symmetry and transitivity. This construction is functorial. Products and [equalizers](../../../../../equaliser.md) are obtained by meeting domains and equalizing restrictions, so it preserves [finite limits](../../../../../finite-limit.md). A right adjoint is obtained by taking, over each open family $u$, the parameterized maps $A_u\to Y$ for $Y\in\mathcal E$. These maps satisfy the sheaf condition because a covering join gives an effective gluing of the $A_u$; their parameter objects are supplied by the original [adjunction](../../../../../adjoint-functors.md) $f^*\dashv f_*$ and exponentials. The map bijection on basic open families, followed by gluing, proves this is right adjoint to $h^*$. Thus $h$ is a [geometric morphism](../../../../../geometric-morphism.md).

We must check hyperconnectedness, not just construct a factorization. A map $A_u\to A_v$ has a graph which is a [subobject](../../../../../subobject.md) of $f^*(X\times Y)$. The represented-subobject bijection turns it into an $L$-valued relation on $X\times Y$. Its totality and single-valuedness say exactly that this relation is a map between the corresponding basic sheaf objects: totality uses the covering join, and single-valuedness uses intersections and the diagonal of $Y$. Thus maps between basic open families are precisely their maps in $\mathcal E$. Applying this to the local sections of arbitrary sheaves, compatible maps glue uniquely on both sides. Hence $h^*$ is full and faithful. Likewise a [subobject](../../../../../subobject.md) of $h^*S$ pulls back to [subobjects](../../../../../subobject.md) of its basic $A_u$; each is again represented by an open family, and their compatibility glues to a subsheaf of $S$. The essential image is therefore subobject-closed, proving that $h$ is hyperconnected.

The inverse image $p^*X$ is the constant family over the whole locale. The construction sends it to $f^*X$, so $h^*p^*\cong f^*$; taking right adjoints gives the required factorization

$$
\boxed{\mathcal E\xrightarrow{h}\operatorname{Sh}_{\mathcal F}(L)\xrightarrow{p}\mathcal F.}
$$

This argument uses the usual effective quotient and local-section constructions in a topos; it also explains why the relevant internal opens are relative [subobjects](../../../../../subobject.md) of $f^*X$, not just global [subobjects](../../../../../subobject.md) of the [terminal object](../../../../../terminal-object.md).

For uniqueness, suppose $f=p'h'$ with $h'$ hyperconnected and $p'$ localic. Then for every $X$,

$$
\operatorname{Sub}_{\mathcal E}(f^*X)\cong\operatorname{Sub}_{\mathcal D'}(p'^*X).
$$

If $\mathcal D'$ is sheaves on an internal locale $L'$, the right side is represented by its frame $\mathcal O(L')$. These identifications preserve intersections, joins and parameter change, so the representing internal frames are isomorphic: $\mathcal O(L')\cong f_*\Omega_{\mathcal E}$. The locale and its [sheaf topos](../../../../../grothendieck-topos.md) are therefore equivalent over $\mathcal F$. Under this equivalence the basic open families have the same images in $\mathcal E$, and their local-section presentations determine all other images and maps. Thus the two hyperconnected parts agree up to the same equivalence. **The factorization is unique up to equivalence.**

Finally suppose $f=h i$ with $i:\mathcal E\hookrightarrow\mathcal D$ a geometric embedding and $h:\mathcal D\to\mathcal F$ hyperconnected. Let $j$ be the [local operator](../../../../../lawvere-tierney-topology.md) on $\mathcal D$ presenting the inclusion. For a [subobject](../../../../../subobject.md) $A\hookrightarrow X$ of $\mathcal F$, take the $j$-closure of $h^*A$ in $h^*X$. Hyperconnectedness makes it the inverse image of a unique [subobject](../../../../../subobject.md) of $X$. This defines a closure operation on $\mathcal F$; its extensivity, idempotence, intersection preservation and pullback stability descend from the $j$-closure. Let $k$ be its [local operator](../../../../../lawvere-tierney-topology.md).

Hyperconnectedness also gives $h_*\Omega_{\mathcal D}\cong\Omega_{\mathcal F}$, by the represented-subobject bijections. The direct image $i_*\Omega_{\mathcal E}$ is the closed-truth object $\Omega_j$, and hence

$$
f_*\Omega_{\mathcal E}=h_*\Omega_j\cong\Omega_k.
$$

This follows either by taking the [equalizer](../../../../../equaliser.md) of $j$ and the identity or by representing closed [subobjects](../../../../../subobject.md) in the preceding closure construction. The internal locale with frame $\Omega_k$ is the sublocale of the terminal locale determined by $k$: covering joins are exactly closure by $k$. Its sheaves are the $k$-sheaves in $\mathcal F$, and its projection is their geometric inclusion. Applying the just-proved factorization to $f$ therefore gives

$$
\boxed{\mathcal E\xrightarrow{\text{hyperconnected}}\operatorname{sh}_k(\mathcal F)\xrightarrow{\text{inclusion}}\mathcal F.}
$$

This supplies the requested reordered factorization.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
