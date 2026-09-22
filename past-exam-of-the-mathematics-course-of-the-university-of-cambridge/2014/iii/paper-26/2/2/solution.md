<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $T\leq N$ for a deterministic integer $N$. The stopped [martingale](../../../../../../martingale-split.md) has the finite-sum representation

$$
M_T=M_0+\sum_{k=1}^N\mathbf1_{\{T\geq k\}}(M_k-M_{k-1}).
$$

Each summand is integrable, and $\{T\geq k\}=\{T>k-1\}\in\mathcal F_{k-1}$ by the [stopping time](../../../../../../stopping-time.md) property. Therefore the [conditional expectation](../../../../../../conditional-expectation.md) identity for a [martingale](../../../../../../martingale-split.md) gives

$$
\mathbb E\bigl[\mathbf1_{\{T\geq k\}}(M_k-M_{k-1})\bigr]
=\mathbb E\bigl[\mathbf1_{\{T\geq k\}}\mathbb E[M_k-M_{k-1}\mid\mathcal F_{k-1}]\bigr]=0.
$$

Taking expectations in the finite sum proves the bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md):

$$
\boxed{\mathbb E M_T=\mathbb E M_0.}
$$

No limiting argument or uniform-integrability assumption is needed for a [bounded stopping time](../../../../../../bounded-stopping-time.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
