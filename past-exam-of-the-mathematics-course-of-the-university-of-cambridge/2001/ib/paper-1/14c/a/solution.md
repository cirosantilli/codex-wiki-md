<h1 id="14c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $J_k(\lambda)$ for the [Jordan block](../../../../../../jordan-block.md) with diagonal $\lambda$ and ones on the superdiagonal. Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) and [minimal polynomial](../../../../../../minimal-polynomial.md) are both $(x-\lambda)^k$. Therefore one answer to the first request is

$$
\boxed{M=J_3(2)\oplus J_2(-1)}.
$$

For the second request, take

$$
\boxed{M_1=J_2(3)\oplus J_2(3)\oplus J_1(3)\oplus J_2(1)},
$$



$$
\boxed{M_2=J_2(3)\oplus J_1(3)\oplus J_1(3)\oplus J_1(3)\oplus J_2(1)}.
$$

The algebraic multiplicities are five and two, and the largest block at each [eigenvalue](../../../../../../eigenvalue.md) has size two, so both prescribed [polynomials](../../../../../../polynomial-split.md) hold. They are not [similar matrices](../../../../../../matrix-similarity.md): the [eigenspace](../../../../../../eigenspace.md) at three has dimensions three and four respectively, and similarity preserves [eigenspace](../../../../../../eigenspace.md) dimension.

**There is no third similarity class.** At [eigenvalue](../../../../../../eigenvalue.md) one, the total size two and maximal block size two force the single block $J_2(1)$. At [eigenvalue](../../../../../../eigenvalue.md) three, the blocks partition five, each has size at most two, and at least one has size two. The only partitions are $2+2+1$ and $2+1+1+1$. The uniqueness of [Jordan normal form](../../../../../../jordan-normal-form.md) up to block order therefore leaves exactly the two classes already exhibited.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14C](../../14c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
