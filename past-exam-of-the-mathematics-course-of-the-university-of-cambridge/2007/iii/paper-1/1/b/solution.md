<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An $\ell$-group here means a [locally profinite group](../../../../../../locally-profinite-group.md), so identity neighbourhoods contain [compact-open subgroups](../../../../../../compact-open-subgroup.md). The right action is a [group representation](../../../../../../group-representation.md) because $\rho(g)\rho(h)f(x)=f(xgh)=\rho(gh)f(x)$.

Let $f$ be a [compactly supported locally constant function](../../../../../../compactly-supported-locally-constant-function.md) with support $S$. For every $x\in S$, local constancy supplies a [compact-open subgroup](../../../../../../compact-open-subgroup.md) $K_x$ with $f$ constant on $xK_x$, and this coset lies in $S$. Compactness gives a finite cover $S=\bigcup_{j=1}^r x_jK_j$. Put $K=\bigcap_jK_j$. Each coset in this cover is right $K$-invariant, so $S$ is right $K$-invariant. Within the support, $xk$ and $x$ lie in the same chosen $x_jK_j$ and have the same function value; outside the support, right $K$-invariance of $S$ ensures that both values remain zero. Hence $\rho(k)f=f$ for all $k\in K$. The zero function is fixed by every subgroup. This proves that the [smooth right regular representation](../../../../../../smooth-right-regular-representation.md) is smooth.

For a fixed [compact-open subgroup](../../../../../../compact-open-subgroup.md) $K$, right-invariant functions are functions on the discrete coset space $G/K$. Compact support becomes finite support there, since the image of a compact set in a discrete space is finite. Conversely every finitely supported function on $G/K$ lifts to a compactly supported locally constant function on $G$. Thus

$$
\boxed{V^K\cong\mathbb C^{(G/K)},}
$$

where the superscript indicates finite support. Its basis is the set of characteristic functions $1_{gK}$, and its dimension is finite exactly when $[G:K]$ is finite.

If $G$ is compact, the discrete quotient $G/K$ is compact and therefore finite for every such $K$; hence the representation is [admissible](../../../../../../admissible-representation-of-a-locally-profinite-group.md). Conversely, admissibility gives finite index for any one [compact-open subgroup](../../../../../../compact-open-subgroup.md). Then $G$ is a finite union of compact cosets, so is compact. Therefore **the representation is admissible if and only if $G$ is compact**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
