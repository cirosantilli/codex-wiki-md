<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The principle [terminal correlation does not identify adapted stock volatility](../../../../../../terminal-correlation-does-not-identify-adapted-stock-volatility.md) exposes a false printed assertion for the [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) defined in the introduction. Take $r=0$, $S_0=S'_0=1$, and

$$
S_t=e^{B_t-t/2},\qquad S'_t=\tfrac12(1+S_t).
$$

Then $dS_t=S_t\,dB_t$ and

$$
dS'_t=\tfrac12S_t\,dB_t=S'_t\frac{S_t}{1+S_t}\,dB_t.
$$

Hence $\sigma_t=1$ and $\sigma'_t=S_t/(1+S_t)$ are bounded. Both terminal prices have positive finite [variance](../../../../../../variance-split.md) and are perfectly correlated, because one is a positive affine function of the other. Nevertheless **$\boxed{\int_0^1(\sigma_t-\sigma'_t)^2dt=\int_0^1\frac{dt}{(1+S_t)^2}>0}$** on every continuous finite stock path. Equal initial prices fix the means, not the affine slope.

Here is the exact general conclusion and the intended qualified proof. Bounded volatilities make these zero-rate stochastic exponentials true square-integrable [martingales](../../../../../../martingale-split.md). Writing $s_0=S_0=S'_0$, perfect terminal correlation gives $S_1-s_0=c(S'_1-s_0)$ for some $c>0$. [Conditional expectation](../../../../../../conditional-expectation.md) therefore gives $S_u-s_0=c(S'_u-s_0)$ for every $0\leq u\leq1$. Comparing stochastic integrals, the [Itô isometry](../../../../../../ito-isometry.md) yields

$$
\sigma_uS_u=c\sigma'_uS'_u\quad\text{for }du\,d\mathbb P\text{-almost every }(u,\omega).
$$

This relation need not imply equality of the volatilities.

The [terminal proportionality identifies bounded stock volatility](../../../../../../terminal-proportionality-identifies-bounded-stock-volatility.md) criterion repairs the statement. If one additionally assumes equal terminal [variances](../../../../../../variance-split.md), then $c=1$ and the whole stock paths coincide, so positivity gives $\sigma=\sigma'$ almost everywhere and the requested integral is zero. The same repair follows if terminal proportionality $S_1=cS'_1$ is assumed: equal [martingale](../../../../../../martingale-split.md) means force $c=1$, after which the conditional-[expectation](../../../../../../expected-value.md) and [Itô isometry](../../../../../../ito-isometry.md) argument applies. This proves the intended conclusion under a sufficient additional hypothesis without treating centered correlation as uncentered proportionality.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
