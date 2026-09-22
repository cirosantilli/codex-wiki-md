<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the forward implication, let $(M_n)$ be a [martingale](../../../../../../../martingale-split.md) and let the [stopping time](../../../../../../../stopping-time.md) $T$ satisfy $0\leq T\leq N$ for a deterministic integer $N$. The stopped variable is integrable because it uses only finitely many integrable values. The pathwise identity

$$
M_T=M_0+\sum_{j=1}^{N}(M_j-M_{j-1})\mathbf1_{\{T\geq j\}}
$$

expresses it through [martingale](../../../../../../../martingale-split.md) increments. Since $\{T\geq j\}=\{T>j-1\}\in\mathcal F_{j-1}$, each summand has [expectation](../../../../../../../expected-value.md) zero by [conditional expectation](../../../../../../../conditional-expectation.md). Consequently

$$
\boxed{\mathbb E M_T=\mathbb E M_0.}
$$

This proves the bounded-time case of the [optional stopping theorem](../../../../../../../optional-sampling-theorem-for-a-supermartingale.md) directly; no assumptions about an unbounded stopping time are being used.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 201](../../../../paper-201-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
