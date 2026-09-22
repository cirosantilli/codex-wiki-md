# Invariant subspaces of a quarter-turn in three dimensions

↑ **Parent:** [Invariant subspace](invariant-subspace.md)

For a quarter-turn [rotation](rotation-mathematics.md) $T$ of $\mathbb R^3$ about a unit axis [vector](vector.md) $n$, the only real [invariant subspaces](invariant-subspace.md) are $\{0\}$, the axis $\mathbb Rn$, its perpendicular plane $n^\perp$, and all of $\mathbb R^3$.

Indeed $T^2$ fixes the axis and negates the perpendicular plane. Hence $P=(I+T^2)/2$ is the [linear projection](projection-linear-algebra.md) onto the axis, while $I-P$ is the [linear projection](projection-linear-algebra.md) onto the perpendicular plane. An [invariant subspace](invariant-subspace.md) $L$ is preserved by these [polynomials](polynomial-split.md) in $T$, so

$$
L=(L\cap\mathbb Rn)\oplus(L\cap n^\perp).
$$

The first intersection is either zero or the axis. If the second contains a nonzero $v$, it also contains $Tv$. These are perpendicular nonzero [vectors](vector.md), so they [span](linear-span.md) the perpendicular plane. This proves the classification.

Over the [complex numbers](complex-number.md) the situation changes: the [rotation matrix](rotation-matrix.md) has [eigenvalues](eigenvalue.md) $1,i,-i$, giving three one-dimensional [eigenspaces](eigenspace.md). The absence of real [eigenvalues](eigenvalue.md) on the perpendicular plane explains why it has no real one-dimensional [invariant subspace](invariant-subspace.md).

## ↑ Ancestors (7)

1. [Invariant subspace](invariant-subspace.md)
2. [Group representation](group-representation.md)
3. [Representation theory](representation-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-i/3/b/solution.md)
