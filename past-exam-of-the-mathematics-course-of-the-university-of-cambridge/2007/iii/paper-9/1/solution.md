<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume $X$ is nonempty, as is necessary for a [probability measure](../../../../../probability-measure.md) to exist. Give its [isometry group](../../../../../isometry-group.md) $I_X$ the uniform [metric](../../../../../metric.md)

$$
D(g,h)=\sup_{x\in X}d(gx,hx).
$$

Every distance-preserving self-map of a [compact metric space](../../../../../compact-metric-space.md) is onto. Indeed, if $x_0\notin gX$, then $\delta=d(x_0,gX)>0$, and for $n>m$ the iterates satisfy $d(g^mx_0,g^nx_0)=d(x_0,g^{n-m}x_0)\geq\delta$. This infinite separated set contradicts [compactness](../../../../../compact-space.md). Consequently $I_X$ is a [group](../../../../../group-split.md) under composition, with the identity and inverses again [isometries](../../../../../isometry.md).

The [metric](../../../../../metric.md) $D$ is invariant under both left and right multiplication: left invariance uses preservation of distances, and right invariance uses surjectivity. Inversion is an [isometry](../../../../../isometry.md) for $D$, and $D(gh,g'h')\leq D(g,g')+D(h,h')$ proves continuity of multiplication. Moreover, $I_X$ is compact. A sequence of [isometries](../../../../../isometry.md) has a subsequence converging at every point of a countable dense subset of $X$, by a diagonal argument. Their common [Lipschitz constant](../../../../../lipschitz-constant.md) $1$ and finite [epsilon-nets](../../../../../metric-epsilon-net.md) of $X$ make this subsequence uniformly Cauchy. Its [uniform limit](../../../../../uniform-limit.md) preserves distances and is onto by the preceding argument. Thus **$I_X$ is a compact metrizable [topological group](../../../../../topological-group-split.md)**. A [transitive group action](../../../../../transitive-group-action.md) means that for every $x,y\in X$ some $g\in I_X$ has $gx=y$.

We construct the invariant [Borel probability measure](../../../../../borel-probability-measure.md) directly. The [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) says that a finite [bipartite graph](../../../../../bipartite-graph.md) with equal-sized vertex classes $A,B$ has a [perfect matching](../../../../../perfect-matching.md) precisely when every subset $S\subseteq A$ has at least $|S|$ neighbours in $B$. Its following consequence is useful. If $A,B$ are $\varepsilon$-separated subsets of maximum [cardinality](../../../../../cardinality.md) in a [compact metric space](../../../../../compact-metric-space.md), join points whose distance is less than $\varepsilon$. If some $S\subseteq A$ had fewer than $|S|$ neighbours, replacing those neighbours in $B$ by $S$ would produce a larger $\varepsilon$-separated set. This contradicts maximal [cardinality](../../../../../cardinality.md). Hence there is a bijection between $A$ and $B$ moving each point by less than $\varepsilon$.

Choose $\varepsilon_n\downarrow0$ and maximum-[cardinality](../../../../../cardinality.md) $\varepsilon_n$-separated sets $A_n\subset I_X$. Such sets exist: a finite covering by balls of radius less than $\varepsilon_n/2$ bounds every separated set's [cardinality](../../../../../cardinality.md). Fix $x_0\in X$ and define the empirical [probability measures](../../../../../probability-measure.md)

$$
\mu_n=\frac1{|A_n|}\sum_{a\in A_n}\delta_{ax_0}.
$$

For $f\in C(X)$ let $\omega_f(r)=\sup_{d(x,y)\leq r}|f(x)-f(y)|$, which tends to zero with $r$ by [uniform continuity](../../../../../uniform-continuity.md). For every $h\in I_X$, left invariance of $D$ makes $hA_n$ another maximum-[cardinality](../../../../../cardinality.md) separated set. Match it to $A_n$ as above. Then

$$
\left|\int f\,d\mu_n-\int f(hx)\,d\mu_n(x)\right|\leq\omega_f(\varepsilon_n).
$$

The allowed [compactness of probability measures on a compact metric space](../../../../../compactness-of-probability-measures-on-a-compact-metric-space.md) supplies a subsequence converging to $\mu$ in the [weak-star topology](../../../../../weak-star-topology.md). Passing to that limit for each fixed $h,f$ gives $\int f\,d\mu=\int f\circ h\,d\mu$. The same subsequence works for every $h,f$, since the displayed estimate held for all of them before taking the limit.

For uniqueness, put $F_n(x)=|A_n|^{-1}\sum_{a\in A_n}f(ax)$. For $x=hx_0$, right invariance of $D$ lets us match $A_nh$ with $A_n$. Transitivity therefore gives the uniform estimate $|F_n(x)-F_n(x_0)|\leq\omega_f(\varepsilon_n)$ for every $x\in X$. If $\nu$ is any invariant [Borel probability measure](../../../../../borel-probability-measure.md), then

$$
\int f\,d\nu=\int F_n\,d\nu,\qquad
\left|\int f\,d\nu-F_n(x_0)\right|\leq\omega_f(\varepsilon_n).
$$

Two invariant [probability measures](../../../../../probability-measure.md) consequently differ on the integral of $f$ by at most $2\omega_f(\varepsilon_n)$, hence agree on every [continuous function](../../../../../continuous-function.md). [Continuous functions](../../../../../continuous-function.md) determine [Borel probability measures](../../../../../borel-probability-measure.md) on a [compact metric space](../../../../../compact-metric-space.md), so **the invariant [probability measure](../../../../../probability-measure.md) exists and is unique**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
