<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an integer $m$ and $d\in\{-1,0,1\}$, verify the single-step identity

$$
(m+d)^+-m^+=f(m)d+\frac12\mathbf1_{\{m=0\}}d^2.
$$

If $m\geq1$, the [positive part](../../../../../../positive-part-of-a-real-valued-function.md) is linear across the step and $f(m)=1$; if $m\leq-1$, it remains zero and $f(m)=0$. At $m=0$, $d^+=(d+d^2)/2$, which is checked for the three permitted values of $d$.

Apply this with $m=S_{t-1}-K$ and $d=S_t-S_{t-1}$, and telescope over $t$. The result is the [discrete Tanaka formula](../../../../../../discrete-tanaka-formula.md)

$$
\boxed{(S_T-K)^+=(S_0-K)^++\sum_{t=1}^Tf(S_{t-1}-K)\Delta S_t+\frac12\sum_{t=1}^T\mathbf1_{\{S_{t-1}=K\}}(\Delta S_t)^2.}
$$

The first sum is a [martingale transform](../../../../../../martingale-transform.md); the second records the correction at the kink of the [positive part](../../../../../../positive-part-of-a-real-valued-function.md). The algebraic identity itself needs only the integer values and permitted increments, not the [martingale](../../../../../../martingale-split.md) property.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
