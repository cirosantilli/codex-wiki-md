<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Both $X_n$ and $A_n$ are increasing, so each has a [limit of a sequence](../../../../../limit-of-a-sequence.md) in $[0,\infty]$. Apply part (c)(ii) to the [martingale](../../../../../martingale-split.md) $M_n=X_n-A_n$, whose [bounded increments](../../../../../bounded-increments.md) were verified in part (i).

On $\{X_\infty<\infty,\ A_\infty=\infty\}$ we would have $M_n\to-\infty$. On $\{X_\infty=\infty,\ A_\infty<\infty\}$ we would have $M_n\to+\infty$. Both [events](../../../../../event.md) have [probability](../../../../../probability.md) zero by the convergence-or-oscillation conclusion. Hence the two divergence [events](../../../../../event.md) agree up to a [null set](../../../../../null-set.md). Since $X_\infty=\infty$ means precisely that infinitely many $B_n$ occur,

$$
\boxed{\{B_n\text{ infinitely often}\}=\left\{\sum_{k=1}^\infty\mathbb E[\mathbf1_{B_k}\mid\mathcal F_{k-1}]=\infty\right\}\quad\text{almost surely}.}
$$

Taking [probabilities](../../../../../probability.md) proves the displayed equality in the question. This stronger agreement of [events](../../../../../event.md) is the [Conditional Borel-Cantelli lemma](../../../../../conditional-borel-cantelli-lemma.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
