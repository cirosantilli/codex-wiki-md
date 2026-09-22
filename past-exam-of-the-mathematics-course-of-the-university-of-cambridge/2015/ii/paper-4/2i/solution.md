<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

For nonempty [compact sets](../../../../../compact-space.md), define the [distance from a point to a closed set](../../../../../distance-from-a-point-to-a-closed-set.md) by $d(x,B)=\min_{b\in B}|x-b|$ and the [Hausdorff distance](../../../../../hausdorff-distance.md) by

$$
d_H(A,B)=\max\{\sup_{a\in A}d(a,B),\sup_{b\in B}d(b,A)\}.
$$

The minima and suprema exist: the sets are nonempty and [compact](../../../../../compact-space.md), and the distance function is [Lipschitz continuous](../../../../../lipschitz-continuity.md). The [Hausdorff distance](../../../../../hausdorff-distance.md) is finite, nonnegative and symmetric. If it is zero, every point of $A$ belongs to the [closed set](../../../../../closed-set.md) $B$ and conversely, so $A=B$; the converse is immediate.

For $a\in A$, choose $b\in B$ attaining $d(a,B)$ and then $c\in C$ attaining $d(b,C)$. The [triangle inequality](../../../../../triangle-inequality.md) gives $d(a,C)\leq d(a,B)+d_H(B,C)$. Taking the supremum over $a$, and doing the same with $A,C$ exchanged, proves $d_H(A,C)\leq d_H(A,B)+d_H(B,C)$. Hence this is a [metric](../../../../../metric.md).

The nested [compact sets](../../../../../compact-space.md) have the [finite intersection property](../../../../../finite-intersection-property.md) inside $K_1$, so $K=\bigcap K_n$ is nonempty. It is a [closed subset](../../../../../closed-set.md) of $K_1$ and therefore [compact](../../../../../compact-space.md). Because $K\subseteq K_n$, only $\sup_{x\in K_n}d(x,K)$ contributes to the [Hausdorff distance](../../../../../hausdorff-distance.md). If this did not tend to zero, some increasing indices $n_j$ and $x_j\in K_{n_j}$ would satisfy $d(x_j,K)\geq\epsilon>0$. A [convergent subsequence](../../../../../convergent-subsequence.md) in $K_1$ has limit $x$. For each fixed $m$, its tail belongs to the [closed set](../../../../../closed-set.md) $K_m$, so $x\in K$. But then $d(x_j,K)\leq|x_j-x|\to0$, a contradiction. Thus $\boxed{d_H(K_n,K)\to0}$.

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
