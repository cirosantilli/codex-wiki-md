<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use column vectors for dollar holdings $\theta_t$ and put $b=\mu-r\mathbf1$, $h=\sigma^{-1}b$ and $V=\sigma\sigma^T$. The normalized [state-price density](../../../../../state-price-density.md) is

$$
\boxed{\zeta_t=\exp(-rt-h^TW_t-\tfrac12|h|^2t),\qquad d\zeta_t=-\zeta_t(rdt+h^TdW_t).}
$$

The vector $h$ is the [market price of risk](../../../../../market-price-of-risk.md). The density $e^{rt}\zeta_t$ defines an equivalent [risk-neutral measure](../../../../../risk-neutral-measure.md), under which $W_t^{\mathbb Q}=W_t+ht$ is [Brownian motion](../../../../../brownian-motion-split.md) and every stock has drift $r$. A terminal claim $H$ with finite state-price cost is priced at $\zeta_t^{-1}\mathbb E[\zeta_TH\mid\mathcal F_t]$. Nonsingularity of $\sigma$ and the natural Brownian market information make this a [complete market](../../../../../complete-market.md); in particular the optimal nonnegative payoff below can be replicated.

Let $q=n^{-1}\mathbf1$ and $v=\sigma^Tq$. Apply the [Itô formula](../../../../../ito-s-lemma.md) to each log price, whose return variance is $V_{ii}$:

$$
d\log S_t^i=\sum_j\sigma_{ij}dW_t^j+(\mu_i-\tfrac12V_{ii})dt.
$$

Summing and dividing by $n$ proves the [geometric stock index](../../../../../geometric-stock-index.md) formula

$$
\boxed{\log(J_t/J_0)=\frac1n\left[\mathbf1^T\sigma W_t+\left(\mathbf1^T\mu-\frac12\operatorname{tr}V\right)t\right].}
$$

Thus $J_t=J_0\exp(v^TW_t+a_Jt)$, where $a_J=q^T\mu-\operatorname{tr}(V)/(2n)$. The factor $1/n$ applies to the whole bracket. The geometric average need not itself be a [self-financing portfolio](../../../../../self-financing-portfolio.md); its instantaneous drift is $a_J+|v|^2/2$.

If $\theta_t^i$ is the dollar amount invested in stock $i$, the [bank account](../../../../../bank-account.md) holds $w_t-\mathbf1^T\theta_t$. The [self-financing portfolio](../../../../../self-financing-portfolio.md) equation is

$$
\boxed{dw_t=[rw_t+\theta_t^Tb]dt+\theta_t^T\sigma dW_t.}
$$

Equivalently, $\pi_t=\theta_t/w_t$ gives $dw_t/w_t=(r+\pi_t^Tb)dt+\pi_t^T\sigma dW_t$. For share-holding notation replace $\theta_t^i$ by $S_t^i$ times the number of shares.

Static [expected utility maximization](../../../../../expected-utility-maximization.md) uses the terminal budget $\mathbb E[\zeta_Tw_T]\leq w_0$. Since $J_T$ is an exogenous positive benchmark, differentiating $U(x/J_T)$ in $x$ gives $J_T^{-1}U'(x/J_T)$. An interior [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda>0$ for the budget therefore gives

$$
\frac1{J_T}U'(w_T^*/J_T)=\lambda\zeta_T.
$$

For [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md), write $p=1/R$. Since $U'(y)=y^{-R}$, solving this marginal equation gives

$$
\boxed{w_T^*=\lambda^{-p}\zeta_T^{-p}J_T^{1-p}.}
$$

Every positive lognormal moment is finite here, so the budget determines the constant uniquely. Put

$$
K_T=\mathbb E[(\zeta_TJ_T)^{1-p}].
$$

Then

$$
\boxed{\lambda^{-p}=w_0/K_T,\qquad\lambda=(K_T/w_0)^R.}
$$

This is also a sufficiency condition: [concavity](../../../../../concave-function.md) gives $U(X/J_T)-U(w_T^*/J_T)\leq\lambda\zeta_T(X-w_T^*)$, and taking expectations and using the budget inequality proves global optimality.

To find the whole optimal process, set $c=a_J-r-|h|^2/2$ and

$$
A=(1-p)c+\frac12(1-p)^2|v-h|^2.
$$

Since $\zeta_tJ_t=J_0\exp((v-h)^TW_t+ct)$, the [moment-generating function of a normal distribution](../../../../../moment-generating-function-of-a-normal-distribution.md) gives

$$
K_T=J_0^{1-p}e^{AT},\qquad
\mathbb E[(\zeta_TJ_T)^{1-p}\mid\mathcal F_t]=(\zeta_tJ_t)^{1-p}e^{A(T-t)}.
$$

Pricing the terminal payoff yields the explicit [benchmark-relative power-utility portfolio](../../../../../benchmark-relative-power-utility-portfolio.md) wealth

$$
\boxed{w_t^*=\lambda^{-p}\zeta_t^{-p}J_t^{1-p}e^{A(T-t)}
=w_0\zeta_t^{-p}(J_t/J_0)^{1-p}e^{-At}.}
$$

Its proportional diffusion coefficient is $\ell=ph+(1-p)v$. Since the wealth diffusion coefficient for dollar fractions is $\sigma^T\pi$, replication requires

$$
\sigma^T\pi^*=ph+(1-p)\sigma^Tq.
$$

Using $\sigma^{-T}h=V^{-1}b$ gives the requested fixed proportions:

$$
\boxed{\pi^*=R^{-1}V^{-1}(\mu-r\mathbf1)+(1-R^{-1})\frac1n\mathbf1,\qquad\theta_t^*=w_t^*\pi^*.}
$$

The drift matches the [self-financing portfolio](../../../../../self-financing-portfolio.md) equation as well. Indeed, $\ell=h+(1-p)(v-h)$, so the drift of $\log w^*$ from the explicit formula is

$$
r+\frac12|h|^2-\frac12(1-p)^2|v-h|^2
=r+\ell^Th-\frac12|\ell|^2
=r+(\pi^*)^Tb-\frac12(\pi^*)^TV\pi^*.
$$

Consequently an equivalent form of the solution is

$$
\boxed{w_t^*=w_0\exp\left(\left[r+(\pi^*)^Tb-\tfrac12(\pi^*)^TV\pi^*\right]t+(\sigma^T\pi^*)^TW_t\right).}
$$

The [bank account](../../../../../bank-account.md) fraction is $1-\mathbf1^T\pi^*$, with negative values representing borrowing. The first stock term is ordinary power-utility risk exposure, while the second hedges the random benchmark. At the logarithmic limit $R=1$ the benchmark term disappears, consistently with $\log(w_T/J_T)=\log w_T-\log J_T$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
