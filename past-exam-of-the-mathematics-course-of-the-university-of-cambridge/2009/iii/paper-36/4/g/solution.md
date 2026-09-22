<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Let $p_0=\overline\Phi(2)$ and $p_1=\overline\Phi(2/\sqrt{1+V})$, where $\overline\Phi$ is the standard [normal distribution](../../../../../../normal-distribution.md) upper-tail probability. The [mixture model](../../../../../../mixture-model.md) gives

$$
\Pr(Y_i>2\mid q,V)=(1-q)p_0+qp_1.
$$

For $V>0$, [threshold inference for a mixture proportion](../../../../../../threshold-inference-for-a-mixture-proportion.md) therefore gives

$$
\boxed{\widehat q=\frac{0.15-\overline\Phi(2)}
{\overline\Phi(2/\sqrt{1+V})-\overline\Phi(2)}.}
$$

This is a method-of-moments estimate when it lies in $[0,1]$. More formally, if $K$ of the $N$ independent genes exceed the threshold, then $K\sim\operatorname{Binomial}(N,(1-q)p_0+qp_1)$, and its constrained [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) clips the displayed value to $[0,1]$. No numerical estimate is determined without the given value of $V$.

Here $p_0\approx0.02275$. Matching $15\%$ exactly requires $p_1\geq0.15$, equivalently $V\geq[2/\Phi^{-1}(0.85)]^2-1\approx2.724$. For smaller positive $V$, the maximum is at $q=1$, and a large-sample exceedance fraction this high suggests a mismatch with the prescribed component variances. Sampling fluctuation is still possible; an observed fraction need not equal its expectation. If $V=0$, the denominator vanishes and this summary gives no information about $q$. Because $p_1<1/2$ for finite $V$, matching $15\%$ in expectation also forces $q>(0.15-p_0)/(0.5-p_0)\approx0.267$. Thus the summary suggests tension with the earlier prior concentrated near $0.1$, under this mean-zero alternative model. The event is the one-sided exceedance $Y_i>2$, not $|Y_i|>2$.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
