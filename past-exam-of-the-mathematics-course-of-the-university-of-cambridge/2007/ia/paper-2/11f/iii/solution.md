<h1 id="11f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The statement is true.** For $n\geq2$, being in every pairwise intersection is equivalent to being in all the events:

$$
\bigcap_{i<j}(A_i\cap A_j)=\bigcap_{k=1}^n A_k.
$$

Indeed every index occurs in at least one pair. Apply the [union bound](../../../../../../boole-s-inequality.md) to the complements of these $\binom n2$ pairwise intersections to obtain

$$
P\left(\bigcap_{k=1}^n A_k\right)
\geq1-\sum_{i<j}\{1-P(A_i\cap A_j)\}
=\sum_{i<j}P(A_i\cap A_j)-\binom n2+1>0.
$$

This is [positive common intersection from pair-intersection probabilities](../../../../../../positive-common-intersection-from-pair-intersection-probabilities.md). It remains valid for $n=2$, where it reduces to the asserted positivity of the single pairwise intersection.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
