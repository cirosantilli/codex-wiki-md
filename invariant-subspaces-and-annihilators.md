# Invariant subspaces and annihilators

↑ **Parent:** [Annihilator of a vector subspace](annihilator-of-a-vector-subspace.md)

For a [linear map](linear-map.md) $T:V\to V$, an [invariant subspace](invariant-subspace.md) $U$ has an [annihilator of a vector subspace](annihilator-of-a-vector-subspace.md) $U^0$ invariant under the [dual map](transpose-of-a-linear-map.md) $T'$. Indeed, for $\varphi\in U^0$ and $u\in U$,

$$
(T'\varphi)(u)=\varphi(Tu)=0.
$$

For a [finite-dimensional vector space](finite-dimensional-vector-space.md), the converse also holds. If $T'(U^0)\subseteq U^0$, every $\varphi\in U^0$ vanishes on $Tu$ for each $u\in U$. The [dual basis](dual-basis.md) description of $U^0$ shows that the common zero set of its [linear functionals](linear-functional.md) is exactly $U$, so $Tu\in U$. Thus

$$
\boxed{U\text{ is invariant under }T\iff U^0\text{ is invariant under }T'}.
$$

The [dimension](dimension-vector-space.md) identity $\dim U^0=\dim V-\dim U$ exchanges a one-dimensional [invariant subspace](invariant-subspace.md) with an invariant [hyperplane](hyperplane.md) in the [dual space](dual-space-split.md).

## ↑ Ancestors (7)

1. [Annihilator of a vector subspace](annihilator-of-a-vector-subspace.md)
2. [Dual space](dual-space-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/1/b/iii/solution.md)
- [Triangularization using dual spaces](triangularization-using-dual-spaces.md)
