<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [dimension of an algebraic set](../../../../../dimension-of-an-algebraic-set.md) is the supremum of lengths of strict chains of nonempty [irreducible closed subsets](../../../../../irreducible-closed-subset.md). It is the maximum of the dimensions of the [irreducible components](../../../../../irreducible-component.md). On an [affine variety](../../../../../affine-algebraic-set.md) $X=\operatorname{Spec}A$, it equals the [Krull dimension](../../../../../krull-dimension.md) of $A$; if $X$ is irreducible, [Noether normalization](../../../../../noether-normalization.md) identifies this with the [transcendence degree](../../../../../transcendence-degree.md) of its [function field](../../../../../function-field-of-an-algebraic-variety.md) over $k$. Nonempty [Zariski-open subsets](../../../../../zariski-open-set.md) of an irreducible [algebraic variety](../../../../../algebraic-variety.md) have the same dimension, so the definition is compatible with affine charts and with [birational maps](../../../../../birational-map.md). In particular, $\dim\mathbb A^n=\dim\mathbb P^n=n$ and $\dim(X\times Y)=\dim X+\dim Y$ for irreducible [algebraic varieties](../../../../../algebraic-variety.md).

The [fiber dimension theorem](../../../../../fiber-dimension-theorem.md) says that a dominant [morphism of algebraic varieties](../../../../../morphism-of-algebraic-varieties.md) $f:X\to Y$ between irreducible [algebraic varieties](../../../../../algebraic-variety.md) has generic fibre dimension

$$
r=\dim X-\dim Y.
$$

Every [irreducible component](../../../../../irreducible-component.md) of every nonempty fibre over a closed point has dimension at least $r$. There is a nonempty [Zariski-open subset](../../../../../zariski-open-set.md) of $Y$ on which the fibres are nonempty and are [equidimensional algebraic varieties](../../../../../equidimensional-algebraic-variety.md) of dimension $r$. Dominance is required; for a general [morphism of algebraic varieties](../../../../../morphism-of-algebraic-varieties.md), replace $Y$ by the closure of its image. This gives the [dimension of image of a morphism](../../../../../dimension-of-image-of-a-morphism.md) formula.

For the generic fibre, the formula is the additivity of [transcendence degree](../../../../../transcendence-degree.md) in the tower $k\subset k(Y)\subset k(X)$. The lower bound on closed fibres comes from cutting by at most $\dim Y$ local parameters after a finite [Noether normalization](../../../../../noether-normalization.md) of an affine target chart: the [principal hypersurface dimension lemma](../../../../../principal-hypersurface-dimension-lemma.md) drops dimension by at most one per equation, and the finite normalization fibre separates the finitely many target points. For the generic upper bound, take finitely many affine source charts and apply [Noether normalization](../../../../../noether-normalization.md) to each coordinate ring over $k(Y)$. Clearing denominators in $k[Y]$ makes each chart finite over $\mathbb A^r$ relative to a suitable open target chart. Its fibres have dimension at most $r$. Intersecting these finitely many target opens and using the lower bound gives [generic equidimensionality of fibres](../../../../../generic-equidimensionality-of-fibres.md).

The [upper semicontinuity of local fibre dimension](../../../../../upper-semicontinuity-of-local-fibre-dimension.md) is a statement on the source: for a finite-type [morphism of schemes](../../../../../morphism-of-schemes.md), the points $x$ satisfying $\dim_xX_{f(x)}\le d$ form an open set. For a [proper morphism](../../../../../proper-morphism.md), the maximum fibre dimension is upper semicontinuous on the target as well. The properness qualification matters; one should not assert the latter for every finite-type [morphism of schemes](../../../../../morphism-of-schemes.md).

A first application is dimension counting for [plane sections](../../../../../plane-section.md) and intersections. On an irreducible [affine variety](../../../../../affine-algebraic-set.md), imposing $q$ [polynomial](../../../../../polynomial-split.md) equations gives each nonempty component [algebraic codimension](../../../../../codimension-of-an-algebraic-subvariety.md) at most $q$, by repeated [principal ideal theorem](../../../../../krull-principal-ideal-theorem.md). On a [smooth variety](../../../../../smooth-algebraic-variety.md) this underlies the [intersection dimension bound on a smooth variety](../../../../../intersection-dimension-bound-on-a-smooth-variety.md). A second application is to images: if a [morphism of algebraic varieties](../../../../../morphism-of-algebraic-varieties.md) has finite nonempty fibres, its image closure has the same dimension as the source. If it is also [proper](../../../../../proper-morphism.md), that image is closed. Thus an [isolated fibre point forces dominance in equal dimensions](../../../../../isolated-fibre-point-forces-dominance-in-equal-dimensions.md) when the irreducible source and target have equal dimension.

For the cubic-surface application, [projective lines](../../../../../projective-line.md) in $\mathbb P^3$ form the [Grassmannian](../../../../../grassmannian.md) $G=\operatorname{Gr}(2,4)$ of dimension four. Cubic forms form $\mathbb P^{19}$, since there are $\binom63=20$ degree-three [monomials](../../../../../monomial.md) in four variables. The [cubic surface line incidence variety](../../../../../cubic-surface-line-incidence-variety.md)

$$
I=\{(L,[F])\in G\times\mathbb P^{19}:F|_L=0\}
$$

has fibre $\mathbb P^{15}$ over every $L$: restricting a cubic to a [projective line](../../../../../projective-line.md) gives four independently prescribable coefficients. It is therefore an irreducible [projective-space bundle](../../../../../projective-bundle.md) of dimension $4+15=19$. The other projection $\pi:I\to\mathbb P^{19}$ is a [proper morphism](../../../../../proper-morphism.md), so its image $Z$ is closed and irreducible.

To show $Z=\mathbb P^{19}$, dimension counting alone is not enough; exhibit a fibre with an isolated point. Take

$$
F_0=x_0^2x_2+x_1^2x_3,\qquad L_0=\{x_2=x_3=0\}.
$$

A nearby [projective line](../../../../../projective-line.md) is the graph $x_2=ax_0+bx_1$, $x_3=cx_0+dx_1$. Restriction gives

$$
F_0|_L=ax_0^3+bx_0^2x_1+cx_0x_1^2+dx_1^3.
$$

It vanishes only when $a=b=c=d=0$. Thus $L_0$ is an isolated reduced point of the fibre. Applying the lower bound in the [fiber dimension theorem](../../../../../fiber-dimension-theorem.md) to $I\to Z$ gives $0\ge19-\dim Z$. Since $Z\subseteq\mathbb P^{19}$, its dimension is exactly 19, and closedness forces $Z=\mathbb P^{19}$. This is the [incidence proof that a cubic surface contains a line](../../../../../incidence-proof-that-a-cubic-surface-contains-a-line.md). The auxiliary cubic $F_0$ need not be smooth: the argument proves existence for every cubic form, and hence in particular for every [smooth cubic surface](../../../../../smooth-cubic-surface.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
