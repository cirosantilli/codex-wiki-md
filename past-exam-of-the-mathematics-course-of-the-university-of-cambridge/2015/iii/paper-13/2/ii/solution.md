<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An elementary [union-intersection compression](../../../../../../union-intersection-compression.md) replaces two occurrences $A_1,A_2$ in a [multiset](../../../../../../multiset.md) by $A_1\cup A_2,A_1\cap A_2$. By [entropy submodularity](../../../../../../entropy-submodularity.md), this changes the sum of [information entropies](../../../../../../information-entropy.md) by

$$
H(X_{A_1\cup A_2})+H(X_{A_1\cap A_2})-H(X_{A_1})-H(X_{A_2})\leq0.
$$

A [compression of an entropy sum](../../../../../../compression-of-an-entropy-sum.md) is obtained by iterating these elementary [union-intersection compressions](../../../../../../union-intersection-compression.md). Summing the inequalities over the sequence, with repetitions counted according to their [multiset](../../../../../../multiset.md) multiplicities, proves **the required monotonicity**:

$$
\boxed{\sum_{A\in\mathcal A}H(X_A)\geq\sum_{B\in\mathcal B}H(X_B).}
$$

Neither the number of occurrences of an individual coordinate nor the total number of sets changes under [union-intersection compression](../../../../../../union-intersection-compression.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
