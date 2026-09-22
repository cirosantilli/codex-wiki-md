<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T$ be the [support of a vector](../../../../../../support-of-a-vector.md) $\hat x$. If the columns indexed by $T$ were linearly dependent, there would be a nonzero $h$ supported in $T$ with $Ah=0$. For sufficiently small real $t$, the nonzero signs of $\hat x_T$ remain fixed, so

$$
\|\hat x+th\|_1=\|\hat x\|_1+t\sum_{j\in T}\operatorname{sgn}(\hat x_j)h_j.
$$

Both positive and negative $t$ preserve the residual and hence feasibility, even with noise. A nonzero slope contradicts minimality in one direction. A zero slope gives distinct minimizers, contradicting uniqueness. Thus those columns are linearly independent, and

$$
\boxed{|\operatorname{supp}\hat x|\le\operatorname{rank}A\le m.}
$$

This proves the [sparse vector](../../../../../../sparse-vector.md) assertion without assuming a noiseless residual.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
