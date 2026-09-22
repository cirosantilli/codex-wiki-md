<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

For $x\geq0$, the function $h(x)=e^x-1-x$ has $h(0)=0$ and $h'(x)=e^x-1\geq0$, because the [exponential function](../../../../../exponential-function.md) is increasing and $e^0=1$. Therefore $\boxed{e^x\geq1+x}$.

Write $S_n=\sum_{j=1}^n a_j$ and $P_n=\prod_{j=1}^n(1+a_j)$. Expanding the product produces $1+S_n$ and additional nonnegative terms, giving $P_n\geq1+S_n\geq S_n$. Applying the exponential inequality to every factor gives

$$
\boxed{S_n\leq P_n\leq\prod_{j=1}^n e^{a_j}=e^{S_n}.}
$$

Both sequences are increasing, since the terms $a_j$ are positive. If $S_n$ converges to a finite value $S$, then $P_n\leq e^S$, so the convergence theorem for [monotone bounded sequences](../../../../../monotone-bounded-sequence.md) makes $P_n$ converge. Conversely, if $P_n$ has a finite limit, then $S_n\leq P_n$ is bounded and increasing, hence converges by the same theorem. Thus **the positive series and the product both converge to finite limits, or both diverge to $+\infty$**. This proves the [positive sum-product convergence criterion](../../../../../positive-sum-product-convergence-criterion.md). The word limit here means a finite real limit; allowing extended infinite limits would make the conclusion vacuous for these [monotone sequences](../../../../../monotone-sequence.md).

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
