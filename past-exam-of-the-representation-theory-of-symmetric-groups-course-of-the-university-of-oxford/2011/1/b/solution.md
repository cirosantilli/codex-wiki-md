<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the question's indexing convention: $m_{\lambda,\mu}$ is the [multiplicity](../../../../multiplicity-mathematics.md) of the [irreducible](../../../../irreducible-representation.md) [Specht module](../../../../specht-module.md) $S^\mu_{\mathbb C}$ in the [permutation module](../../../../permutation-module.md) $M^\lambda_{\mathbb C}$. In notation for semistandard-tableau [Kostka numbers](../../../../kostka-number.md) this is often written $K_{\mu\lambda}$, with the indices reversed.

Let $S_\lambda=S_{\lambda_1}\times S_{\lambda_2}\times\cdots$ be the [Young subgroup](../../../../young-subgroup.md). The [permutation character](../../../../permutation-character.md) is

$$
\xi^\lambda=\operatorname{Ind}_{S_\lambda}^{S_n}\mathbf1,
$$

and $\xi^\lambda(g)$ counts the $\lambda$-tabloids fixed by $g$. Equivalently it counts [ordered partitions](../../../../set-partition.md) into labelled rows of the prescribed sizes, each row [invariant](../../../../invariant-mathematics.md) under $g$. [Character](../../../../character-of-a-representation.md) inner products and [Frobenius reciprocity](../../../../frobenius-reciprocity.md) give the purely character-theoretic computation

$$
\boxed{m_{\lambda,\mu}=\langle\xi^\lambda,\chi_\mu\rangle_{S_n}
=\frac1{|S_\lambda|}\sum_{h\in S_\lambda}\chi_\mu(h).}
$$

The [characters](../../../../character-of-a-representation.md) of [symmetric groups](../../../../symmetric-group.md) are real-valued, so no conjugation is needed in the displayed [subgroup](../../../../subgroup.md) average.

For $\lambda=(2,1^3)$, the [Young subgroup](../../../../young-subgroup.md) has two elements, the identity and one [transposition](../../../../transposition-permutation.md). Thus $m_{(2,1^3),\mu}=(\chi_\mu(1)+\chi_\mu((12)))/2$, and part (a) gives

$$
\boxed{\begin{array}{c|rrrrrrr}
\mu&(5)&(4,1)&(3,2)&(3,1,1)&(2,2,1)&(2,1^3)&(1^5)\\\hline
m_{(2,1^3),\mu}&1&3&3&3&2&1&0
\end{array}}
$$

The resulting [dimension](../../../../dimension-vector-space.md) is $1+3\cdot4+3\cdot5+3\cdot6+2\cdot5+4=60=5!/2$, the [dimension](../../../../dimension-vector-space.md) of the [permutation module](../../../../permutation-module.md).

This is the [character average for Kostka numbers](../../../../character-average-for-kostka-numbers.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the representation Theory of Symmetric Groups course of the University of Oxford](../../../split.md)
5. [Representation Theory of Symmetric Groups course of the University of Oxford](../../../../representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
