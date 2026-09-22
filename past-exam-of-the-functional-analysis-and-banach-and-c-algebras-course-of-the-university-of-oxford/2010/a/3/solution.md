<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [weak topology](../../../../weak-topology-split.md) $\sigma(X,X^*)$ is the coarsest [topology](../../../../topology-split.md) making every $f\in X^*$ continuous. Its basic neighbourhoods impose finitely many inequalities $|f_j(x-x_0)|<\varepsilon$. The [weak-star topology](../../../../weak-star-topology.md) $\sigma(X^*,X)$ is the coarsest [topology](../../../../topology-split.md) making each evaluation $f\mapsto f(x)$ continuous, for $x\in X$.

The [canonical embedding into the bidual](../../../../canonical-embedding-into-the-bidual.md) is

$$
J_Xx\in X^{**},\qquad(J_Xx)(f)=f(x).
$$

It is linear and $\|J_Xx\|\leq\|x\|$. For $x\ne0$, the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) supplies a [norming functional](../../../../norming-functional.md) $f$ with $\|f\|=1$ and $f(x)=\|x\|$, proving equality. Thus $J_X$ is an [isometric embedding](../../../../isometric-embedding.md). The coordinates defining the [weak-star topology](../../../../weak-star-topology.md) on $X^{**}$, restricted to $J_X(X)$, are precisely $J_Xx\mapsto f(x)$ for $f\in X^*$. These are exactly the coordinates defining the [weak topology](../../../../weak-topology-split.md) on $X$, so $J_X$ is also a [topological embedding](../../../../topological-embedding.md) for these [topologies](../../../../topology-split.md).

A [normed vector space](../../../../normed-vector-space-split.md) is a [reflexive space](../../../../reflexive-space.md) if $J_X$ is onto $X^{**}$. Such a space is automatically a [Banach space](../../../../banach-space-split.md), since it is isometric to the complete [continuous dual space](../../../../continuous-dual-space-split.md) $X^{**}$. The [Banach-Alaoglu theorem](../../../../banach-alaoglu-theorem.md) states that the closed unit ball of a [continuous dual space](../../../../continuous-dual-space-split.md) is compact for its [weak-star topology](../../../../weak-star-topology.md). The [Goldstine theorem](../../../../goldstine-theorem.md) states that $J_X(B_X)$ is dense in the [weak-star topology](../../../../weak-star-topology.md) in $B_{X^{**}}$. Consequently

$$
\boxed{X\text{ is reflexive}\iff B_X\text{ is weakly compact}.}
$$

If $J_X$ is onto, its weak-to-weak-star [homeomorphism](../../../../homeomorphism.md) carries $B_X$ onto the [Banach-Alaoglu theorem](../../../../banach-alaoglu-theorem.md)'s compact ball $B_{X^{**}}$. Conversely, if $B_X$ is [weakly compact](../../../../weakly-compact-set.md), $J_X(B_X)$ is compact and hence closed in the [Hausdorff](../../../../hausdorff-space.md) [weak-star topology](../../../../weak-star-topology.md). Its density from the [Goldstine theorem](../../../../goldstine-theorem.md) makes it all of $B_{X^{**}}$, and scaling gives surjectivity of $J_X$.

Now suppose $X$ is separable and nonzero. Choose a countable dense set $(u_n)$ in its unit sphere and, using the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md), choose [norming functionals](../../../../norming-functional.md) $f_n$ with $\|f_n\|=1$ and $f_n(u_n)=1$. These [continuous linear functionals](../../../../continuous-linear-functional.md) separate points: for $x\ne0$, choose $\|u_n-x/\|x\|\|<1/2$ to get $f_n(x)>\|x\|/2$. Define

$$
d(x,x')=\sum_{n\geq1}\min\{2^{-n},|f_n(x-x')|\}.
$$

The [series](../../../../series-mathematics.md) converges uniformly, separates distinct points, and obeys the [triangle inequality](../../../../triangle-inequality.md) because $\min(c,a+b)\leq\min(c,a)+\min(c,b)$. Thus $d$ is a [metric](../../../../metric.md). Its [topology](../../../../topology-split.md) is coarser than the [weak topology](../../../../weak-topology-split.md): a finite set of coordinate controls makes the finite initial sum small, while the remaining sum is at most $\sum_{n>N}2^{-n}=2^{-N}$. On a [weakly compact set](../../../../weakly-compact-set.md) $K$, the identity $(K,\text{weak})\to(K,d)$ is therefore a continuous bijection from a [compact space](../../../../compact-space.md) into a [Hausdorff space](../../../../hausdorff-space.md), hence a [homeomorphism](../../../../homeomorphism.md). This proves that **$K$ is metrizable in its [weak topology](../../../../weak-topology-split.md)**, an instance of [countable separating family metrizes a weakly compact set](../../../../countable-separating-family-metrizes-a-weakly-compact-set.md).

If $X$ is also a [reflexive space](../../../../reflexive-space.md), its closed unit ball is [weakly compact](../../../../weakly-compact-set.md) and therefore metrizable by this construction. Compactness in a [metric space](../../../../metric-space.md) implies [sequential compactness](../../../../sequentially-compact-space.md), so every sequence in $B_X$ has a [weakly convergent](../../../../weak-convergence.md) subsequence. Scaling proves the claim for every bounded sequence.

For the converse, assume every bounded sequence in $X$ has a [weakly convergent](../../../../weak-convergence.md) subsequence. Use the same [metric](../../../../metric.md) $d$ on $B_X$. A [weak limit](../../../../weak-limit.md) of points of $B_X$ remains in $B_X$: $|f(x)|\leq1$ for every $\|f\|\leq1$, and the [Hahn-Banach theorem](../../../../hahn-banach-theorem.md) recovers $\|x\|\leq1$. Thus every sequence in $B_X$ has a subsequence convergent in $d$ to a point of $B_X$, so $(B_X,d)$ is sequentially compact and hence compact.

We must still recover the entire [weak topology](../../../../weak-topology-split.md), rather than just the selected coordinates. Suppose $x_n\to x$ in $d$ but not weakly. There is a neighbourhood in the [weak topology](../../../../weak-topology-split.md) $U$ of $x$ and a subsequence outside $U$. By hypothesis that subsequence has a further subsequence converging weakly to $y\in B_X$. It then converges in $d$ to $y$, so uniqueness of [metric](../../../../metric.md) limits gives $y=x$, contradicting eventual membership in $U$. Hence convergence in $d$ implies [weak convergence](../../../../weak-convergence.md). Every $f\in X^*$ is therefore sequentially continuous on $(B_X,d)$ and hence continuous, since the domain is a [metric space](../../../../metric-space.md). The [weak topology](../../../../weak-topology-split.md) and $d$-topology on $B_X$ coincide. The ball is [weakly compact](../../../../weakly-compact-set.md), so the criterion above proves

$$
\boxed{X\text{ separable}:\quad X\text{ reflexive}\iff\text{every bounded sequence has a weakly convergent subsequence}.}
$$

The zero space satisfies all statements directly. The converse did not assume completeness, nor use the full [Eberlein-Šmulian theorem](../../../../eberlein-smulian-theorem.md).

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
