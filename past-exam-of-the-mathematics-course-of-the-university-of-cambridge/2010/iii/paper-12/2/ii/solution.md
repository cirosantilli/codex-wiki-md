<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $d=d_H(A,B)=\min\{d_H(\alpha,\beta):\alpha\in A,\ \beta\in B\}$, and define $f(\sigma)=d_H(\sigma,A)$. The triangle inequality shows that $f$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) with [Lipschitz constant](../../../../../../lipschitz-constant.md) one. It vanishes on $A$, and $f\geq d$ on $B$. Let $\mu=\mathbb Ef$ for a uniform [permutation](../../../../../../permutation.md).

If $\mu\geq d/2$, apply the lower-tail bound proved in part (i):

$$
\frac{|A|}{n!}=\mathbb P(\sigma\in A)
\leq\mathbb P(f-\mu\leq-\mu)
\leq e^{-\mu^2/(2n)}\leq e^{-d^2/(8n)}.
$$

If $\mu<d/2$, apply its upper-tail bound:

$$
\frac{|B|}{n!}\leq\mathbb P(f-\mu\geq d-\mu)
\leq e^{-(d-\mu)^2/(2n)}\leq e^{-d^2/(8n)}.
$$

For $d=0$ the desired inequality is simply $\min\{|A|,|B|\}\leq n!$. Hence in all cases

$$
\boxed{\min\{|A|,|B|\}\leq n!\exp\!\left(-\frac{d_H(A,B)^2}{8n}\right).}
$$

This uses only the precise one-sided [concentration inequality](../../../../../../concentration-inequality.md) from part (i) and the [Hamming distance](../../../../../../hamming-distance.md) triangle inequality. The normalization of the distance matters: it counts mismatching coordinates, rather than dividing their number by $n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
