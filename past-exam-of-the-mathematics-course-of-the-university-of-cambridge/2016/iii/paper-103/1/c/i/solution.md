<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The relevant [centralizer of a subalgebra](../../../../../../../centralizer-of-a-subalgebra.md) is

$$
Z_{(n-1,1)}
=\{a\in\mathbb C S_n:ab=ba\text{ for all }b\in\mathbb C S_{n-1}\}.
$$

Equivalently, it is the fixed subspace of $\mathbb C S_n$ under conjugation by $S_{n-1}$. We prove the [Olshanskii centralizer lemma](../../../../../../../olshanskii-centralizer-lemma.md) directly, without assuming [multiplicity-free restriction](../../../../../../../multiplicity-free-restriction.md).

A permutation has one cycle containing $n$, of some length $r\geq1$. Let $\nu$ record the lengths of its other nontrivial cycles, omitting fixed points. Two permutations are conjugate under $S_{n-1}$ exactly when these data $(r,\nu)$ agree: a relabelling of the other letters identifies the distinguished cycles and all remaining cycles. Hence the sums $K_{r,\nu}$ over these conjugation orbits form a basis of $Z_{(n-1,1)}$.

Filter these orbit sums by the number of moved letters other than $n$:

$$
t=(r-1)+|\nu|.
$$

If $r=1$, the permutation fixes $n$, and $K_{1,\nu}$ is already a [conjugacy-class sum](../../../../../../../conjugacy-class-sum.md) in $Z_{n-1}$. For $r\geq2$, let $C_\nu\in Z_{n-1}$ be the class sum with nontrivial cycle lengths $\nu$. Expand

$$
X_n^{\,r-1}C_\nu.
$$

Terms in which the $r-1$ star [transpositions](../../../../../../../transposition-permutation.md) use distinct letters, disjoint from the support of the chosen term of $C_\nu$, produce precisely $K_{r,\nu}$, each with coefficient one. Indeed, a cycle through $n$ has a unique expression as an ordered product of star [transpositions](../../../../../../../transposition-permutation.md) using each of its other letters once; the remaining cycles uniquely determine the term of $C_\nu$.

Every other term moves fewer than $t$ letters outside $n$. A repeated letter uses at most $r-2$ distinct such letters in the star product, and an overlap with the support of $C_\nu$ likewise reduces the size of their union. Since the whole product commutes with $S_{n-1}$, these remaining terms are a [linear combination](../../../../../../../linear-combination.md) of lower-filtered orbit sums. Thus

$$
X_n^{\,r-1}C_\nu=K_{r,\nu}+\sum_{(r',\nu'):\ r'-1+|\nu'|<t}c_{r',\nu'}K_{r',\nu'}.
$$

Induction on $t$, starting with the identity, puts every orbit sum in $\operatorname{alg}(Z_{n-1},X_n)$. The reverse inclusion holds because both proposed generators commute with $\mathbb C S_{n-1}$. Therefore

$$
\boxed{Z_{(n-1,1)}=\operatorname{alg}(Z_{n-1},X_n)}.
$$

In particular this [centralizer of a subalgebra](../../../../../../../centralizer-of-a-subalgebra.md) is commutative: $Z_{n-1}$ is commutative and $X_n$ commutes with it.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
