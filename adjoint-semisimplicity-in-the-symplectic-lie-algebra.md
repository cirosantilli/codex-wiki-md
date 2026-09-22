# Adjoint semisimplicity in the symplectic Lie algebra

↑ **Parent:** [Symplectic Lie algebra](symplectic-lie-algebra.md)

Let $V$ be a finite-dimensional [symplectic vector space](symplectic-vector-space.md) over an [algebraically closed field](algebraically-closed-field.md) of [characteristic zero](characteristic-zero.md). For $a\in\mathfrak{sp}(V)$, write its [Jordan–Chevalley decomposition](jordan-chevalley-decomposition.md) as $a=S+N$. Applying the [symplectic adjoint](symplectic-adjoint.md) to this decomposition and using $a^*=-a$, uniqueness gives $S^*=-S$ and $N^*=-N$. Thus both parts belong to the [symplectic Lie algebra](symplectic-lie-algebra.md). The operators $\operatorname{ad}S$ and $\operatorname{ad}N$ commute. The former is [diagonalizable](diagonalizable-matrix.md) on $\operatorname{End}(V)$ in a [matrix unit](matrix-unit.md) [basis](basis.md) for an [eigenbasis](eigenbasis.md) of $S$, and the latter is a [nilpotent linear map](nilpotent-linear-map.md), as follows from

$$
(\operatorname{ad}N)^m(T)=\sum_{j=0}^m(-1)^j\binom mjN^{m-j}TN^j.
$$

The restrictions to the invariant [symplectic Lie algebra](symplectic-lie-algebra.md) retain these properties. Hence these restrictions form the [Jordan–Chevalley decomposition](jordan-chevalley-decomposition.md) of $\operatorname{ad}a$.

If $\operatorname{ad}a$ is [diagonalizable](diagonalizable-matrix.md), $\operatorname{ad}N=0$. For every $v\in V$, the rank-one map $T_v(w)=\omega(v,w)v$ lies in $\mathfrak{sp}(V)$, since the two terms in $\omega(T_vw,u)+\omega(w,T_vu)$ cancel by alternation. For $v\ne0$ its image is $kv$, so commuting with $T_v$ forces $N$ to preserve $kv$. A [linear map](linear-map.md) preserving every line is scalar: compare its action on two [linearly independent](linear-independence.md) vectors and on their sum. Since $N$ is a [nilpotent linear map](nilpotent-linear-map.md), that scalar is zero. Thus $a=S$ is [diagonalizable](diagonalizable-matrix.md). Conversely, if $a$ is [diagonalizable](diagonalizable-matrix.md) on $V$, its [operator commutator](operator-commutator.md) action is [diagonalizable](diagonalizable-matrix.md) on $\operatorname{End}(V)$ and therefore on its invariant [symplectic Lie algebra](symplectic-lie-algebra.md). This proves both directions, including $V=0$.

## ↑ Ancestors (10)

1. [Symplectic Lie algebra](symplectic-lie-algebra.md)
2. [Simple Lie algebra](simple-lie-algebra.md)
3. [Semisimple Lie algebra](semisimple-lie-algebra-split.md)
4. [Lie algebra](lie-algebra-split.md)
5. [Lie theory](lie-theory-split.md)
6. [Diagonal dominance](diagonal-dominance.md)
7. [Algebra](algebra-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford/2023/3/b/solution.md)
- [Toral subalgebra](toral-subalgebra.md)
