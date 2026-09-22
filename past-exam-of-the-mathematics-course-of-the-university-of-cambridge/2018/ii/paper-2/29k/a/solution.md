<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The price process is a [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) with

$$
\frac{dS_t}{S_t}=
\left(\mu+\frac12\sigma^2\right)dt+\sigma dB_t.
$$

Put

$$
\vartheta=\frac{\mu+\sigma^2/2-r}{\sigma}
$$

and define the equivalent measure $Q$ on $\mathcal F_T$ by the [exponential Brownian martingale](../../../../../../exponential-brownian-martingale.md)

$$
\frac{dQ}{d\mathbb P}
=\exp\left(-\vartheta B_T-\frac12\vartheta^2T\right).
$$

The [Cameron-Martin-Girsanov theorem](../../../../../../girsanov-theorem.md) says that $W_t^Q=B_t+\vartheta t$ is Brownian motion under $Q$. Therefore

$$
S_t=S_0\exp\left(\sigma W_t^Q+
\left(r-\frac12\sigma^2\right)t\right),
$$

so $e^{-rt}S_t$ is a $Q$-martingale. This is the unique [equivalent martingale measure](../../../../../../risk-neutral-measure.md), since cancellation of the single Brownian risk forces the displayed drift shift.

By [risk-neutral valuation](../../../../../../risk-neutral-pricing.md),

$$
\pi_C=e^{-rT}\mathbb E_Qf(S_T).
$$

Writing $W_T^Q=\sqrt T Y$ with $Y\sim N(0,1)$ gives

$$
\boxed{
\pi_C=e^{-rT}\int_{-\infty}^{\infty}
f\left(S_0e^{\sigma\sqrt T y+(r-\sigma^2/2)T}
\right)
\frac{e^{-y^2/2}}{\sqrt{2\pi}} dy.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
