<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume first that the [topological group](../../../../../topological-group-split.md) is Hausdorff. This separation condition is necessary: an indiscrete group with two elements has the one-element [neighbourhood basis](../../../../../neighbourhood-basis.md) consisting of the whole group, but its [topology](../../../../../topology-split.md) cannot come from a [metric](../../../../../metric.md).

Translations are [homeomorphisms](../../../../../homeomorphism.md), since multiplication by a fixed element is continuous and its inverse is multiplication by the inverse element. Inversion is likewise a [homeomorphism](../../../../../homeomorphism.md). If $W$ is an [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md), continuity of the triple product at $(e,e,e)$ supplies [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) $A,B,C$ with $ABC\subset W$. Their intersection with their inverses contains a symmetric open [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) $V$, and $V^3\subset W$. This proves the [neighbourhood](../../../../../neighbourhood-mathematics.md) shrinking property needed below rather than assuming it.

Let $(B_n)$ be a countable [neighbourhood basis](../../../../../neighbourhood-basis.md) at the [identity element](../../../../../identity-element.md), choosing open representatives inside its members. Starting with $U_0=G$, recursively choose symmetric open [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) such that

$$
U_n\subset B_n\cap U_{n-1},\qquad U_n^3\subset U_{n-1}\quad(n\ge1).
$$

They are still a basis. Their intersection is $\{e\}$: for $x\ne e$, the Hausdorff condition gives an [neighbourhood](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) not containing $x$, and some $U_n$ lies inside it.

Here is the [dyadic product estimate for group neighbourhoods](../../../../../dyadic-product-estimate-for-group-neighbourhoods.md). If $g_j\in U_{n_j}$ and $\sum_j2^{-n_j}\le2^{-n}$, then the ordered product lies in $U_{n-1}$, for $n\ge1$. Prove this by induction on the number of factors. A single factor has $n_j\ge n$ and hence belongs to $U_n\subset U_{n-1}$. For a longer word, choose the factor crossing the half-total-cost point. The words preceding and following it each have cost at most half the total, hence at most $2^{-n-1}$. The induction hypothesis puts both in $U_n$, and the middle factor also lies in $U_n$. Their threefold product is in $U_{n-1}$. Empty side words cause no problem because $e\in U_n$.

Give an edge from $x_{j-1}$ to $x_j$ cost $2^{-n_j}$ whenever $x_{j-1}^{-1}x_j\in U_{n_j}$, and define

$$
\boxed{d(x,y)=\inf\left\{\sum_{j=1}^m2^{-n_j}:x_0=x,\ x_m=y,\ x_{j-1}^{-1}x_j\in U_{n_j}\right\}}.
$$

Chains exist because $U_0=G$. Reversing a chain proves symmetry, concatenating chains proves the [triangle inequality](../../../../../triangle-inequality.md), and translating every vertex on the left leaves all edge differences unchanged. Thus $d$ is left invariant. The product estimate also gives

$$
d(x,y)<2^{-n-1}\ \Longrightarrow\ x^{-1}y\in U_n,
\qquad x^{-1}y\in U_n\ \Longrightarrow\ d(x,y)\le2^{-n}.
$$

The first implication follows by choosing a chain with total cost below the bound and applying the estimate with index $n+1$. If $d(x,y)=0$, the first implication puts $x^{-1}y$ in every $U_n$, so $x=y$. Hence $d$ is a genuine [left-invariant group metric](../../../../../left-invariant-group-metric.md). These two inclusions show that its balls and the original [neighbourhoods](../../../../../neighbourhood-mathematics.md) of the [identity element](../../../../../identity-element.md) refine one another; translations then show equality of the two [topologies](../../../../../topology-split.md) everywhere. More explicitly, every [metric](../../../../../metric.md) ball contains a sufficiently small translated $U_n$, and every open [neighbourhood](../../../../../neighbourhood-mathematics.md) contains a sufficiently small [metric](../../../../../metric.md) ball. This proves the sufficient direction of the [Birkhoff-Kakutani theorem](../../../../../birkhoff-kakutani-theorem.md).

Conversely, if a compatible [metric](../../../../../metric.md) exists, the balls $B_d(e,1/n)$ form a countable [neighbourhood basis](../../../../../neighbourhood-basis.md) at the [identity element](../../../../../identity-element.md). Invariance is not even needed for this direction. Thus, with the necessary Hausdorff convention, **a compatible left-invariant [metric](../../../../../metric.md) exists exactly when the [identity element](../../../../../identity-element.md) has a countable [neighbourhood basis](../../../../../neighbourhood-basis.md)**.

For the requested counterexample, take the [orientation-preserving affine group of the real line](../../../../../orientation-preserving-affine-group-of-the-real-line.md), represented by $(a,b)$ with $a>0$ and product $(a,b)(a',b')=(aa',b+ab')$. Its [topology](../../../../../topology-split.md) is metrizable, for instance by the ordinary Euclidean distance in coordinates $(\log a,b)$, and the product and inverse are continuous. Let $D_a=(a,0)$ and $T_b=(1,b)$. Direct multiplication gives $D_aT_bD_a^{-1}=T_{ab}$. A compatible [bi-invariant group metric](../../../../../bi-invariant-group-metric.md) would make every [conjugation](../../../../../conjugation.md) an [isometry](../../../../../isometry.md) fixing $e$. Therefore

$$
d(e,T_{1/n})=d(e,D_nT_{1/n}D_n^{-1})=d(e,T_1)>0.
$$

But $T_{1/n}\to e$ in the group's [topology](../../../../../topology-split.md), a contradiction. This is the [affine conjugation obstruction to a bi-invariant group metric](../../../../../affine-conjugation-obstruction-to-a-bi-invariant-group-metric.md): the group is metrizable, and even admits a compatible left-invariant [metric](../../../../../metric.md), but **admits no compatible [metric](../../../../../metric.md) invariant on both sides**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
