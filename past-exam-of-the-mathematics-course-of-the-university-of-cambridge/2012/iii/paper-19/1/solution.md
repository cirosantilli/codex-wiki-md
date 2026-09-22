<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose a generator $[S^n]$ of $\widetilde H_n(S^n;\mathbb Z)\cong\mathbb Z$. The [mapping degree](../../../../../degree-of-a-continuous-mapping.md) of a [continuous map](../../../../../continuous-map.md) is the integer determined by

$$
\boxed{f_*[S^n]=(\deg f)[S^n].}
$$

For $n\geq1$ this is ordinary top-dimensional [homology](../../../../../homology-split.md); using [reduced homology](../../../../../reduced-homology.md) also gives a convention for $n=0$. Domain and target use the same [orientation](../../../../../orientation-of-a-simplex.md), so reversing the chosen generator in both leaves the integer unchanged. [Homotopy invariance of homology](../../../../../homotopy-invariance-of-homology.md) makes the [mapping degree](../../../../../degree-of-a-continuous-mapping.md) invariant under [homotopy](../../../../../homotopy.md).

We interpret the [manifold criterion for a suspension](../../../../../manifold-criterion-for-a-suspension.md) in the category of nonempty [topological manifolds](../../../../../topological-manifold.md) without boundary, and “[sphere](../../../../../sphere.md)” as homeomorphic to the standard [sphere](../../../../../sphere.md). Let $X$ have dimension $d$. If $X\cong S^d$, an explicit [homeomorphism](../../../../../homeomorphism.md) from its [suspension](../../../../../suspension-topology.md) to $S^{d+1}$ is

$$
[x,t]\longmapsto(\sin(\pi t)x,\cos(\pi t)).
$$

It is a [continuous map](../../../../../continuous-map.md) that is a [bijection](../../../../../bijection.md): the two collapsed ends become the poles, and every other point determines $t$ and $x$ uniquely. The [compact-to-Hausdorff continuous bijection theorem](../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) makes it a [homeomorphism](../../../../../homeomorphism.md).

Conversely suppose $SX$ is a [topological manifold](../../../../../topological-manifold.md). Its open part $X\times(0,1)$ shows its dimension is $d+1$. At a suspension vertex $v$ there is an open cone neighbourhood $U$ on $X$. It is [contractible](../../../../../contractible-space.md), while $U\setminus\{v\}$ admits a [deformation retraction](../../../../../deformation-retraction.md) onto $X$. The [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) and [excision](../../../../../excision-theorem.md) give the [local homology from a link](../../../../../local-homology-from-a-link.md) calculation

$$
H_i(SX,SX\setminus\{v\};\mathbb Z)\cong\widetilde H_{i-1}(X;\mathbb Z).
$$

A point of a $(d+1)$-dimensional [topological manifold](../../../../../topological-manifold.md) without boundary has [local homology](../../../../../local-homology.md) $\mathbb Z$ in degree $d+1$ and zero in all other degrees. Consequently

$$
\widetilde H_j(X;\mathbb Z)\cong
\begin{cases}\mathbb Z,&j=d,\\0,&j\neq d.\end{cases}
$$

Thus $X$ is an [integral homology sphere](../../../../../homology-sphere.md). This conclusion alone does not identify its [homeomorphism](../../../../../homeomorphism.md) type.

If $d\geq2$, it is also [simply connected](../../../../../simply-connected-space.md). Choose a cone neighbourhood $U$ of the vertex and an open coordinate ball $B$ around the vertex inside $U$. By [compactness](../../../../../compact-space.md) of $X$, sufficiently short entire cone neighbourhoods fit inside any neighbourhood of $v$: the inverse image of that neighbourhood contains $X\times\{0\}$, and a finite subcover supplies one uniform collar length. Choose such a shorter cone $V\subset B$. The inclusions of punctured neighbourhoods factor as

$$
V\setminus\{v\}\longrightarrow B\setminus\{v\}\longrightarrow U\setminus\{v\}.
$$

The composite induces an [isomorphism](../../../../../isomorphism.md) of [fundamental groups](../../../../../fundamental-group.md), since both cone punctures are products of $X$ with intervals and their inclusion is a [homotopy equivalence](../../../../../homotopy-equivalence.md). The middle punctured ball has the [homotopy type](../../../../../homotopy-type.md) of $S^d$ and is [simply connected](../../../../../simply-connected-space.md) for $d\geq2$. Hence the composite is also zero on the [fundamental group](../../../../../fundamental-group.md), forcing $\pi_1(X)=0$. This uses the nested neighbourhoods, not an unsupported claim that an arbitrary punctured neighbourhood is a [sphere](../../../../../sphere.md).

