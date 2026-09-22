<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $z\in K$. If $z\in\partial K$, the conclusion is immediate. Otherwise $z$ is in the [interior](../../../../../../interior-topology.md) of $K$. If $f(z)=0$, nonnegativity of the [boundary](../../../../../../boundary-of-a-set.md) [supremum](../../../../../../supremum.md) suffices. For $f(z)\ne0$, the complex [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) gives a [bounded linear functional](../../../../../../continuous-linear-functional.md) $\ell:A\to\mathbb C$ with $\|\ell\|=1$ and $\ell(f(z))=\|f(z)\|$. The scalar function $g=\ell\circ f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md).

Let $V$ be the [connected component](../../../../../../connected-component.md) of the [interior](../../../../../../interior-topology.md) of $K$ containing $z$. It is bounded, its closure is contained in $K$, and $\partial V\subseteq\partial K$. To see the last inclusion, a [boundary](../../../../../../boundary-of-a-set.md) point of $V$ lying in the [interior](../../../../../../interior-topology.md) of $K$ would have a small [connected](../../../../../../connected-space.md) open ball in that [interior](../../../../../../interior-topology.md) meeting $V$; the ball would belong to the same component, contradicting that it is a [boundary](../../../../../../boundary-of-a-set.md) point. The scalar [maximum modulus principle on a bounded domain](../../../../../../maximum-modulus-principle-on-a-bounded-domain.md) therefore gives

$$
\|f(z)\|=|g(z)|\le\sup_{w\in\partial V}|g(w)|\le\sup_{w\in\partial K}\|f(w)\|.
$$

For [completeness](../../../../../../completeness.md), this [boundary](../../../../../../boundary-of-a-set.md) form of the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) follows by taking the maximum on the [compact](../../../../../../compact-space.md) closure of $V$. An [interior](../../../../../../interior-topology.md) maximum makes $g$ constant on $V$, in which case [continuity](../../../../../../continuous-function.md) gives the same value on its nonempty [boundary](../../../../../../boundary-of-a-set.md). Thus the [norm maximum principle for a Banach-space-valued holomorphic function](../../../../../../norm-maximum-principle-for-a-banach-space-valued-holomorphic-function.md) applies to arbitrary [compact](../../../../../../compact-space.md) $K$, even when it is disconnected or has nonsmooth [boundary](../../../../../../boundary-of-a-set.md):

$$
\boxed{\|f(z)\|\le\sup_{w\in\partial K}\|f(w)\|.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
