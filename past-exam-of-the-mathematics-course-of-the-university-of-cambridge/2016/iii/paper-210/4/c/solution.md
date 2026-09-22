<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For partitions, the appropriate [Hamming distance between unlabelled bipartitions](../../../../../../hamming-distance-between-unlabelled-bipartitions.md) is $\Delta(T,S)=\min\{|T\mathbin\triangle S|,|T\mathbin\triangle S^c|\}$. It counts vertices assigned to the wrong group after the better global exchange of the two group names. The printed signed-indicator formula does not implement this exchange: negating a zero-one indicator is not taking its complement. It must be read as this partition distance, or written with the $\pm1$ membership vectors.

Use the corrected leading [eigenvector](../../../../../../eigenvector.md) estimator from 4(b), and orient its sign to minimize $\|\widehat v-\sigma v\|_2$. At every wrongly signed coordinate, this difference has magnitude at least $1/\sqrt n$. Therefore the [sign rounding bound for a unit eigenvector](../../../../../../sign-rounding-bound-for-a-unit-eigenvector.md) gives

$$
\Delta(\widehat S,S)\leq n\min_\sigma\|\widehat v-\sigma v\|_2^2\leq n\|\widehat v\widehat v^\top-vv^\top\|_F^2\leq2n\|\widehat v\widehat v^\top-vv^\top\|_F.
$$

The last inequality uses the projector distance bound $\sqrt2\leq2$. Taking the [expected value](../../../../../../expected-value.md) of this [Frobenius norm](../../../../../../frobenius-norm.md) estimate proves **$\mathbb E\Delta(\widehat S,S)\leq2nc/t$**. The assertion relies on the corrected estimator and partition-distance definition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
