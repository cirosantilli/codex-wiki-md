<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Suppose first that $X$ is separable, and choose a norm-dense sequence $(x_n)$ in its unit ball. On the dual unit ball define

$$
d(f,g)=\sum_{n=1}^\infty2^{-n}
\frac{|(f-g)(x_n)|}{1+|(f-g)(x_n)|}.
$$

Uniform boundedness on the unit ball and density of the $x_n$ show that this metric induces the weak-star topology. Conversely, if $B_{X^*}$ is weak-star metrizable, the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes it a compact metric space. Hence $C(B_{X^*})$ is separable. The evaluation map

$$
X\longrightarrow C(B_{X^*}),\qquad
x\longmapsto(f\mapsto f(x))
$$

is an isometry by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). A subspace of a separable metric space is separable, so $X$ is separable. This proves the [weak-star metrizability criterion for a dual ball](../../../../../weak-star-metrizability-criterion-for-a-dual-ball.md).

If $X$ has a countable weakly dense subset $D$, the rational linear span of $D$ is weakly dense. Its norm closure is a convex set, so [Mazur theorem](../../../../../mazur-theorem.md) says that its weak and norm closures agree. Thus $X$ is norm separable. The weak-star compact metric ball $B_{X^*}$ consequently has a countable weak-star dense subset, and the union of its integer dilates is weak-star dense in $X^*$. Therefore $X^*$ is weak-star separable.

It need not be weakly separable. Take $X=\ell^1$, whose dual is $\ell^\infty$. A weakly separable normed space is norm separable by the preceding convex-closure argument, whereas $\ell^\infty$ is not norm separable.

If the Banach space $X$ is reflexive, its closed unit ball identifies with the weak-star compact ball of $X^{**}$, hence is weakly compact. Conversely, if $B_X$ is weakly compact, its canonical image $J(B_X)$ is weak-star compact and therefore weak-star closed in $X^{**}$. [Goldstine theorem](../../../../../goldstine-theorem.md) says it is weak-star dense in $B_{X^{**}}$, so

$$
J(B_X)=B_{X^{**}}.
$$

Scaling proves that $J$ is surjective and $X$ is reflexive. This is the [weak compactness characterization of reflexivity](../../../../../weak-compactness-characterization-of-reflexivity.md).

The [Krein-Milman theorem](../../../../../krein-milman-theorem.md) says that a nonempty compact convex subset of a locally convex space is the closed convex hull of its extreme points. For reflexive $X$, the ball $B_X$ is weakly compact, so

$$
B_X=\overline{\operatorname{conv}}\operatorname{Ext}(B_X),
$$

where weak and norm closure agree for the convex hull by Mazur's theorem.

For the final claim, let $\mathcal H$ be the set of functions $\mathbb Z^2\to[0,1]$ with the mean-value property. It is a compact convex subset of the product $[0,1]^{\mathbb Z^2}$. If $f$ is extreme, its four unit translates also lie in $\mathcal H$, and the mean-value identity writes $f$ as their average. Extremality forces every translate to equal $f$, so $f$ is constant. Every extreme point is therefore constant. Krein--Milman now makes every member of $\mathcal H$ a limit of convex combinations of constant functions, and hence constant. This is the [bounded harmonic function theorem on the integer lattice](../../../../../bounded-harmonic-function-theorem-on-the-integer-lattice.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
