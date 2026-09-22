# Finite-dimensional subspace is an intersection of kernels

↑ **Parent:** [Annihilator of a vector subspace](annihilator-of-a-vector-subspace.md)

For a [vector subspace](vector-subspace.md) $U$ of a finite-dimensional [vector space](vector-space-split.md) $V$, its [annihilator of a vector subspace](annihilator-of-a-vector-subspace.md) $U^0\subseteq V^*$ determines $U$ exactly: $U=\bigcap_{f\in U^0}\ker f$. Indeed, a [basis](basis.md) of $U$ can be extended to one of $V$. If $v\notin U$, include $v$ among the added basis vectors and define a [linear functional](linear-functional.md) taking value one at $v$ and zero on all the other basis vectors. This functional vanishes on $U$ but not at $v$, excluding every outside vector from the intersection.

It suffices to intersect the [kernels](kernel-of-a-linear-map-split.md) of any [basis](basis.md) $g_1,\ldots,g_k$ of $U^0$: every other annihilating functional is their [linear combination](linear-combination.md). The [dual basis](dual-basis.md) for a basis of $V$ extending a basis of $U$ shows $k=\dim V-\dim U$. If $U=V$, the empty intersection is $V$. This translates a subspace description by spanning vectors into an exact description by independent linear equations.

## ↑ Ancestors (7)

1. [Annihilator of a vector subspace](annihilator-of-a-vector-subspace.md)
2. [Dual space](dual-space-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
