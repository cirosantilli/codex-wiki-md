# Tripotent linear operator

↑ **Parent:** [Linear operator](linear-operator.md)

For a [linear operator](linear-operator.md) on a real [vector space](vector-space-split.md), the identity $T^3=T$ gives an explicit [eigenspace](eigenspace.md) decomposition

$$
V=\ker T\oplus\ker(T-I)\oplus\ker(T+I).
$$

Indeed, the [linear operators](linear-operator.md)

$$
P_0=I-T^2,\qquad P_+=\frac{T^2+T}{2},\qquad P_-=\frac{T^2-T}{2}
$$

sum to $I$. Their images lie respectively in the [eigenspaces](eigenspace.md) for $0$, $1$, and $-1$, since $TP_0=0$, $TP_+=P_+$, and $TP_-=-P_-$. On each of these [eigenspaces](eigenspace.md), its corresponding $P$ is the identity and the other two vanish, which proves uniqueness of the decomposition. Thus a finite-dimensional tripotent [linear operator](linear-operator.md) admits a [diagonalization](diagonalization-of-a-matrix.md) with diagonal entries in $\{0,1,-1\}$. The condition $T^2\ne T$ is equivalent to the presence of a nonzero $-1$ [eigenspace](eigenspace.md), and $T^2\ne I$ is equivalent to a nonzero [kernel](kernel-of-a-linear-map-split.md).

## ↑ Ancestors (8)

1. [Linear operator](linear-operator.md)
2. [Linear map](linear-map.md)
3. [Vector space](vector-space-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-i/4/b/ii/solution.md)
