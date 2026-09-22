<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [market price of risk](../../../../../../market-price-of-risk.md) $\lambda_t=(\mu-rS_t)/\sigma$. The [Girsanov theorem](../../../../../../girsanov-theorem.md), with the hypotheses allowed in the question, gives an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) $\mathbb Q$ under which

$$
dW_t^{\mathbb Q}=dW_t+\lambda_tdt,\qquad
dS_t=rS_tdt+\sigma dW_t^{\mathbb Q}.
$$

Thus the [stock](../../../../../../stock.md) under the [risk-neutral measure](../../../../../../risk-neutral-measure.md) is a linear [Gaussian](../../../../../../normal-distribution.md) diffusion. In particular, for $\tau=T-t$ its conditional mean and standard deviation are

$$
m=e^{r\tau}S_t,\qquad
v=\sigma\sqrt{\frac{e^{2r\tau}-1}{2r}}.
$$

Put $\phi(x)=(2\pi)^{-1/2}e^{-x^2/2}$ and let $\Phi$ be the standard [normal distribution](../../../../../../normal-distribution.md) function. For $N\sim N(0,1)$,

$$
\mathbb E(m+vN-K)^+=(m-K)\Phi((m-K)/v)+v\phi((m-K)/v),
$$

since $\int_{-d}^\infty x\phi(x)dx=\phi(d)$. Discounting this [expectation](../../../../../../expected-value.md) gives the [call price in an arithmetic stock model with interest](../../../../../../call-price-in-an-arithmetic-stock-model-with-interest.md). A particularly convenient expression is

$$
\begin{aligned}
\nu(\tau)&=\sigma\sqrt{\frac{1-e^{-2r\tau}}{2r}},
&d(t,s)&=\frac{s-Ke^{-r\tau}}{\nu(\tau)},\\
\boxed{C(t,s)}&=\boxed{(s-Ke^{-r\tau})\Phi(d(t,s))+\nu(\tau)\phi(d(t,s))}.
\end{aligned}
$$

At maturity define $C(T,s)=(s-K)^+$. This value is nonnegative because it is a discounted [expectation](../../../../../../expected-value.md) of a nonnegative payoff.

For $t<T$, hold $\pi_t=C_s(t,S_t)$ shares and hold $\beta_t=[C(t,S_t)-\pi_tS_t]/B_t$ units of the [continuous-time bank account](../../../../../../continuous-time-bank-account.md). The pricing function solves

$$
C_t+rsC_s+\tfrac12\sigma^2C_{ss}-rC=0.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) under the physical measure therefore gives

$$
dC(t,S_t)=C_s(t,S_t)dS_t+r[C(t,S_t)-S_tC_s(t,S_t)]dt
=\pi_t dS_t+\beta_t dB_t.
$$

This proves [self-financing](../../../../../../self-financing-portfolio.md) and terminal replication, with wealth always $C(t,S_t)\geq0$. The coefficients are locally smooth before maturity, and the strategy extends to maturity through its continuous wealth limit and the square-integrable discounted payoff representation.

To see minimality, any other nonnegative [self-financing portfolio](../../../../../../self-financing-portfolio.md) replicating the payoff has discounted wealth a nonnegative [local martingale](../../../../../../local-martingale.md) under $\mathbb Q$, hence a [supermartingale](../../../../../../supermartingale.md). Its initial capital $x$ must satisfy $x\geq\mathbb E^{\mathbb Q}[e^{-rT}(S_T-K)^+]=C(0,S_0)$. The strategy constructed above attains equality. Thus

$$
\boxed{x_{\min}=C(0,S_0).}
$$

The additive physical diffusion may take negative [stock](../../../../../../stock.md) values; the formula and nonnegative replicating wealth remain valid. Replacing it by a multiplicative Black–Scholes diffusion would give the wrong price and hedge.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
