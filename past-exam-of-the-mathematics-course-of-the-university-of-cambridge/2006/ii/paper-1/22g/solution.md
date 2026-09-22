<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

Two [norms](../../../../../norm.md) are [Lipschitz equivalent norms](../../../../../equivalent-norms.md) if constants $c,C>0$ satisfy $c\|u\|_1\leq\|u\|_2\leq C\|u\|_1$ for every $u$. On the [vector space](../../../../../vector-space-split.md) of finitely supported sequences, the [norms](../../../../../norm.md) $\|x\|_1=\sum|x_i|$ and $\|x\|_\infty=\max|x_i|$ are not equivalent: a vector with $N$ entries equal to one has the two [norms](../../../../../norm.md) $N$ and one.

For dimension $d<\infty$, choose a [basis](../../../../../basis.md) and write $u=\sum x_ie_i$. Any [norm](../../../../../norm.md) satisfies $\|u\|\leq\sum|x_i|\|e_i\|\leq C|x|_2$. This also implies its [continuity](../../../../../continuous-function.md) in the Euclidean coordinates, by $|\|u\|-\|v\||\leq\|u-v\|\leq C|x-y|_2$. Its positive continuous values on the [compact](../../../../../compact-space.md) Euclidean [unit sphere](../../../../../unit-sphere.md) have a positive minimum $c$. Homogeneity gives $c|x|_2\leq\|u\|$, proving equivalence with the Euclidean [norm](../../../../../norm.md) and hence between any two [norms](../../../../../norm.md).

If a finite-dimensional subspace $U$ of a normed space contains a sequence converging in the ambient [norm](../../../../../norm.md), its coefficient vectors are Cauchy by this equivalence. The coefficients converge in $\mathbb R^d$ or $\mathbb C^d$, and the reconstructed vector lies in $U$ and is the ambient limit. Thus **finite-dimensional subspaces are closed**.

A finite-dimensional normed space has nonempty open balls with [compact](../../../../../compact-space.md) closures by equivalence and Heine-Borel. Conversely let an [open set](../../../../../open-set.md) $O$ have [compact closure](../../../../../relatively-compact-subset.md). Choose $w\in O$ and $r>0$ such that $B(w,r)\subset O$. Its closed ball of radius $r/2$ is a [closed subset](../../../../../closed-set.md) of the [compact closure](../../../../../relatively-compact-subset.md) of $O$ and is therefore [compact](../../../../../compact-space.md). Translation and scaling make the closed [unit ball](../../../../../unit-ball.md) [compact](../../../../../compact-space.md).

If the space were infinite-dimensional, construct unit vectors $x_j$ with $\operatorname{dist}(x_j,\operatorname{span}(x_1,\ldots,x_{j-1}))>1/2$. Here is the needed [Riesz lemma](../../../../../riesz-s-lemma.md): for a proper closed subspace $M$, choose $z\notin M$, put $d=\operatorname{dist}(z,M)>0$, and choose $m\in M$ with $\|z-m\|<2d$; then $(z-m)/\|z-m\|$ has distance greater than $1/2$ from $M$. The finite spans are closed by the earlier argument, so this constructs the sequence. Its members are separated by more than $1/2$, and have no convergent subsequence, contradicting [compactness](../../../../../compact-space.md). Therefore **the space is finite-dimensional exactly when it has a nonempty [open set](../../../../../open-set.md) with [compact closure](../../../../../relatively-compact-subset.md)**.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
