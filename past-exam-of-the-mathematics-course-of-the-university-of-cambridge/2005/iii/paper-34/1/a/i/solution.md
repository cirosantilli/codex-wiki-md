<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [martingale](../../../../../../../martingale-split.md) and a [stopping time](../../../../../../../stopping-time.md) $T\leq N$, expand the stopped value using its [martingale differences](../../../../../../../martingale-difference.md):

$$
M_T-M_0=\sum_{k=1}^N\mathbf1_{\{T\geq k\}}(M_k-M_{k-1}).
$$

The event $\{T\geq k\}=\{T>k-1\}$ belongs to the [filtration](../../../../../../../filtration-probability-theory.md) $\mathcal F_{k-1}$. Each summand is integrable and its [conditional expectation](../../../../../../../conditional-expectation.md) given $\mathcal F_{k-1}$ is zero. Taking [expectations](../../../../../../../expected-value.md) of this finite sum therefore proves **$\mathbb E M_T=\mathbb E M_0$ for every bounded stopping time**. This proves the forward direction of the [bounded-stopping-time characterization of a martingale](../../../../../../../bounded-stopping-time-characterization-of-a-martingale.md) without assuming an [optional stopping theorem](../../../../../../../optional-sampling-theorem-for-a-supermartingale.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 34](../../../../paper-34-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
