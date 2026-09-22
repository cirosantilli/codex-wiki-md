<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $p=1-R$ and, for a constant bank rate $s$, define

$$
B(s)=s+\frac{(\mu-s)^2}{2R\sigma^2},
\qquad
\gamma(s)=\frac{\rho-pB(s)}{R}.
$$

Assume $\sigma>0$, positive [portfolio wealth](../../../../../../portfolio-wealth.md), unrestricted [stock](../../../../../../stock.md) fractions and the usual nonnegative-wealth admissibility. Once the rate has changed, the model is the [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md) with $s=r$. Put $\gamma_0=\gamma(r)$. In its finite-value regime $\gamma_0>0$, the answer is

$$
\boxed{V_0(w)=\frac{\gamma_0^{-R}w^{1-R}}{1-R},\qquad
\pi_0^*=\frac{\mu-r}{R\sigma^2},\qquad c_t^*=\gamma_0w_t.}
$$

Here $\pi_0^*$ is the fraction of [portfolio wealth](../../../../../../portfolio-wealth.md) in the [stock](../../../../../../stock.md), so the dollar holding is $\pi_0^*w_t$.

The positive-coefficient condition matters: the stated signs of $\rho$ and $R$ alone do not guarantee finite infinite-horizon [expected utility maximization](../../../../../../expected-utility-maximization.md). If $\gamma_0\leq0$, the unconstrained [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md) has value $+\infty$ for $0<R<1$ and $-\infty$ for $R>1$. The remaining calculation therefore uses $\gamma_0>0$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