The [Hurewicz theorem](../../../../../hurewicz-theorem.md), applied successively to the vanishing lower [homology groups](../../../../../homology-group.md), now gives $\pi_j(X)=0$ for $j<d$ and $\pi_d(X)\cong H_d(X)\cong\mathbb Z$. A representative of its generator is a [continuous map](../../../../../continuous-map.md) $S^d\to X$ inducing an [isomorphism](../../../../../isomorphism.md) in every [integral homology](../../../../../integral-homology.md) degree. [Topological manifolds](../../../../../topological-manifold.md) have the [homotopy type](../../../../../homotopy-type.md) of [CW complexes](../../../../../cw-complex.md), so the [homological Whitehead theorem](../../../../../homological-whitehead-theorem.md) makes it a [homotopy equivalence](../../../../../homotopy-equivalence.md). We have proved that $X$ is a [homotopy sphere](../../../../../homotopy-sphere.md).

At this point the **topological classification theorem is essential**: the [topological generalized Poincare theorem](../../../../../topological-generalized-poincare-theorem.md) says that a closed [homotopy sphere](../../../../../homotopy-sphere.md) is homeomorphic to the standard [sphere](../../../../../sphere.md). Applying it completes the converse for $d\geq2$. For $d=1$, the local calculation makes $X$ a connected [compact](../../../../../compact-space.md) one-dimensional [manifold](../../../../../topological-manifold.md) without boundary, hence a [circle](../../../../../circle.md). For $d=0$, a [compact](../../../../../compact-space.md) zero-dimensional [manifold](../../../../../topological-manifold.md) is a finite set, and $\widetilde H_0(X)\cong\mathbb Z$ forces exactly two points. Thus it is $S^0$. Altogether,

$$
\boxed{SX\text{ is a topological manifold without boundary}\iff X\cong S^d.}
$$

The last classification step is not a consequence of [homology](../../../../../homology-split.md) alone, and we make no assertion of [diffeomorphism](../../../../../diffeomorphism.md) with a prescribed smooth structure. If the word [manifold](../../../../../topological-manifold.md) allows boundary on both sides, the printed assertion needs this correction: the suspension of the interval is a closed disk. For instance $[x,t]\mapsto((2x-1)(1-|2t-1|),2t-1)$ identifies it with the filled diamond $|u|+|v|\leq1$, although the interval is not a [sphere](../../../../../sphere.md).

To construct [sphere maps of arbitrary integer degree](../../../../../sphere-maps-of-arbitrary-integer-degree.md), first use $h_m:S^1\to S^1$, $h_m(z)=z^m$ for any integer $m$, including the constant map when $m=0$. Lifting its argument to the real line gives $\theta\mapsto m\theta$, so the fundamental one-cycle is sent to $m$ times itself. Therefore $\deg h_m=m$.

Two cone neighbourhoods cover a [suspension](../../../../../suspension-topology.md); their intersection admits a [deformation retraction](../../../../../deformation-retraction.md) onto the original space. The reduced [Mayer–Vietoris theorem](../../../../../mayer-vietoris-sequence.md) gives a natural [suspension isomorphism](../../../../../suspension-isomorphism.md)

$$
\widetilde H_{q+1}(SX)\cong\widetilde H_q(X).
$$

Naturality means that the [suspension](../../../../../suspension-topology.md) of a [continuous map](../../../../../continuous-map.md) induces the same integer multiplier. This proves [degree under suspension](../../../../../degree-under-suspension.md). Using the standard identification $S(S^k)\cong S^{k+1}$, set

$$
\boxed{f_{n,m}=S^{\,n-1}h_m:S^n\to S^n,\qquad \deg f_{n,m}=m\quad(n\geq1).}
$$

Thus every integer occurs in every positive [sphere](../../../../../sphere.md) dimension, with negative degrees handled just as well as positive ones.

If “every $n$” includes zero, that final printed assertion is false. The generator of $\widetilde H_0(S^0)$ is the difference of its two points. A map of a two-point set is the identity, the transposition, or one of two constant maps, giving precisely

$$
\boxed{\deg f\in\{-1,0,1\}\quad\text{on }S^0.}
$$

These [degrees of maps of the zero-sphere](../../../../../degrees-of-maps-of-the-zero-sphere.md) are the explicit exception to the arbitrary-degree construction.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
