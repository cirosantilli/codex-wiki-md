<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the preceding construction with type-$i$ claims of deterministic size $a_i$. For $\Lambda=\sum_i\lambda_i>0$, the answer is

$$
\boxed{N\sim\operatorname{Pois}(\Lambda),\qquad
\mathbb P(X=a_i)=\frac{\lambda_i}{\Lambda},\qquad
F_X(x)=\sum_{i:a_i\le x}\frac{\lambda_i}{\Lambda}.}
$$

The [characteristic function](../../../../../../characteristic-function.md) verifies this directly:

$$
\mathbb Ee^{itT}=\prod_i\exp\{\lambda_i(e^{ita_i}-1)\}
=\exp\{\Lambda(\mathbb Ee^{itX}-1)\}.
$$

Hence $T$ has the stated [compound Poisson distribution](../../../../../../compound-poisson-distribution.md). Distinctness of the $a_i$ makes the atomic [probabilities](../../../../../../probability.md) unambiguous.

A zero coefficient is allowed. It corresponds to zero-sized claims in this representation and contributes nothing to $T$. If a representation using only positive claims is preferred, remove that category: its count parameter becomes $\Lambda_+=\sum_{i:a_i>0}\lambda_i$, with [probabilities](../../../../../../probability.md) $\lambda_i/\Lambda_+$ on the positive values. The [zero claim sizes in a compound Poisson representation](../../../../../../zero-claim-sizes-in-a-compound-poisson-representation.md) explain why the count parameter need not be unique. If $\Lambda=0$, or if all positive-size categories have zero rate, the aggregate is identically zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
