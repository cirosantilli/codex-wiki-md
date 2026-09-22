<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

A [sufficient statistic](../../../../../sufficient-statistic.md) $T$ has a conditional distribution of the data given $T$ that does not depend on the parameter. In a dominated family, the [factorization criterion for sufficiency](../../../../../fisher-neyman-factorization-theorem.md) states that this is equivalent to $p_\mu(x)=h(x)g_\mu(T(x))$ for a nonnegative parameter-free $h$. Bayes' formula then gives a [posterior distribution](../../../../../bayesian-posterior.md) proportional to $\pi(\mu)g_\mu(T(x))$, because $h(x)$ cancels from numerator and normalizing denominator. Thus the posterior depends on the data only through $T$.

For the normal sample,

$$
\sum_i(x_i-\mu)^2=\sum_i(x_i-\bar x)^2+n(\bar x-\mu)^2.
$$

The first term is parameter-free, so the factorization proves sufficiency of $\bar X$. Combining its likelihood with the normal prior and completing the square gives

$$
\boxed{M\mid X_1,\ldots,X_n\sim N\left(\frac{n\tau^2}{1+n\tau^2}\bar x,\frac{\tau^2}{1+n\tau^2}\right).}
$$

The prior [predictive distribution](../../../../../predictive-distribution.md) of the sample mean is obtained from $\bar X=M+\varepsilon$, $\varepsilon\sim N(0,1/n)$ [independent](../../../../../independent-random-variables.md) of $M$:

$$
\boxed{\bar X\sim N(0,\tau^2+1/n).}
$$

Define the [Bayes factor](../../../../../bayes-factor.md) $B_{01}$ as the marginal likelihood under $H_0$ divided by that under $H_1$. The common residual factor cancels, so it is the ratio of the densities of $\bar X$ under these two hypotheses:

$$
\boxed{B_{01}=\sqrt{1+n\tau^2}\,
\exp\left[-\frac{n^2\tau^2\bar x^2}{2(1+n\tau^2)}\right].}
$$

The reverse [Bayes factor](../../../../../bayes-factor.md) is its reciprocal. At $|\bar x|=1.96/\sqrt n$,

$$
B_{01}=\sqrt{1+n\tau^2}
\exp\left[-\frac{1.96^2}{2}\frac{n\tau^2}{1+n\tau^2}\right]
\sim\tau\sqrt n\,e^{-1.96^2/2}\longrightarrow\infty
$$

for a fixed positive $\tau$. Thus the frequentist test is at its rejection threshold while fixed prior odds give increasingly strong posterior support for the point null. This is the [Jeffreys-Lindley paradox for a Gaussian point null](../../../../../jeffreys-lindley-paradox-for-a-gaussian-point-null.md): the standardized statistic stays fixed, but the observed effect tends to zero and the fixed-scale alternative spreads predictive mass much more widely. There is no logical contradiction, since the procedures compare hypotheses using different calibrations. For the degenerate $\tau=0$ the hypotheses coincide and $B_{01}=1$.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
