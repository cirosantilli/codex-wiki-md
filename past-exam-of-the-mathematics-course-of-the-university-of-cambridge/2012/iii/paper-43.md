# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_43.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [With transaction costs](#5/with-transaction-costs)
    - [i](#5/with-transaction-costs/i)
      - [Solution](#5/with-transaction-costs/i/solution)
    - [ii](#5/with-transaction-costs/ii)
      - [Solution](#5/with-transaction-costs/ii/solution)
    - [iii](#5/with-transaction-costs/iii)
      - [Solution](#5/with-transaction-costs/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work under the money-market [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), with $r_0\geq0$. The [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is $P(0,T)=\mathbb E[\exp(-\int_0^T r_sds)]$. For this [CIR model](../../../mathematical-finance.md#cox-ingersoll-ross-model), write $p(\tau,r)=A(\tau)e^{-B(\tau)r}$. The [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) gives

$$
\partial_\tau p=(a-br)\partial_rp+\tfrac12\sigma^2r\partial_{rr}p-rp,\qquad p(0,r)=1.
$$

Matching the constant and linear coefficients of $r$ yields

$$
B'=1-bB-\tfrac12\sigma^2B^2,\qquad A'/A=-aB,\qquad B(0)=0,\quad A(0)=1.
$$

For [CIR bond pricing](../../../mathematical-finance.md#cir-bond-pricing), solving this [Riccati equation](../../../analysis.md#riccati-equation) and integrating the scalar equation for $A$, put $\gamma=\sqrt{b^2+2\sigma^2}$ and $D(\tau)=(\gamma+b)(e^{\gamma\tau}-1)+2\gamma$. Then

$$
B(\tau)=\frac{2(e^{\gamma\tau}-1)}{D(\tau)},\qquad A(\tau)=\left[\frac{2\gamma e^{(b+\gamma)\tau/2}}{D(\tau)}\right]^{2a/\sigma^2}.
$$

Substitution verifies both equations and their initial conditions. The discounted candidate solves the [martingale](../../../martingale.md) pricing equation; its boundedness on finite horizons, or [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula), identifies it with the [conditional expectation](../../../measure-theory.md#conditional-expectation). **The answer is $\boxed{P(0,T)=A(T)e^{-B(T)r_0}}$.** More generally the same coefficients give $P(t,T)=A(T-t)e^{-B(T-t)r_t}$.

The [CIR model](../../../mathematical-finance.md#cox-ingersoll-ross-model) mean reverts to $a/b$ and has volatility $\sigma\sqrt r$, so it remains nonnegative and its fluctuation size depends on the rate level. For positive initial rate, zero is inaccessible if $2a\geq\sigma^2$; below this threshold zero is reachable but the process remains nonnegative. Its stationary law is a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution), of shape $2a/\sigma^2$ and rate $2b/\sigma^2$. Explicit affine bond prices and nonnegative rates are useful features. Limitations include exclusion of negative rates, restricted volatility behavior and a single stochastic factor; the time-homogeneous parameter family cannot fit an arbitrary initial term structure exactly.

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [futures contract](../../../mathematical-finance.md#futures-contract) fixes a maturity and underlying quantity, but its quoted delivery price is marked to market: gains and losses from quote changes are settled through the margin account, typically daily. A newly settled position has zero contract value; the quoted futures price is not an upfront purchase price for that position. At maturity the quote equals the spot price. In the continuous-settlement idealization, discounted futures gains must be local [martingales](../../../martingale.md) under the money-market [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure). Thus the quote has zero pricing-measure drift. Assuming the relevant [integrability](../../../measure-theory.md#integrability) makes it a true [martingale](../../../martingale.md), **$\boxed{F_{tT}=\mathbb E_Q[S_T\mid\mathcal F_t]}$.**

This is a [futures pricing](../../../mathematical-finance.md#futures-pricing) formula. In contrast, an unsettled [forward contract](../../../mathematical-finance.md#forward-contract) has delivery quote $\mathbb E_Q[D_{tT}S_T\mid\mathcal F_t]/\mathbb E_Q[D_{tT}\mid\mathcal F_t]$, where $D_{tT}=e^{-\int_t^T r_udu}$. Stochastic [interest rates](../../../mathematical-finance.md#interest-rate) can make the two quotes differ. [Contango](../../../mathematical-finance.md#contango) means the futures quote is above spot for the maturity considered, while [backwardation](../../../mathematical-finance.md#backwardation) means it is below spot; futures curves are correspondingly described as rising or falling when comparing maturities.

For the [Multivariate Ornstein-Uhlenbeck process](../../../stochastic-process.md#multivariate-ornstein-uhlenbeck-process), multiplication by the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) $e^{At}$ gives $d(e^{At}X_t)=e^{At}dB_t$, hence

$$
\boxed{X_t=e^{-At}X_0+\int_0^t e^{-A(t-u)}dB_u.}
$$

For deterministic $X_0=x_0$, the [Gaussian distribution](../../../probability-theory.md#normal-distribution) has mean $e^{-At}x_0$ and [covariance](../../../variance.md#covariance)

$$
C_t=\int_0^t e^{-Au}e^{-A^{\mathsf T}u}\,du.
$$

Equivalently $\dot C=I-AC-CA^{\mathsf T}$, $C_0=0$. No symmetry or invertibility of $A$ is required. This [covariance](../../../variance.md#covariance) can also be evaluated from a single block [matrix exponential](../../../linear-operator-theory.md#matrix-exponential): if the upper-right block of $\exp(t\left(\begin{smallmatrix}-A&I\\0&A^{\mathsf T}\end{smallmatrix}\right))$ is $H_t$, then $C_t=H_te^{-A^{\mathsf T}t}$. If $X_0$ is random, these assertions hold conditionally on $X_0$; the unconditional law need not be Gaussian. A stationary Gaussian law exists when the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $A$ have positive real parts, but stability is unnecessary for the finite-time formulas.

For $\tau=T-t$, the conditional mean of $X_T$ is $e^{-A\tau}X_t$ and its conditional [covariance](../../../variance.md#covariance) is $C_\tau$. The Gaussian exponential-moment formula therefore gives **the explicit quote**

$$
\boxed{F_{tT}=\exp\left(b^{\mathsf T}e^{-A\tau}X_t+\tfrac12 b^{\mathsf T}C_\tau b\right).}
$$

It tends to $e^{b\cdot X_t}=S_t$ as $T\downarrow t$, as required.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For centered square-integrable variables with positive [variances](../../../variance.md), the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) is

$$
\rho(X,X')=\frac{\mathbb E[XX']}{\sqrt{\mathbb E[X^2]\mathbb E[(X')^2]}}.
$$

Put $v=\sqrt{\mathbb E[X^2]}$ and $v'=\sqrt{\mathbb E[(X')^2]}$. Then

$$
\mathbb E\left[\left(\frac Xv-\frac{X'}{v'}\right)^2\right]=2(1-\rho).
$$

Thus **$\boxed{\rho=1\iff X=(v/v')X'\text{ almost surely}}$**, with positive proportionality factor. Conversely positive proportionality immediately gives correlation one. For variables with nonzero means, this criterion applies to their centered versions and yields an affine, not necessarily proportional, relationship. That distinction is essential for the positive stock prices below.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Assume positive deterministic initial stock prices and finite, positive terminal [variances](../../../variance.md), as required to define the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient). The explicit stochastic-exponential solutions with constant volatilities give

$$
\frac{S_t}{S'_t}=\frac{S_0}{S'_0}\exp\left[(\sigma-\sigma')B_t-\tfrac12(\sigma^2-(\sigma')^2)t\right].
$$

The common, possibly random, accumulated interest rate cancels. If $\sigma=\sigma'$, this ratio is a positive constant, so the prices are perfectly correlated.

Conversely, perfect correlation would give $S_t=cS'_t+d$ almost surely for constants $c>0,d$. If $\sigma\ne\sigma'$, the displayed ratio is a nonconstant variable with a [lognormal distribution](../../../probability-theory.md#log-normal-distribution) with full support $(0,\infty)$. If $d>0$, the ratio would always exceed $c$, and if $d<0$ it would always be below $c$, both impossible. If $d=0$, the ratio would be constant, also impossible. **Therefore $\boxed{\rho(S_t,S'_t)=1\iff\sigma=\sigma'}$**, whenever the stated terminal [variances](../../../variance.md) exist and are positive. No deterministic-interest assumption is needed. Degenerate terminal prices, for example zero volatilities and deterministic rates, have undefined correlation and must be excluded.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The principle [terminal correlation does not identify adapted stock volatility](../../../variance.md#terminal-correlation-does-not-identify-adapted-stock-volatility) exposes a false printed assertion for the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) defined in the introduction. Take $r=0$, $S_0=S'_0=1$, and

$$
S_t=e^{B_t-t/2},\qquad S'_t=\tfrac12(1+S_t).
$$

Then $dS_t=S_t\,dB_t$ and

$$
dS'_t=\tfrac12S_t\,dB_t=S'_t\frac{S_t}{1+S_t}\,dB_t.
$$

Hence $\sigma_t=1$ and $\sigma'_t=S_t/(1+S_t)$ are bounded. Both terminal prices have positive finite [variance](../../../variance.md) and are perfectly correlated, because one is a positive affine function of the other. Nevertheless **$\boxed{\int_0^1(\sigma_t-\sigma'_t)^2dt=\int_0^1\frac{dt}{(1+S_t)^2}>0}$** on every continuous finite stock path. Equal initial prices fix the means, not the affine slope.

Here is the exact general conclusion and the intended qualified proof. Bounded volatilities make these zero-rate stochastic exponentials true square-integrable [martingales](../../../martingale.md). Writing $s_0=S_0=S'_0$, perfect terminal correlation gives $S_1-s_0=c(S'_1-s_0)$ for some $c>0$. [Conditional expectation](../../../measure-theory.md#conditional-expectation) therefore gives $S_u-s_0=c(S'_u-s_0)$ for every $0\leq u\leq1$. Comparing stochastic integrals, the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) yields

$$
\sigma_uS_u=c\sigma'_uS'_u\quad\text{for }du\,d\mathbb P\text{-almost every }(u,\omega).
$$

This relation need not imply equality of the volatilities.

The [terminal proportionality identifies bounded stock volatility](../../../variance.md#terminal-proportionality-identifies-bounded-stock-volatility) criterion repairs the statement. If one additionally assumes equal terminal [variances](../../../variance.md), then $c=1$ and the whole stock paths coincide, so positivity gives $\sigma=\sigma'$ almost everywhere and the requested integral is zero. The same repair follows if terminal proportionality $S_1=cS'_1$ is assumed: equal [martingale](../../../martingale.md) means force $c=1$, after which the conditional-[expectation](../../../probability-theory.md#expected-value) and [Itô isometry](../../../stochastic-calculus.md#ito-isometry) argument applies. This proves the intended conclusion under a sufficient additional hypothesis without treating centered correlation as uncentered proportionality.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

**Yes: different adapted volatilities can give perfectly correlated terminal prices.** The counterexample in part ii already establishes this with one nonconstant volatility. Both can be nonconstant as well. Put $h(x)=1+\tfrac12\tanh x$ and take

$$
S_t=\mathcal E\left(\int_0^\cdot h(B_u)dB_u\right)_t,\qquad S'_t=\tfrac12(1+S_t),\qquad r=0.
$$

The [Doléans-Dade exponential](../../../stochastic-calculus.md#doleans-dade-exponential) has volatility $h(B_t)$, bounded between $1/2$ and $3/2$. The second stock has volatility $h(B_t)S_t/(1+S_t)$, also bounded and nonconstant. Their squared volatility difference integrates to

$$
\int_0^t\frac{h(B_u)^2}{(1+S_u)^2}\,du>0\quad(t>0).
$$

The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) and boundedness give true square-integrable [martingales](../../../martingale.md), and the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives positive [variance](../../../variance.md) for each $t>0$. Yet $S'_t=(1+S_t)/2$ gives correlation one. The mechanism is positive affine dependence, not equality of the multiplicative volatility coefficients; it also explains the failure of the literal part-ii premise.

## 4

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the [quadratic Ornstein-Uhlenbeck state-price density](../../../mathematical-finance.md#quadratic-ornstein-uhlenbeck-state-price-density), apply the [Itô's formula](../../../stochastic-calculus.md#ito-s-lemma) under the reference probability measure. Since $f'(x)=x$ and $f''(x)=1$,

$$
d\zeta_t=e^{-\alpha t}\sigma X_t\,dB_t-e^{-\alpha t}\left[\alpha a-\tfrac12\sigma^2+(\lambda+\tfrac12\alpha)X_t^2\right]dt.
$$

The [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is a true [martingale](../../../martingale.md) on finite horizons by the finite moments of the [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process). **A uniform sufficient condition is $\boxed{\alpha\geq\sigma^2/(2a)}$**, making the finite-variation drift nonpositive. This is also the condition for nonpositive drift at every state.

Use the positive [state-price density](../../../mathematical-finance.md#state-price-density) $\zeta$ to price a terminal payoff $H$ by $\Pi_t(H)=\mathbb E[\zeta_TH\mid\mathcal F_t]/\zeta_t$. The riskless account must cancel the drift of $\zeta$, giving the [short rate](../../../mathematical-finance.md#short-rate)

$$
\boxed{r_t=\frac{\alpha a-\sigma^2/2+(\lambda+\alpha/2)X_t^2}{a+X_t^2/2}=\alpha+\frac{\lambda X_t^2-\sigma^2/2}{a+X_t^2/2}.}
$$

This pricing system is consistent with a money-market [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure): with $M_t=e^{\int_0^tr_udu}$, the process $\zeta_tM_t/\zeta_0$ is a [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) whose diffusion coefficient $\sigma X_t/f(X_t)$ is bounded. The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) makes it a true density [martingale](../../../martingale.md). The original [Brownian motion](../../../brownian-motion.md) is for the reference measure, not automatically for this new pricing measure.

For $X_0=x_0$, the OU second moment is $\mathbb E X_T^2=x_0^2e^{-2\lambda T}+\sigma^2(1-e^{-2\lambda T})/(2\lambda)$. Thus **the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is**

$$
\boxed{P(0,T)=e^{-\alpha T}\frac{a+\tfrac12x_0^2e^{-2\lambda T}+\frac{\sigma^2}{4\lambda}(1-e^{-2\lambda T})}{a+\tfrac12x_0^2}.}
$$

Conditionally at time $t$, replace $T$ by $T-t$ and $x_0$ by $X_t$.

The [short rate](../../../mathematical-finance.md#short-rate) is nonnegative under the condition above, increases with $X_t^2$, and lies between $\alpha-\sigma^2/(2a)$ and $\alpha+2\lambda$. The model is tractable but imposes fixed rate bounds, identical rates for opposite values of $X$, and a restricted one-factor term structure. Its long-maturity yield is $\alpha$. These structural restrictions, including exclusion of negative rates under the supermartingale condition, may be unsuitable for a general interest-rate fit.

## 5

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For $0\leq s\leq1$, pointwise concavity of the [utility function](../../../utility-function.md) gives

$$
U((s\theta+(1-s)\eta)X)\geq sU(\theta X)+(1-s)U(\eta X).
$$

Taking [expectations](../../../probability-theory.md#expected-value) is legitimate because all three values are finite. **Therefore $\boxed{F(s\theta+(1-s)\eta)\geq sF(\theta)+(1-s)F(\eta)}$: $F$ is concave.** Strict concavity is not required and is not asserted.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

For [secant domination for expected utility derivatives](../../../utility-function.md#secant-domination-for-expected-utility-derivatives), at each sample value $x$ set $g_x(\theta)=U(\theta x)$. This is a differentiable concave function, regardless of the sign of $x$. Fix $\theta_0$ and $\delta>0$. For $\theta\in[\theta_0-\delta,\theta_0+\delta]$, concavity bounds its derivative between the two outer secant slopes:

$$
\frac{g_x(\theta_0+2\delta)-g_x(\theta_0+\delta)}\delta\leq g'_x(\theta)\leq\frac{g_x(\theta_0-\delta)-g_x(\theta_0-2\delta)}\delta.
$$

Because $U<0$, finiteness of $F$ means $\mathbb E|U(\eta X)|<\infty$ at each of these four endpoints. Their absolute values divided by $\delta$ therefore give a common integrable bound on $|g'_X(\theta)|$. Difference quotients satisfy the same bound by the [mean value theorem](../../../calculus.md#mean-value-theorem). The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) permits differentiation under the [expectation](../../../probability-theory.md#expected-value), and pointwise continuity of $XU'(\theta X)$ with the same bound gives continuity of the derivative. **Hence $\boxed{F'(\theta)=\mathbb E[XU'(\theta X)]}$ and $F\in C^1(\mathbb R)$.** This argument proves absolute [integrability](../../../measure-theory.md#integrability) of the displayed derivative; no unjustified differentiation assumption is needed.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

A strictly increasing differentiable concave [utility function](../../../utility-function.md) on all of $\mathbb R$ has $U'(x)>0$ everywhere. Otherwise monotonicity and the decreasing derivative would make it constant on a right half-line. Its tangent at zero also shows $U(x)\to-\infty$ as $x\to-\infty$.

If $X$ has only one sign, the stated second alternative already holds. Otherwise both $\mathbb P(X<0)$ and $\mathbb P(X>0)$ are positive. As $\theta\to\infty$, $-U(\theta X)$ tends to infinity on $\{X<0\}$; as $\theta\to-\infty$, it does so on $\{X>0\}$. Since $-U\geq0$, [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) implies $F(\theta)\to-\infty$ at both ends. Continuity gives a finite maximizer $\theta_*$, and differentiability gives $F'(\theta_*)=0$.

For [optimal marginal utility as a one-period pricing density](../../../utility-function.md#optimal-marginal-utility-as-a-one-period-pricing-density), put $Z=U'(\theta_*X)$. It is strictly positive. On $\{|X|\geq1\}$ it is bounded by $|X|U'(\theta_*X)$, whose [expectation](../../../probability-theory.md#expected-value) is finite by part ii. On $\{|X|<1\}$ continuity bounds $U'$ on the compact interval $[-|\theta_*|,|\theta_*|]$. Thus $Z$ is integrable and $XZ$ is absolutely integrable. **Consequently $\boxed{\mathbb E[XZ]=0}$**. Normalizing $Z$ by its positive [expectation](../../../probability-theory.md#expected-value), if desired, makes it a probability density with the same zero pricing [expectation](../../../probability-theory.md#expected-value).

<h3 id="5/with-transaction-costs">With transaction costs</h3>

↑ **Parent:** [5](#5)

<h4 id="5/with-transaction-costs/i">i</h4>

↑ **Parent:** [With transaction costs](#5/with-transaction-costs)

<h5 id="5/with-transaction-costs/i/solution">Solution</h5>

↑ **Parent:** [I](#5/with-transaction-costs/i)

Under a [proportional transaction cost](../../../utility-function.md#proportional-transaction-cost), the sample gain $h_x(\theta)=\theta x-\varepsilon|\theta|$ is concave when $\varepsilon\geq0$. The [utility function](../../../utility-function.md) is increasing and concave, so

$$
U(h_x(s\theta+(1-s)\eta))\geq U(sh_x(\theta)+(1-s)h_x(\eta))\geq sU(h_x(\theta))+(1-s)U(h_x(\eta)).
$$

Take finite [expectations](../../../probability-theory.md#expected-value). **Thus $\boxed{G\text{ is concave}}$.** The monotonicity of $U$ is essential to composing it with the concave transaction-cost payoff.

<h4 id="5/with-transaction-costs/ii">ii</h4>

↑ **Parent:** [With transaction costs](#5/with-transaction-costs)

<h5 id="5/with-transaction-costs/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/with-transaction-costs/ii)

On each open half-line the sample objective is a utility of a linear gain: $U(\theta(X-\varepsilon))$ on the positive half-line, and $U(\theta(X+\varepsilon))$ on the negative half-line. On a compact subinterval wholly inside either half-line, the secant domination argument from the frictionless part ii applies verbatim, using finiteness of $G$ at four surrounding points. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore gives **the derivatives**

$$
\boxed{G'(\theta)=\begin{cases}\mathbb E[(X-\varepsilon)U'(\theta(X-\varepsilon))],&\theta>0,\\\mathbb E[(X+\varepsilon)U'(\theta(X+\varepsilon))],&\theta<0.\end{cases}}
$$

They are continuous on their respective half-lines. Near zero, the same outer secants of the globally concave sample objective bound its one-sided slopes. Dominated convergence consequently gives

$$
G'_+(0)=U'(0)(\mathbb EX-\varepsilon),\qquad G'_-(0)=U'(0)(\mathbb EX+\varepsilon).
$$

Here $\mathbb E|X|<\infty$: the frictionless derivative at zero already proves it, since $U'(0)>0$. Thus zero generally has a transaction-cost kink; when $\varepsilon=0$ the two formulas agree.

<h4 id="5/with-transaction-costs/iii">iii</h4>

↑ **Parent:** [With transaction costs](#5/with-transaction-costs)

<h5 id="5/with-transaction-costs/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/with-transaction-costs/iii)

For [marginal utility pricing with proportional transaction costs](../../../utility-function.md#marginal-utility-pricing-with-proportional-transaction-costs), if $X-\varepsilon\geq0$ almost surely or $-X-\varepsilon\geq0$ almost surely, the source's second alternative holds. Otherwise $\mathbb P(X<\varepsilon)>0$ and $\mathbb P(X>-\varepsilon)>0$. The [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) argument now gives $G(\theta)\to-\infty$ at both ends, since a large positive holding loses on the first event and a large negative holding loses on the second. Let $\theta_*$ be a finite maximizer.

If $\theta_*>0$, set $Z_0=U'(\theta_*(X-\varepsilon))$. The derivative condition gives $\mathbb E[XZ_0]=\varepsilon\mathbb E Z_0$. As before, split according to $|X-\varepsilon|\geq1$ to obtain [integrability](../../../measure-theory.md#integrability) of $Z_0$ from the absolutely integrable derivative, with a compact-set bound on the complement. If $\theta_*<0$, use $Z_0=U'(\theta_*(X+\varepsilon))$ and obtain $\mathbb E[XZ_0]=-\varepsilon\mathbb E Z_0$. In either case normalize $Z=Z_0/\mathbb E Z_0$; then $Z>0$, $\mathbb EZ=1$, and $XZ$ is absolutely integrable.

If $\theta_*=0$, a concave maximum has $G'_-(0)\geq0\geq G'_+(0)$, so $\mathbb EX\in[-\varepsilon,\varepsilon]$. Choose $Z=1$. **In every case of this first alternative, $\boxed{\mathbb E[XZ]\in[-\varepsilon,\varepsilon]}$.** The normalization establishes a stronger, economically meaningful statement than the literal unnormalized condition: the expected gain under the resulting density lies inside the transaction-cost spread.

## 6

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

For zero drift, the reflection principle gives the known [Brownian first-passage time](../../../markov-process.md#brownian-first-passage-time) density

$$
h_0(t)=\frac{a}{\sqrt{2\pi t^3}}e^{-a^2/(2t)},\qquad t>0.
$$

To obtain a general drift, on a fixed finite horizon use the exponential [martingale](../../../martingale.md) $M_t=e^{cB_t-c^2t/2}$ as change-of-measure density. The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds for constant $c$, and the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) says that the coordinate process $B$ has drift $c$ under the new measure. Thus the hitting law of $B$ under that measure is the law of $B+ct$ under the original measure. [Conditional expectation](../../../measure-theory.md#conditional-expectation) of $M_T$ at a hitting time bounded by $T$ equals its stopped value, by the [martingale](../../../martingale.md) [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale). At $H_a=t$ this value is $e^{ca-c^2t/2}$. The [drifted Brownian first-passage density](../../../markov-process.md#drifted-brownian-first-passage-density) is obtained by multiplying $h_0$, giving **$\boxed{h_c(t)=a e^{-(a-ct)^2/(2t)}/\sqrt{2\pi t^3}}$.**

To verify the integrated formula, put $u=(a-cT)/\sqrt T$ and $v=(-a-cT)/\sqrt T$. The identity $e^{2ac}\phi(v)=\phi(u)$ for the standard normal density gives

$$
\frac d{dT}[\overline\Phi(u)+e^{2ac}\Phi(v)]=\phi(u)\frac{a+cT+a-cT}{2T^{3/2}}=h_c(T).
$$

Both terms vanish as $T\downarrow0$, so **$\boxed{\mathbb P(H_a\leq T)=\overline\Phi((a-cT)/\sqrt T)+e^{2ac}\Phi((-a-cT)/\sqrt T)}$.** The distribution has total mass one for $c\geq0$ and mass $e^{2ac}$ for $c<0$; in the latter case the remaining probability is an atom at infinity.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Under the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) pricing measure, write $\log S_t/\sigma=B_t+ct$, where $c=(r-\sigma^2/2)/\sigma$. Brownian continuity and immediate crossing on reaching a level make the strict up-crossing time equal almost surely to the hitting time $H_a$. Its finite-time law has no atom at $T$, so the convention before rather than at expiry does not affect the price.

For [truncated discounted Brownian first passage](../../../markov-process.md#truncated-discounted-brownian-first-passage), since payment occurs at the hitting time, discount there, not at expiry. The [one-touch option](../../../mathematical-finance.md#one-touch-option) price is

$$
V_0=\mathbb E[e^{-rH_a}\mathbf1\{H_a\leq T\}]=\int_0^T e^{-rt}h_c(t)dt.
$$

Set $d=\sqrt{c^2+2r}=|r+\sigma^2/2|/\sigma$. The expression under the square root is nonnegative for every real $r$, by this Black-Scholes identity. The discounted density satisfies $e^{-rt}h_c(t)=e^{a(c-d)}h_d(t)$. Applying part i yields **the closed price**

$$
\boxed{V_0=e^{a(c-d)}\Phi\left(\frac{dT-a}{\sqrt T}\right)+e^{a(c+d)}\Phi\left(\frac{-a-dT}{\sqrt T}\right).}
$$

This formula also covers $d=0$ and negative rates. When $r\geq0$, one may use $d=(r+\sigma^2/2)/\sigma$, so the two prefactors simplify to $e^{-\sigma a}$ and $e^{2ra/\sigma}$. At $r=0$ the expression is the undiscounted hitting probability, as a consistency check.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
