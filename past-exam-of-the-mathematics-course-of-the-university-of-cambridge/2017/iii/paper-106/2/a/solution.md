<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [weak topology](../../../../../../weak-topology-split.md) $\sigma(X,X^*)$ is the coarsest topology making every [bounded linear functional](../../../../../../continuous-linear-functional.md) continuous. A neighbourhood basis at $x$ consists of sets $\{y:|f_j(y-x)|<\epsilon,\ 1\le j\le m\}$ for finite families in $X^*$.

[Mazur theorem](../../../../../../mazur-theorem.md) says that for any [convex](../../../../../../convex-function.md) subset $C$ of a real or complex [normed vector space](../../../../../../normed-vector-space.md),

$$
\boxed{\overline C^{\,w}=\overline C^{\,\|\cdot\|}.}
$$

The [norm](../../../../../../norm.md) closure is [convex](../../../../../../convex-function.md). If $x$ is outside it, the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) gives a [bounded linear functional](../../../../../../continuous-linear-functional.md) $f$ and a real $a$ with $\operatorname{Re}f(x)>a\ge\sup_{y\in C}\operatorname{Re}f(y)$. In the real case omit the real part. Thus $x$ has a weak neighbourhood missing $C$, proving that the weak closure lies in the [norm](../../../../../../norm.md) closure. The other inclusion follows because the weak topology is weaker than the [norm](../../../../../../norm.md) topology. In the complex case real separation is converted to a complex functional by $f(z)=h(z)-ih(iz)$.

The sequential formulation, [Mazur lemma](../../../../../../mazur-s-lemma.md), follows as well. If $x_n\rightharpoonup x$, then $x$ lies in the weak closure of each tail and hence in the [norm](../../../../../../norm.md) closure of its [convex hull](../../../../../../convex-hull.md). Select a finite [convex](../../../../../../convex-function.md) combination of the $n$th tail at [norm](../../../../../../norm.md) distance less than $1/n$ from $x$.

A [weakly bounded set](../../../../../../weakly-bounded-set.md) $D$ satisfies $\sup_{x\in D}|f(x)|<\infty$ for every $f\in X^*$. Regard $J(D)$ as a pointwise bounded family of functionals on $X^*$. The [completeness of the dual space](../../../../../../completeness-of-the-dual-space.md) holds even if $X$ is incomplete: a norm-Cauchy sequence of functionals has a pointwise bounded linear limit and then converges uniformly on the [unit ball](../../../../../../unit-ball.md). The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) therefore gives $\sup_{x\in D}\|Jx\|<\infty$, and $\|Jx\|=\|x\|$ proves [norm](../../../../../../norm.md) boundedness.

One can see the precise Baire argument here. The closed sets $F_n=\{f\in X^*:\sup_{x\in D}|f(x)|\le n\}$ cover the [Banach space](../../../../../../banach-space-split.md) $X^*$. The [Baire category theorem](../../../../../../baire-category-theorem.md) makes some $F_n$ contain a ball $f_0+rB_{X^*}$, after shrinking the radius. For $\|g\|\le r$, both $f_0$ and $f_0+g$ lie in $F_n$, so $\sup_D|g(x)|\le2n$. Scaling and the dual [norm](../../../../../../norm.md) formula yield $\sup_D\|x\|\le2n/r$. A [weakly compact set](../../../../../../weakly-compact-set.md) is weakly bounded because each functional has compact, hence bounded, image. Consequently it is [norm](../../../../../../norm.md) bounded.

For a [Banach space](../../../../../../banach-space-split.md), let $J:X\to X^{**}$ be its canonical [isometry](../../../../../../isometry.md). We use two explicitly stated weak-star facts: [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) makes a dual [unit ball](../../../../../../unit-ball.md) weak-star compact, and [Goldstine theorem](../../../../../../goldstine-theorem.md) makes $J(B_X)$ weak-star dense in $B_{X^{**}}$. The weak topology on $X$ is carried by $J$ to $\sigma(X^{**},X^*)$ on its image, since their coordinates are the same evaluations $f(x)$.

If $X$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md), $J(B_X)=B_{X^{**}}$ and Banach-Alaoglu proves weak compactness. Conversely, if $B_X$ is weakly compact, its image is weak-star compact and hence closed in the [Hausdorff space](../../../../../../hausdorff-space.md) $X^{**}$. Goldstine density then forces $J(B_X)=B_{X^{**}}$, which implies $JX=X^{**}$. This proves the [weak compactness characterization of reflexivity](../../../../../../weak-compactness-characterization-of-reflexivity.md):

$$
\boxed{X\text{ is reflexive}\iff B_X\text{ is weakly compact}.}
$$

Finally let $K\subset X$ be weakly compact and let $(f_n)\subset B_{X^*}$ separate points. If $K$ is empty there is nothing to prove; otherwise define

$$
\boxed{d(x,y)=\sum_{n=1}^\infty 2^{-n}\frac{|f_n(x-y)|}{1+|f_n(x-y)|}.}
$$

The summands are bounded by $2^{-n}$ and separation makes $d(x,y)=0$ only for $x=y$. The coordinate maps are weakly continuous, so the series, being uniformly convergent, makes the identity from weak $K$ to metric $K$ continuous. A continuous bijection from a compact space to a [Hausdorff space](../../../../../../hausdorff-space.md) is a [homeomorphism](../../../../../../homeomorphism.md). Thus $d$ induces precisely the weak topology on $K$, the [countable separating family metrizes a weakly compact set](../../../../../../countable-separating-family-metrizes-a-weakly-compact-set.md) result. No norm-density of the separating family in $X^*$ is claimed or required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
