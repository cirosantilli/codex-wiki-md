<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the nondegenerate case $\sigma>0$ and an integer trading horizon $T$. For [exponential utility](../../../../../../constant-absolute-risk-aversion-utility.md), maximize the negative of the exponential loss, equivalently minimize its [expectation](../../../../../../expected-value.md). Conditional on past information, a [predictable](../../../../../../predictable-process.md) choice $\pi$ has

$$
\mathbb E[e^{-\gamma\pi\Delta S_t}\mid\mathcal F_{t-1}]=\exp\left(-\gamma\mu\pi+\tfrac12\gamma^2\sigma^2\pi^2\right).
$$

Complete the square:

$$
-\gamma\mu\pi+\tfrac12\gamma^2\sigma^2\pi^2=\tfrac12\gamma^2\sigma^2\left(\pi-\frac\mu{\gamma\sigma^2}\right)^2-\frac{\mu^2}{2\sigma^2}.
$$

Thus the minimum conditional multiplier is $e^{-\kappa}$ with $\kappa=\mu^2/(2\sigma^2)$. [Backward induction](../../../../../../backward-induction.md) starts with terminal loss $e^{-\gamma x}$ and gives the minimal continuation loss $e^{-\gamma x-\kappa(T-t)}$. [Independence](../../../../../../independent-random-variables.md) of the next increment justifies the same conditional minimization for every history, not just deterministic trading plans. Hence [exponential-utility trading with Gaussian increments](../../../../../../exponential-utility-trading-with-gaussian-increments.md) gives

$$
\boxed{\pi_t^*=\frac\mu{\gamma\sigma^2},\quad1\leq t\leq T,\qquad V_0(x)=-\exp\left(-\gamma x-\frac{T\mu^2}{2\sigma^2}\right).}
$$

These are constant numbers of shares, not constant wealth fractions. Strategies with infinite exponential loss have expected utility $-\infty$ and cannot improve this finite value. If $\sigma=0$, the usual formula is inapplicable: with $\mu=0$ trading has no effect, while a nonzero deterministic increment admits unbounded riskless gains and no finite maximizing position.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
