<h1 id="3/i/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $p_1$ be the alternative death [probability](../../../../../../../probability.md). The [odds ratio](../../../../../../../odds-ratio.md) specifies

$$
\frac{p_1}{1-p_1}=k\frac{p_0}{1-p_0},\qquad p_1=\frac{kp_0}{1-p_0+kp_0},\qquad 1-p_1=\frac{1-p_0}{1-p_0+kp_0}.
$$

Assume $0<p_0<1$ and $k>0$. For observed batch count $y_t$, the common combinatorial factor in the two [binomial likelihoods](../../../../../../../binomial-likelihood.md) cancels, giving the [CUSUM](../../../../../../../cusum.md) increment

$$
\begin{aligned}
W_t&=\log\frac{\binom n{y_t}p_1^{y_t}(1-p_1)^{n-y_t}}{\binom n{y_t}p_0^{y_t}(1-p_0)^{n-y_t}}\\
&=y_t\log(p_1/p_0)+(n-y_t)\log[(1-p_1)/(1-p_0)].
\end{aligned}
$$

Therefore

$$
\boxed{W_t=y_t\log k-n\log\{1+(k-1)p_0\}.}
$$

For $k>1$ large death counts add positive evidence of deterioration; for $k<1$ unusually small death counts add evidence for improvement. The score has nonpositive [expectation](../../../../../../../expected-value.md) under the null and nonnegative [expectation](../../../../../../../expected-value.md) under the specified alternative, as follows from the nonnegativity of [Kullback-Leibler divergence](../../../../../../../kullback-leibler-divergence.md). Independent, nonoverlapping batches avoid counting the same patient's outcome repeatedly.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [I](../../i.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
