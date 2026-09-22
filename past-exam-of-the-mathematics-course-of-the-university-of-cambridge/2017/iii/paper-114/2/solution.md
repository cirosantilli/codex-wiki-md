<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the [sphere](../../../../../sphere.md) [homology](../../../../../homology-split.md) calculation use [singular homology](../../../../../singular-homology.md), [homotopy invariance of homology](../../../../../homotopy-invariance-of-homology.md), and the reduced [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md), not [cellular homology](../../../../../cellular-chain-complex.md). For a point, its [chain group](../../../../../chain-group.md) for [singular homology](../../../../../singular-homology.md) is $\mathbb Z$ in every nonnegative degree, and its [boundary operator](../../../../../boundary-operator.md) is multiplication by $\sum_{i=0}^q(-1)^i$, hence alternately zero and one in positive degrees. Its [homology](../../../../../homology-split.md) is therefore $\mathbb Z$ in degree zero and zero above. [Singular chains](../../../../../singular-chain.md) of a disjoint union split into the summand [chain complexes](../../../../../chain-complex.md). Start with $S^0$, the disjoint union of two points: $H_0(S^0;\mathbb Z)=\mathbb Z^2$, all positive groups vanish, and $\widetilde H_0(S^0;\mathbb Z)=\mathbb Z$. For $n\geq1$, remove the north and south poles to obtain an [open cover](../../../../../open-cover.md) $U,V$ of $S^n$. Each member is [contractible](../../../../../contractible-space.md), while $U\cap V$ has a [deformation retraction](../../../../../deformation-retraction.md) to $S^{n-1}$, including the disconnected intersection when $n=1$. The reduced [exact sequence](../../../../../exact-sequence.md) therefore supplies

$$
\widetilde H_q(S^n;\mathbb Z)\cong\widetilde H_{q-1}(S^{n-1};\mathbb Z)\qquad(q\geq1).
$$

Also $S^n$ is connected, so its reduced degree-zero group vanishes. Induction gives

$$
\boxed{H_q(S^n;\mathbb Z)\cong\begin{cases}\mathbb Z,&q=0,n,\\0,&q\notin\{0,n\},\end{cases}\qquad n\geq1.}
$$

The separate $S^0$ calculation avoids conflating its two degree-zero generators.

Choose an [orientation](../../../../../orientation-of-a-simplex.md) of $S^n$, with $n\geq1$, and let $[S^n]$ be its [fundamental class](../../../../../fundamental-class.md). The [mapping degree](../../../../../degree-of-a-continuous-mapping.md) is the [integer](../../../../../integer.md) determined by $f_*[S^n]=\deg(f)[S^n]$. To define the [local degree](../../../../../local-degree-of-a-continuous-map.md) at $x_0$, set $y_0=f(x_0)$ and require $x_0$ to be isolated in $f^{-1}(y_0)$. Choose an open neighborhood $B$ containing no other point of that fiber. Then $f$ defines a map of pairs

$$
(B,B\setminus\{x_0\})\longrightarrow(S^n,S^n\setminus\{y_0\}).
$$

The degree-$n$ [relative homology](../../../../../relative-homology.md) groups on both sides are $\mathbb Z$, by a [manifold chart](../../../../../manifold-chart.md) and [excision](../../../../../excision-theorem.md). The [local orientation of a manifold](../../../../../local-orientation-of-a-manifold.md) chooses their generators. The induced map multiplies these generators by an [integer](../../../../../integer.md), denoted $\deg_{x_0}f$. [Excision](../../../../../excision-theorem.md) and naturality show independence of the choice of $B$. Differentiability is unnecessary; if $f$ is smooth and $Df_{x_0}$ is invertible, the [inverse function theorem](../../../../../inverse-function-theorem.md) gives $\deg_{x_0}f=\operatorname{sign}\det Df_{x_0}$ relative to the [orientations](../../../../../orientation-of-a-simplex.md). Without isolation in the fiber this pointwise definition need not apply.

For the [degree as a sum of local degrees](../../../../../degree-as-a-sum-of-local-degrees.md), assume $y\in S^n$ has finite fiber $F=\{x_1,\ldots,x_s\}$. Disjoint coordinate neighborhoods and [excision](../../../../../excision-theorem.md) identify

$$
H_n(S^n,S^n\setminus F;\mathbb Z)\cong\bigoplus_{j=1}^s H_n(S^n,S^n\setminus\{x_j\};\mathbb Z).
$$

The absolute [fundamental class](../../../../../fundamental-class.md) maps to the tuple of local [orientation](../../../../../orientation-of-a-simplex.md) generators. Under the relative map induced by $f$, the $j$th generator goes to $\deg_{x_j}f$ times the generator at $y$, and the resulting map from the [direct sum](../../../../../direct-sum.md) adds these contributions. On the other hand, naturality says that first applying the absolute map $f_*$ and then passing to the local group at $y$ gives $\deg(f)$ times that generator. Thus

$$
\boxed{\deg(f)=\sum_{x\in f^{-1}(y)}\deg_x f.}
$$

If the fiber is empty the sum is zero: the map factors through the [contractible](../../../../../contractible-space.md) punctured [sphere](../../../../../sphere.md) and has degree zero. If every point of a fiber is isolated, compactness makes that closed fiber finite, so the theorem applies. In particular, a [regular value](../../../../../regular-value.md) of a smooth map gives the signed count of its inverse images. For $n=0$, define a [mapping degree](../../../../../degree-of-a-continuous-mapping.md) on the reduced generator $[p_+]-[p_-]$: the identity has [mapping degree](../../../../../degree-of-a-continuous-mapping.md) one, the swap of the two points minus one, and either constant map zero. With local [orientation](../../../../../orientation-of-a-simplex.md) signs positive at $p_+$ and negative at $p_-$, the same sum formula holds. The connected-[sphere](../../../../../sphere.md) convention above is the standard positive-dimensional one.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
