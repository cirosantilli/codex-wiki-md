# Banach space

↑ **Parent:** [Normed vector space](functional-analysis.md#normed-vector-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Banach_space)

A Banach space is a normed vector space that is complete in its norm metric.

**Table of contents**

- [Finite codimension in a Banach space](#finite-codimension-in-a-banach-space)
- [Banach-Saks property](#banach-saks-property)
- [Cotype of a Banach space](#cotype-of-a-banach-space)
  - [Cotype 2](#cotype-2)
    - [Cotype 2 extrapolation on finite-dimensional linfinity](#cotype-2-extrapolation-on-finite-dimensional-linfinity)
- [Complemented subspace](#complemented-subspace)
  - [Pełczyński decomposition method](#pelczynski-decomposition-method)
- [Hereditarily indecomposable Banach space](#hereditarily-indecomposable-banach-space)
  - [Gowers dichotomy theorem](#gowers-dichotomy-theorem)
- [Quotient Banach space](#quotient-banach-space)
  - [Approximate weakly null lifting through a quotient](#approximate-weakly-null-lifting-through-a-quotient)
  - [Quotient norm](#quotient-norm)
- [Convex block](#convex-block)
  - [Convex-block cancellation of a weak-star limit](#convex-block-cancellation-of-a-weak-star-limit)
- [Duality mapping](#duality-mapping)
- [Bounded scalar functions on an index set](#bounded-scalar-functions-on-an-index-set)
  - [Coordinate functional representation of an operator into bounded indexed functions](#coordinate-functional-representation-of-an-operator-into-bounded-indexed-functions)
- [Separable Banach space](#separable-banach-space)
- [l-p sequence space](#l-p-sequence-space)
  - [Absolutely summable sequence space](#absolutely-summable-sequence-space)
  - [l2 sequence space](#l2-sequence-space)
    - [Uniform convexity of l2](#uniform-convexity-of-l2)
  - [Finitely supported sequence](#finitely-supported-sequence)
    - [Density of finitely supported sequences in l-p](#density-of-finitely-supported-sequences-in-l-p)
- [l-infinity sequence space](#l-infinity-sequence-space)
  - [Generalized limit](#generalized-limit)
  - [Banach limit](#banach-limit)
    - [Cesàro construction of a Banach limit](#cesaro-construction-of-a-banach-limit)
    - [Ultrafilter construction of a Banach limit](#ultrafilter-construction-of-a-banach-limit)
  - [Left shift on bounded sequences](#left-shift-on-bounded-sequences)
- [Riesz's lemma](#riesz-s-lemma)
  - [Compact unit ball characterizes finite-dimensional normed spaces](#compact-unit-ball-characterizes-finite-dimensional-normed-spaces)
- [Uniformly convex Banach space](#uniformly-convex-banach-space)
  - [Nearest point in a uniformly convex Banach space](#nearest-point-in-a-uniformly-convex-banach-space)
  - [Clarkson's inequalities](#clarkson-s-inequalities)
    - [Dual-exponent Clarkson inequality](#dual-exponent-clarkson-inequality)
- [Uniform boundedness principle](#uniform-boundedness-principle)
  - [Weak boundedness implies norm boundedness](#weak-boundedness-implies-norm-boundedness)
  - [Uniform bound from pointwise absolute summability of dual evaluations](#uniform-bound-from-pointwise-absolute-summability-of-dual-evaluations)

## Finite codimension in a Banach space

↑ **Parent:** [Banach space](banach-space.md)

For a closed [linear subspace](vector-space.md#vector-subspace) $Y$ of a [Banach space](banach-space.md) $X$, finite codimension means the vector quotient $X/Y$ has finite [dimension](vector-space.md#dimension-vector-space). This definition does not subtract two infinite dimensions. A local [stable manifold](dynamical-systems.md#stable-manifold) has the codimension of its tangent subspace. If the linearized phase space has a [direct sum](vector-space.md#direct-sum) decomposition $X=E^s\oplus E^u$ with $\dim E^u=1$, then $X/E^s$ is isomorphic to $E^u$, so a local stable manifold tangent to $E^s$ has codimension one.

## Banach-Saks property

↑ **Parent:** [Banach space](banach-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Banach-Saks_property)

A [Banach space](banach-space.md) has the Banach-Saks property if every bounded [sequence](real-analysis.md#sequence) contains a [subsequence](real-analysis.md#subsequence) whose arithmetic averages converge in [norm](functional-analysis.md#norm). The weak Banach-Saks property requires this only for weakly convergent sequences. The [weak Banach–Saks theorem in a Hilbert space](hilbert-space.md#weak-banach-saks-theorem-in-a-hilbert-space) establishes that weak version in [Hilbert spaces](hilbert-space.md).

## Cotype of a Banach space

↑ **Parent:** [Banach space](banach-space.md)

A [Banach space](banach-space.md) $X$ has cotype $q$, $2\le q<\infty$, if a constant $C$ independent of the number of vectors satisfies $(\sum_j\|x_j\|^q)^{1/q}\le C(\mathbb E\|\sum_j\varepsilon_jx_j\|^2)^{1/2}$ for independent symmetric [Rademacher random variables](probability-theory.md#rademacher-distribution). It prevents many large vectors from having a small random sum.

### Cotype 2

↑ **Parent:** [Cotype of a Banach space](#cotype-of-a-banach-space)

This is [cotype of a Banach space](#cotype-of-a-banach-space) with $q=2$. The [Lp space](measure-theory.md#lp-space) $L^1$ has cotype 2 with constant at most $\sqrt2$: the triangle inequality for the Euclidean norm gives $(\sum\|f_j\|_1^2)^{1/2}\le\int(\sum|f_j(t)|^2)^{1/2}\,dt$, and the [sharp Rademacher second-moment inequality](fourier-analysis.md#sharp-rademacher-second-moment-inequality), followed by [Fubini theorem](measure-theory.md#fubini-s-theorem), bounds this by $\sqrt2\,\mathbb E\|\sum\varepsilon_jf_j\|_1$.

#### Cotype 2 extrapolation on finite-dimensional linfinity

↑ **Parent:** [Cotype 2](#cotype-2)

If a [Banach space](banach-space.md) $Y$ has [cotype 2](#cotype-2) constant $C$, every [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:\ell_\infty^N\to Y$ satisfies $\pi_2(T)\le3^{1/4}C\pi_4(T)$ and $\pi_2(T)\le4\sqrt3 C^2\|T\|$, uniformly in $N$. The first bound follows from [Pietsch factorization theorem](topological-vector-space.md#pietsch-factorization-theorem) and the fourth moment bound for [Rademacher sums](probability-theory.md#rademacher-sum). For the second, 2-summing domination gives a weighted coordinate $L^2$ norm; clipping coordinates at a variable threshold yields $\pi_4(T)\le2\sqrt{\|T\|\pi_2(T)}$, which absorbs the first bound.

## Complemented subspace

↑ **Parent:** [Banach space](banach-space.md)

A closed [vector subspace](vector-space.md#vector-subspace) $Y$ of a [Banach space](banach-space.md) $X$ is complemented if a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $P:X\to X$ satisfies $P^2=P$ and $P(X)=Y$. Equivalently, $X$ is the topological [direct sum](vector-space.md#direct-sum) of $Y$ and a closed subspace: a projection gives $X=Y\oplus\ker P$, and the coordinate projection of such a decomposition is bounded.

<h3 id="pelczynski-decomposition-method">Pełczyński decomposition method</h3>

↑ **Parent:** [Complemented subspace](#complemented-subspace)

For a [Banach space](banach-space.md) $E$ satisfying $E\cong(\bigoplus_{n\ge1}E)_p$, a [complemented subspace](#complemented-subspace) $W$ is absorbed by $E$: write $E\cong W\oplus V$, expand the countable sum, and absorb one additional copy of $W$ into the countably many $W$ summands. Hence $E\oplus W\cong E$. If $Z$ is complemented in $E$ and contains a complemented copy of $E$, write $Z\cong E\oplus W$ with $W$ complemented in $E$; the preceding argument gives $Z\cong E$. The decompositions are [Banach space isomorphisms](functional-analysis.md#banach-space-isomorphism), not merely algebraic decompositions.

## Hereditarily indecomposable Banach space

↑ **Parent:** [Banach space](banach-space.md)

An infinite-dimensional Banach space is hereditarily indecomposable if no closed infinite-dimensional subspace is a topological direct sum of two infinite-dimensional closed subspaces. Equivalently, for any two infinite-dimensional closed subspaces $U,V$ and any $\varepsilon>0$, some unit vectors $u\in U,v\in V$ satisfy $\|u-v\|<\varepsilon$. A positive lower bound on such distances would make the addition map from $U\oplus V$ an isomorphism onto a closed subspace.

### Gowers dichotomy theorem

↑ **Parent:** [Hereditarily indecomposable Banach space](#hereditarily-indecomposable-banach-space)

Every infinite-dimensional [Banach space](banach-space.md) contains either an [unconditional basic sequence](functional-analysis.md#unconditional-basic-sequence) or a [hereditarily indecomposable Banach space](#hereditarily-indecomposable-banach-space). For a space with a basis and no unconditional basic sequence, apply the block Ramsey theorem to finite sequences whose odd and even spans contain nearby unit vectors. A diagonal sequence of successively sharper games gives a subspace in which every pair of infinite-dimensional subspaces has angle zero.

## Quotient Banach space

↑ **Parent:** [Banach space](banach-space.md)

For a closed [vector subspace](vector-space.md#vector-subspace) $Y$ of a [Banach space](banach-space.md) $X$, the [quotient vector space](vector-space.md#quotient-vector-space) $X/Y$ is complete with its [quotient norm](#quotient-norm). Closedness makes the quotient seminorm a norm. Completeness follows by choosing representatives of a rapidly Cauchy subsequence whose successive differences have summable norms in $X$.

### Approximate weakly null lifting through a quotient

↑ **Parent:** [Quotient Banach space](#quotient-banach-space)

If a [Banach space](banach-space.md) $X$ has separable dual and $q:X\to X/Y$ is a quotient by a closed subspace, every [weakly null sequence](weak-topology.md#weakly-null-sequence) in the quotient's closed unit ball has a subsequence with approximate weakly null lifts of norm at most $3$. Choose representatives of norm below $3/2$, pass to a common bidual weak-star limit, and subtract [convex blocks](#convex-block) whose quotient images tend to zero in norm. [Convex-block cancellation of a weak-star limit](#convex-block-cancellation-of-a-weak-star-limit) gives weak nullity and the triangle inequality gives the bound $3$.

### Quotient norm

↑ **Parent:** [Quotient Banach space](#quotient-banach-space)

The quotient norm measures the smallest norm among representatives of a coset. Its infimum need not be attained. Nevertheless, for every $\varepsilon>0$, an element $z\in X/Y$ has a representative $v\in X$ with $\|v\|<\|z\|+\varepsilon$. The [quotient map](topology.md#quotient-map) is contractive.

## Convex block

↑ **Parent:** [Banach space](banach-space.md)

A convex block of a sequence in a [Banach space](banach-space.md) is a sequence of [convex combinations](mathematical-optimization.md#convex-combination) supported on successively disjoint finite intervals, with $p_n<q_n<p_{n+1}$, $a_i\ge0$, and $\sum_{i=p_n}^{q_n}a_i=1$. Zero coefficients can fill gaps and ensure strict endpoint inequalities. By the [Mazur theorem](hilbert-space.md#mazur-theorem), every [weakly null sequence](weak-topology.md#weakly-null-sequence) has convex blocks tending to zero in norm.

### Convex-block cancellation of a weak-star limit

↑ **Parent:** [Convex block](#convex-block)

If a bounded sequence $(y_n)$ in $X$ converges weak-star to $\phi\in X^{**}$ under the [canonical embedding into the bidual](functional-analysis.md#canonical-embedding-into-the-bidual), then any [convex blocks](#convex-block) $(u_n)$ have the same scalar limit on every $f\in X^*$. Thus $y_n-u_n$ is a [weakly null sequence](weak-topology.md#weakly-null-sequence), even when $\phi$ does not belong to the embedded space $X$.

## Duality mapping

↑ **Parent:** [Banach space](banach-space.md)

The [duality mapping](#duality-mapping) takes a vector to its supporting dual functionals for half its squared [norm](functional-analysis.md#norm). Equivalently $p\in\mathcal J(x)$ when $\|p\|_* =\|x\|$ and $\langle x,p\rangle=\|x\|^2$. This follows from the dual-norm inequality and equality in the conjugate relation for squared norms. In a [Hilbert space](hilbert-space.md), the [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) identifies it with the identity; in a general [Banach space](banach-space.md) it can be set-valued.

## Bounded scalar functions on an index set

↑ **Parent:** [Banach space](banach-space.md)

For an arbitrary set $\Gamma$ and scalar field $\mathbb F$, this is the space of bounded functions $u:\Gamma\to\mathbb F$ with the [supremum norm](functional-analysis.md#supremum-norm) $\|u\|=\sup_\gamma|u(\gamma)|$. Uniform limits of Cauchy sequences prove it is a [Banach space](banach-space.md). For $\Gamma=\mathbb N$ it is the [l-infinity sequence space](#l-infinity-sequence-space); for the empty index set it is the zero space, with norm zero.

### Coordinate functional representation of an operator into bounded indexed functions

↑ **Parent:** [Bounded scalar functions on an index set](#bounded-scalar-functions-on-an-index-set)

A [bounded linear operator](topological-vector-space.md#continuous-linear-operator) $T:X\to\ell_\infty(\Gamma)$ is exactly a uniformly bounded family of [bounded linear functionals](topological-vector-space.md#continuous-linear-functional) $f_\gamma\in X^*$ through $(Tx)(\gamma)=f_\gamma(x)$. Evaluation shows $\|f_\gamma\|\le\|T\|$; conversely the family bound gives $\|Tx\|\le(\sup\|f_\gamma\|)\|x\|$, proving equality. Taking all functionals in the dual unit ball gives an [isometric embedding](riemannian-geometry.md#isometric-embedding) by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem).

## Separable Banach space

↑ **Parent:** [Banach space](banach-space.md)

A [Banach space](banach-space.md) is separable when it has a countable [dense subset](topology.md#dense-set) for its [norm topology](functional-analysis.md#norm-topology). It then has a countable base of norm balls and a [countable norming family](functional-analysis.md#countable-norming-family). Its [continuous dual space](continuous-dual-space.md) need not be norm separable.

## l-p sequence space

↑ **Parent:** [Banach space](banach-space.md)

For $1\le p<\infty$, the space $\ell^p$ consists of scalar sequences $x=(x_n)$ satisfying

$$
\|x\|_p=\left(\sum_{n=1}^\infty|x_n|^p\right)^{1/p}<\infty.
$$

It is a [Banach space](banach-space.md), and $\ell^q\subset\ell^p$ when $1\le q<p$.

As a [Lebesgue space](measure-theory.md#lp-space) it uses counting measure; as a space of sequences it is a [sequence space](vector-space.md#sequence-space).

### Absolutely summable sequence space

↑ **Parent:** [L-p sequence space](#l-p-sequence-space)

The [Banach space](banach-space.md) $\ell^1$ consists of absolutely summable scalar sequences, with [norm](functional-analysis.md#norm) $\|x\|_1=\sum_n|x_n|$. Its continuous dual is $\ell^\infty$, under the pairing $\sum_nx_ny_n$. Finitely supported sequences are [norm](functional-analysis.md#norm) dense, which identifies a [linear functional](linear-algebra.md#linear-functional) from its values on coordinate vectors. The [space of sequences converging to zero](functional-analysis.md#space-of-sequences-converging-to-zero) inside this dual is a [norming subspace](continuous-dual-space.md#norming-subspace-of-a-dual-space) of infinite codimension.

### l2 sequence space

↑ **Parent:** [L-p sequence space](#l-p-sequence-space)

The space $\ell^2$ consists of scalar sequences $x=(x_n)$ satisfying $\sum_n|x_n|^2<\infty$. With inner product $\langle x,y\rangle=\sum_nx_n\overline{y_n}$, it is a [Hilbert space](hilbert-space.md).

#### Uniform convexity of l2

↑ **Parent:** [L2 sequence space](#l2-sequence-space)

The [l2 sequence space](#l2-sequence-space) is a [uniformly convex Banach space](#uniformly-convex-banach-space). If $\lVert x\rVert_2=\lVert y\rVert_2=1$, the [parallelogram law](linear-algebra.md#parallelogram-law) gives

$$
\left\lVert\frac{x+y}{2}\right\rVert_2^2
=1-\frac14\lVert x-y\rVert_2^2.
$$

Thus $\lVert x-y\rVert_2\geq\varepsilon$ permits the modulus $\delta(\varepsilon)=1-\sqrt{1-\varepsilon^2/4}$.

### Finitely supported sequence

↑ **Parent:** [L-p sequence space](#l-p-sequence-space)

A finitely supported sequence has only finitely many nonzero coordinates. Their vector space is commonly denoted $c_{00}$.

#### Density of finitely supported sequences in l-p

↑ **Parent:** [Finitely supported sequence](#finitely-supported-sequence)

For $1\leq p<\infty$, coordinate truncations converge in $\ell^p$, so $c_{00}$ is dense. It is not dense in $\ell^\infty$: every finitely supported sequence is at distance at least one from the constant-one sequence.

## l-infinity sequence space

↑ **Parent:** [Banach space](banach-space.md)

The space $\ell^\infty$ consists of bounded scalar sequences with norm $\lVert x\rVert_\infty=\sup_n|x_n|$.

It is the bounded-sequence example of a [sequence space](vector-space.md#sequence-space).

### Generalized limit

↑ **Parent:** [L-infinity sequence space](#l-infinity-sequence-space)

A generalized limit on real bounded sequences is a [positive linear functional](continuous-dual-space.md#positive-linear-functional) of [operator norm](continuous-dual-space.md#operator-norm) one that extends the ordinary [limit of a sequence](real-analysis.md#limit-of-a-sequence). Such a functional can be chosen by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem): extend the limit on the [convergent sequence space](functional-analysis.md#convergent-sequence-space) while dominating it by the [sublinear functional](functional-analysis.md#sublinear-function) $p(x)=\limsup_n x_n$. Applying the same domination to $-x$ gives the displayed lower bound. A [Banach limit](#banach-limit) additionally has invariance under the [left shift on bounded sequences](#left-shift-on-bounded-sequences).

### Banach limit

↑ **Parent:** [L-infinity sequence space](#l-infinity-sequence-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Banach_limit)

A Banach limit is a [positive linear functional](continuous-dual-space.md#positive-linear-functional) on the real [l-infinity sequence space](#l-infinity-sequence-space) that extends the ordinary limit on the [convergent sequence space](functional-analysis.md#convergent-sequence-space), has [operator norm](continuous-dual-space.md#operator-norm) one, and is invariant under the [left shift on bounded sequences](#left-shift-on-bounded-sequences). The [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) constructs one by separating the constant sequence $\mathbf1$ from the subspace $(I-S)\ell^\infty$, whose distance from $\mathbf1$ is one. The functional is generally not unique.

<h4 id="cesaro-construction-of-a-banach-limit">Cesàro construction of a Banach limit</h4>

↑ **Parent:** [Banach limit](#banach-limit)

The displayed [sublinear functional](functional-analysis.md#sublinear-function) on the real [l-infinity sequence space](#l-infinity-sequence-space) agrees with the ordinary limit on [convergent sequences](real-analysis.md#convergent-sequence). A dominated extension by the [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) therefore defines a [generalized limit](#generalized-limit) bounded between the lower and upper limits of the [Cesaro means](real-analysis.md#cesaro-mean). For the [left shift on bounded sequences](#left-shift-on-bounded-sequences) $S$, the averages of $Sx-x$ equal $(x_{N+1}-x_1)/N$, which tend to zero. Domination applied to both signs gives $L(Sx-x)=0$, hence shift invariance. Positivity, agreement on constant sequences and the [operator norm](continuous-dual-space.md#operator-norm) one follow from the bounds, so $L$ is a [Banach limit](#banach-limit).

#### Ultrafilter construction of a Banach limit

↑ **Parent:** [Banach limit](#banach-limit)

A [nonprincipal ultrafilter](set-theory.md#nonprincipal-ultrafilter) on the [natural numbers](arithmetic.md#natural-number) gives a [Banach limit](#banach-limit) by taking the [ultralimit](set-theory.md#ultralimit) of the [Cesaro means](real-analysis.md#cesaro-mean) of each bounded sequence. Compactness of a closed bounded interval, or disk for complex sequences, supplies the limit. Finite intersections in the filter give linearity; nonnegative averages give positivity; constants give norm one. The [Cesaro theorem for convergent sequences](real-analysis.md#cesaro-theorem-for-convergent-sequences) gives agreement with ordinary limits because the ultrafilter contains every cofinite set. For the [left shift on bounded sequences](#left-shift-on-bounded-sequences), the two means differ by $(x_{n+1}-x_1)/n$, which tends to zero, proving shift invariance.

### Left shift on bounded sequences

↑ **Parent:** [L-infinity sequence space](#l-infinity-sequence-space)

The left shift is a [bounded linear operator](topological-vector-space.md#continuous-linear-operator) of [operator norm](continuous-dual-space.md#operator-norm) one on the [l-infinity sequence space](#l-infinity-sequence-space). For $y=x-Sx$, telescoping gives $N^{-1}\sum_{n=1}^Ny_n=(x_1-x_{N+1})/N\to0$. This identity is useful in constructing a [Banach limit](#banach-limit).

<h2 id="riesz-s-lemma">Riesz's lemma</h2>

↑ **Parent:** [Banach space](banach-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz's_lemma)

If $Y$ is a proper closed subspace of a normed space $X$ and $0<\alpha<1$, there is a unit vector $x\in X$ whose distance from $Y$ exceeds $\alpha$.

### Compact unit ball characterizes finite-dimensional normed spaces

↑ **Parent:** [Riesz's lemma](#riesz-s-lemma)

A normed vector space has compact closed unit ball if and only if it is finite-dimensional. In an infinite-dimensional space, repeated application of [Riesz lemma](#riesz-s-lemma) produces unit vectors separated pairwise by a fixed positive distance, contradicting sequential compactness.

## Uniformly convex Banach space

↑ **Parent:** [Banach space](banach-space.md)

A Banach space $X$ is uniformly convex when, for every $\varepsilon>0$, some $\delta>0$ satisfies

$$
\lVert x\rVert,\lVert y\rVert\leq1,
\quad \lVert x-y\rVert\geq\varepsilon
\quad\Longrightarrow\quad
\left\lVert\frac{x+y}{2}\right\rVert\leq1-\delta.
$$

This is a complete [uniformly convex space](functional-analysis.md#uniformly-convex-space).

### Nearest point in a uniformly convex Banach space

↑ **Parent:** [Uniformly convex Banach space](#uniformly-convex-banach-space)

Every nonempty closed convex subset of a uniformly convex [Banach space](banach-space.md) has a unique nearest point to each vector. A minimizing sequence is Cauchy: otherwise uniform convexity would put some midpoint strictly closer than the infimum. Completeness and closedness give its limiting point. In $\ell^p$, $p\geq2$, the [Clarkson inequality](#clarkson-s-inequalities) makes this quantitative: the distance between two minimizing vectors tends to zero after subtracting the midpoint's lower distance bound. Nonemptiness is required.

<h3 id="clarkson-s-inequalities">Clarkson's inequalities</h3>

↑ **Parent:** [Uniformly convex Banach space](#uniformly-convex-banach-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clarkson's_inequalities)

For $2\leq p<\infty$, the Clarkson inequality is

$$
\left\lVert\frac{f+g}{2}\right\rVert_p^p
+\left\lVert\frac{f-g}{2}\right\rVert_p^p
\leq\frac{\lVert f\rVert_p^p+\lVert g\rVert_p^p}{2}.
$$

For $1<p\leq2$ and $q=p/(p-1)$, the other [Clarkson inequality](#clarkson-s-inequalities) is

$$
\left\lVert\frac{f+g}{2}\right\rVert_p^q+\left\lVert\frac{f-g}{2}\right\rVert_p^q\leq\left(\frac{\lVert f\rVert_p^p+\lVert g\rVert_p^p}{2}\right)^{q/p}.
$$

Together these inequalities prove uniform convexity of $L^p$ for $1<p<\infty$.

#### Dual-exponent Clarkson inequality

↑ **Parent:** [Clarkson's inequalities](#clarkson-s-inequalities)

For $p\geq2$ and $p'=p/(p-1)$, interpolate the two-coordinate map $(x,y)\mapsto(x+y,x-y)$ between $\ell^1\to\ell^\infty$ [norm](functional-analysis.md#norm) one and $\ell^2\to\ell^2$ [norm](functional-analysis.md#norm) $\sqrt2$. This proves the scalar inequality with factor $2^{1/p}$. Integrating that estimate and applying [Minkowski inequality](real-analysis.md#minkowski-inequality) to $|f|^{p'}+|g|^{p'}$ in $L^{p/p'}$ gives the displayed function inequality.

## Uniform boundedness principle

↑ **Parent:** [Banach space](banach-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_boundedness_principle)

If a family of bounded linear operators from a Banach space to a normed space is pointwise bounded, then their operator norms are uniformly bounded.

### Weak boundedness implies norm boundedness

↑ **Parent:** [Uniform boundedness principle](#uniform-boundedness-principle)

A subset of a normed space is norm bounded if it is bounded under every continuous linear functional. Apply the [Uniform boundedness principle](#uniform-boundedness-principle) on the complete dual space to the evaluation family $f\mapsto f(x)$. [Hahn-Banach theorem](functional-analysis.md#hahn-banach-theorem) identifies the evaluation norm with $\|x\|$, even when the original normed space is not complete. As a consequence, two norms with exactly the same continuous dual as sets must be equivalent: apply this criterion to either norm's unit ball in the other norm.

### Uniform bound from pointwise absolute summability of dual evaluations

↑ **Parent:** [Uniform boundedness principle](#uniform-boundedness-principle)

Let $(x_n)$ lie in a normed space $X$ and suppose $\sum_n|f(x_n)|<\infty$ for every $f\in X^*$. Then some $C$ satisfies

$$
\sum_n|f(x_n)|\leq C\lVert f\rVert
\qquad(f\in X^*).
$$

Apply the uniform boundedness principle on the Banach space $X^*$ to the finite signed sums $f\mapsto\sum_na_nf(x_n)$ with $|a_n|\leq1$.

## ↑ Ancestors (6)

1. [Normed vector space](functional-analysis.md#normed-vector-space)
2. [Functional analysis](functional-analysis.md)
3. [Analysis](analysis.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (186)

- [A posteriori contraction ball](analysis.md#a-posteriori-contraction-ball)
- [Absolutely p-summing operator](topological-vector-space.md#absolutely-p-summing-operator)
- [Absolutely summable sequence space](#absolutely-summable-sequence-space)
- [Approximate surjectivity with geometric correction](topological-vector-space.md#approximate-surjectivity-with-geometric-correction)
- [Approximate weakly null lifting through a quotient](#approximate-weakly-null-lifting-through-a-quotient)
- [Banach-Mazur distance](functional-analysis.md#banach-mazur-distance)
- [Banach norm rigidity from continuous point evaluations](functional-analysis.md#banach-norm-rigidity-from-continuous-point-evaluations)
- [Banach-Saks property](#banach-saks-property)
- [Banach space has uncountable Hamel dimension](topological-analysis.md#banach-space-has-uncountable-hamel-dimension)
- [Banach space of bounded linear operators](topological-vector-space.md#banach-space-of-bounded-linear-operators)
- [Banach-space proximal minimization](convex-optimization.md#banach-space-proximal-minimization)
- [Banach-space-valued holomorphic function](complex-analysis.md#banach-space-valued-holomorphic-function)
- [Banach–Stone theorem](functional-analysis.md#banach-stone-theorem)
- [Bidual characterization of weakly compact operators](functional-analysis.md#bidual-characterization-of-weakly-compact-operators)
- [Bochner integral](measure-theory.md#bochner-integral)
- [Bounded continuous functions](calculus.md#bounded-continuous-functions)
- [Bounded scalar functions on an index set](#bounded-scalar-functions-on-an-index-set)
- [Bourgain l1-index](functional-analysis.md#bourgain-l1-index)
- [Classical solution of an abstract Cauchy problem](functional-analysis.md#classical-solution-of-an-abstract-cauchy-problem)
- [Coefficient Banach space for normalized even maps](dynamical-systems.md#coefficient-banach-space-for-normalized-even-maps)
- [Complemented subspace](#complemented-subspace)
- [Completely continuous operator](topological-vector-space.md#completely-continuous-operator)
- [Completeness forced by uniformly bounded lifting](functional-analysis.md#completeness-forced-by-uniformly-bounded-lifting)
- [Completion of a normed space](functional-analysis.md#completion-of-a-normed-space)
- [Continuous functions on the p-adic integers](arithmetic.md#continuous-functions-on-the-p-adic-integers)
- [Convex block](#convex-block)
- [Cotype 2 extrapolation on finite-dimensional linfinity](#cotype-2-extrapolation-on-finite-dimensional-linfinity)
- [Cotype of a Banach space](#cotype-of-a-banach-space)
- [Dense open-unit-ball image criterion](functional-analysis.md#dense-open-unit-ball-image-criterion)
- [Disconnected spectrum yields a nontrivial invariant subspace](banach-algebra.md#disconnected-spectrum-yields-a-nontrivial-invariant-subspace)
- [Duality mapping](#duality-mapping)
- [Extension of a bounded linear operator from a dense subspace](topological-vector-space.md#extension-of-a-bounded-linear-operator-from-a-dense-subspace)
- [Fenchel-Moreau theorem](convex-optimization.md#fenchel-moreau-theorem)
- [Finite codimension in a Banach space](#finite-codimension-in-a-banach-space)
- [Finite-codimensional weak-star dense dual subspace is norming](continuous-dual-space.md#finite-codimensional-weak-star-dense-dual-subspace-is-norming)
- [Function of bounded variation on a domain](inverse-problem.md#function-of-bounded-variation-on-a-domain)
- [Generalized singular vector](convex-optimization.md#generalized-singular-vector)
- [Generic unbounded Fourier sums at a fixed point](fourier-series.md#generic-unbounded-fourier-sums-at-a-fixed-point)
- [Geometric correction for approximate surjectivity](functional-analysis.md#geometric-correction-for-approximate-surjectivity)
- [Gliding-hump continuity principle](functional-analysis.md#gliding-hump-continuity-principle)
- [Gowers dichotomy theorem](#gowers-dichotomy-theorem)
- [Graph norm](functional-analysis.md#graph-norm)
- [Hadamard three-circle theorem](complex-analysis.md#hadamard-three-circle-theorem)
- [Hellinger bound for differences of expectations](probability-and-statistics.md#hellinger-bound-for-differences-of-expectations)
- [Kadec-Snobar projection bound](vector-space.md#kadec-snobar-projection-bound)
- [L-p sequence space](#l-p-sequence-space)
- [Lanford contraction proof of the Feigenbaum fixed point](dynamical-systems.md#lanford-contraction-proof-of-the-feigenbaum-fixed-point)
- [Nearest point in a uniformly convex Banach space](#nearest-point-in-a-uniformly-convex-banach-space)
- [Newton iteration in a Banach space](numerical-analysis.md#newton-iteration-in-a-banach-space)
- [Norm-closedness of compact operators](compact-operator.md#norm-closedness-of-compact-operators)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-53.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-10.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-10.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-10.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-10.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-11.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-11.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-11.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-11.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-8.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-8.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-8.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#22f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-13.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#22h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#22h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#22h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#22h/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-8.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#22h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#22h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-64.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#22g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#26k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-6.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-64.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-6.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-7.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#10i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5.md#2/9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-8.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-106.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#21f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#20f/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#20f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#20f/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-106.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#3/5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326.md#4/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#22f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#21f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#21f/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#1/1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326.md#3/2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#22h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#21h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#22h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#22i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#22i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#22i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#22i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-105.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326.md#4/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#22g/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-319.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-319.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-319.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-319.md#1/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#22f/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-319.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-106.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-107.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-106.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-202.md#2/a/solution)
- [Pełczyński decomposition method](#pelczynski-decomposition-method)
- [Positive distance between a unit sphere and a disjoint finite-dimensional subspace](vector-space.md#positive-distance-between-a-unit-sphere-and-a-disjoint-finite-dimensional-subspace)
- [Primitive ideal](associative-algebra.md#primitive-ideal)
- [Quotient Banach space](#quotient-banach-space)
- [Reflexive space](functional-analysis.md#reflexive-space)
- [Rosenthal l1 theorem](functional-analysis.md#rosenthal-l1-theorem)
- [Schauder basis](functional-analysis.md#schauder-basis)
- [Schauder theorem for compact operators](compact-operator.md#schauder-theorem-for-compact-operators)
- [Schur property](continuous-dual-space.md#schur-property)
- [Semigroup restricted to its generator domain](functional-analysis.md#semigroup-restricted-to-its-generator-domain)
- [Semisimple Banach algebra](banach-algebra.md#semisimple-banach-algebra)
- [Separable Banach space](#separable-banach-space)
- [Separating space of a linear map](functional-analysis.md#separating-space-of-a-linear-map)
- [Source-condition estimate for symmetric Bregman distance](inverse-problem.md#source-condition-estimate-for-symmetric-bregman-distance)
- [Space of continuous functions on a compact space](functional-analysis.md#space-of-continuous-functions-on-a-compact-space)
- [Spreading model](functional-analysis.md#spreading-model)
- [Strongly measurable function](measure-theory.md#strongly-measurable-function)
- [Sum of Lp spaces](measure-theory.md#sum-of-lp-spaces)
- [Weak compactness characterization of reflexivity](functional-analysis.md#weak-compactness-characterization-of-reflexivity)
- [Weak compactness of an operator and its adjoint](functional-analysis.md#weak-compactness-of-an-operator-and-its-adjoint)
- [Weak-star fixed point theorem for an adjoint operator](weak-topology.md#weak-star-fixed-point-theorem-for-an-adjoint-operator)
- [Weak-star separability of the entire dual](weak-topology.md#weak-star-separability-of-the-entire-dual)
- [Weak-star topology on an entire infinite-dimensional Banach dual is not metrizable](weak-topology.md#weak-star-topology-on-an-entire-infinite-dimensional-banach-dual-is-not-metrizable)
- [Weighted holomorphic norm on a shrinking time domain](complex-analysis.md#weighted-holomorphic-norm-on-a-shrinking-time-domain)
