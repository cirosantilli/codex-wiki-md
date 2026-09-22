# Unimodular change of lattice basis

↑ **Parent:** [Unimodular matrix](unimodular-matrix.md)

Let $B_1,B_2$ be real square [invertible matrices](invertible-matrix.md) whose columns are [lattice bases](basis-of-a-toric-lattice.md). They generate the same [Euclidean lattice](euclidean-lattice.md) precisely when

$$
\boxed{B_1\mathbb Z^n=B_2\mathbb Z^n
\quad\Longleftrightarrow\quad
B_2=B_1U\text{ for a unimodular matrix }U.}
$$

[§7, Lemma 13, printed p. 9: equivalent lattice bases](intro-to-lattice-algs-and-crypto-mastermath-spring-2018/lecture-1-introduction.md)

If $B_2=B_1U$, multiplication by $U$ merely permutes the integer coordinate vectors, so the two generated [sets](set-split.md) agree. Conversely, equality of the generated [sets](set-split.md) means every column of either basis is an [integer linear combination](integer-linear-combination.md) of the other. Hence $B_2=B_1U$ and $B_1=B_2V$ for [integer matrices](integer-matrix.md) $U,V$. Substitution followed by multiplication by $B_1^{-1}$ gives $UV=I$, so the [integer inverse criterion for a unimodular matrix](integer-inverse-criterion-for-a-unimodular-matrix.md) applies.

Equal real [linear spans](linear-span.md) are a weaker condition: any two real square [invertible matrices](invertible-matrix.md) span the same ambient [vector space](vector-space-split.md). Even equal [covolumes](covolume.md) do not force the same [Euclidean lattice](euclidean-lattice.md). The requirement that the change matrix and its [inverse matrix](matrix-inverse-split.md) have integer entries provides the missing arithmetic information.

## ↑ Ancestors (6)

1. [Unimodular matrix](unimodular-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Unimodular matrix](unimodular-matrix.md)
