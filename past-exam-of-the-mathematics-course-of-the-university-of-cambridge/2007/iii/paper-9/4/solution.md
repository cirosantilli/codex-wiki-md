<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a $d$-dimensional [normed vector space](../../../../../normed-vector-space.md), with [unit ball](../../../../../unit-ball.md) $K$ and [John ellipsoid](../../../../../john-ellipsoid.md) $\mathcal E$, its [volume ratio](../../../../../volume-ratio.md) is

$$
\operatorname{vr}(E)=\left(\frac{\operatorname{vol}K}{\operatorname{vol}\mathcal E}\right)^{1/d}.
$$

It is at least $1$ and invariant under invertible linear coordinate changes.

For $\ell_1^n$, the [unit ball](../../../../../unit-ball.md) has volume $2^n/n!$: its intersection with each orthant is the standard simplex of volume $1/n!$. Its [John ellipsoid](../../../../../john-ellipsoid.md) is $n^{-1/2}B_2^n$. To verify maximum volume, let $AB_2^n$ be any centered inscribed [ellipsoid](../../../../../ellipsoid.md). For each sign vector $\varepsilon\in\{-1,1\}^n$, containment gives $|A^T\varepsilon|\leq1$. Averaging over independent [Rademacher random variables](../../../../../rademacher-distribution.md) yields $\operatorname{tr}(AA^T)\leq1$. The [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) for its squared [singular values](../../../../../singular-value.md) gives $|\det A|\leq n^{-n/2}$. The scalar [matrix](../../../../../matrix.md) $n^{-1/2}I$ attains this bound because $\|x\|_1\leq\sqrt n|x|$. Centered [ellipsoids](../../../../../ellipsoid.md) suffice: if $a+AB_2^n$ is contained in the symmetric convex [unit ball](../../../../../unit-ball.md), averaging it with $-a+AB_2^n$ gives the centered copy with the same volume.

Using the stated [Euclidean ball](../../../../../euclidean-ball.md) volume and $n=2k$,

$$
\operatorname{vr}(\ell_1^{2k})^{2k}
=\frac{2^{2k}(2k)^k k!}{(2k)!\pi^k}
\leq\left(\frac8\pi\right)^k,
$$

since $(2k)!/k!=\prod_{j=k+1}^{2k}j\geq k^k$. Therefore **$\operatorname{vr}(\ell_1^{2k})\leq\sqrt{8/\pi}$ uniformly in $k$**.

**The subsequent assertion for an arbitrary $2k$-dimensional space is false as printed.** Here is a counterexample independent of any asymptotic section theorem. Take $E=\ell_\infty^{2k}$. Its [John ellipsoid](../../../../../john-ellipsoid.md) is $B_2^{2k}$: an inscribed $AB_2^{2k}$ has every row of $A$ of Euclidean length at most $1$, so the [Hadamard inequality](../../../../../hadamard-determinant-inequality.md) gives $|\det A|\leq1$, attained by $A=I$. Let $F$ be any $k$-dimensional subspace and $f_1,\ldots,f_k$ an [orthonormal basis](../../../../../orthonormal-basis.md) of it. The random unit vector

$$
x=\frac1{\sqrt k}\sum_{j=1}^k\varepsilon_j f_j
$$

has $|x|=1$. Since $\sum_j f_j(i)^2\leq1$ for each coordinate $i$, the [moment-generating function](../../../../../moment-generating-function.md) bound for independent [Rademacher random variables](../../../../../rademacher-distribution.md) gives

$$
\mathbb E e^{t x_i}\leq e^{t^2/(2k)},\qquad
\mathbb P(\|x\|_\infty>r)\leq4k\,e^{-kr^2/2}.
$$

Choose $r=\sqrt{2\log(8k)/k}$; the latter [probability](../../../../../probability.md) is at most $1/2$, so some unit vector in $F$ has $\|x\|_\infty\leq r$. The proposed section inequality would therefore force

$$
\boxed{L\geq\sqrt{\frac{k}{2\log(8k)}}\longrightarrow\infty}.
$$

Thus even one half-dimensional section cannot have the printed universal constant.

The valid [orthogonal splitting with bounded volume ratio](../../../../../orthogonal-splitting-with-bounded-volume-ratio.md) is that $L$ may depend on $V=\operatorname{vr}(E)$, and **$L=32V^2$ suffices**. This supplies a dimension-independent constant for the preceding $\ell_1^{2k}$ case, or whenever $V$ is bounded uniformly. We prove the complete qualified assertion, including its [epsilon-net](../../../../../metric-epsilon-net.md) ingredient.

In [John position](../../../../../john-position.md), $\|x\|_E\leq|x|$. Polar integration of the radial function $\rho(u)=1/\|u\|_E$ gives

$$
V^{2k}=\frac{\operatorname{vol}K}{\operatorname{vol}B_2^{2k}}
=\int_{S^{2k-1}}\|u\|_E^{-2k}\,d\sigma(u),\qquad
\sigma\{\|u\|_E\leq r\}\leq(Vr)^{2k},
$$

where $\sigma$ is normalized spherical measure.

A maximal $\varepsilon$-separated subset of $S^{k-1}$ is an [epsilon-net](../../../../../metric-epsilon-net.md). Balls of radius $\varepsilon/2$ about its points have disjoint interiors and lie in the ball of radius $1+\varepsilon/2$. Comparing volumes bounds its [cardinality](../../../../../cardinality.md) by $(1+2/\varepsilon)^k$. Finite existence follows from this packing bound, and maximality proves the net property without assuming a separate covering theorem.

Choose two orthogonal $k$-dimensional subspaces $F_0,F_0^\perp$ and one such net on each [unit sphere](../../../../../unit-sphere.md). Rotate both by a common uniformly distributed orthogonal [matrix](../../../../../matrix.md) $U$. This distribution can be obtained from Question 1 applied to the compact [orthogonal group](../../../../../orthogonal-group.md) with its Frobenius [metric](../../../../../metric.md); left and right multiplication are transitive [isometries](../../../../../isometry.md). Consequently $Uv$ is uniformly distributed on $S^{2k-1}$ for every fixed unit vector $v$. The [union bound](../../../../../boole-s-inequality.md) shows that the [probability](../../../../../probability.md) that some rotated net point has [norm](../../../../../norm.md) less than $2\varepsilon$ is at most

$$
2(1+2/\varepsilon)^k(2V\varepsilon)^{2k}
=2\left[4V^2(\varepsilon^2+2\varepsilon)\right]^k.
$$

Set $\varepsilon=(32V^2)^{-1}$. Because $V\geq1$, the bracket is at most $1/4+1/256$, and twice its $k$th power is less than $1$ for every $k\geq1$. Some rotation therefore makes every point of both nets have [norm](../../../../../norm.md) at least $2\varepsilon$.

The [triangle inequality](../../../../../triangle-inequality.md) and $\|x\|_E\leq|x|$ imply that $\|\cdot\|_E$ is $1$-[Lipschitz](../../../../../lipschitz-continuity.md) for the [Euclidean metric](../../../../../euclidean-metric.md). Every unit vector of $UF_0$ or $UF_0^\perp$ is within $\varepsilon$ of a good net point and thus has [norm](../../../../../norm.md) at least $\varepsilon$. By homogeneity, on both orthogonal subspaces,

$$
\boxed{\|x\|_E\leq |x|\leq32\operatorname{vr}(E)^2\|x\|_E}.
$$

For $\ell_1^{2k}$ the first computation gives the absolute choice $L=256/\pi$. The missing bounded-[volume ratio](../../../../../volume-ratio.md) restriction is essential; the literal unrestricted assertion cannot be proved.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
