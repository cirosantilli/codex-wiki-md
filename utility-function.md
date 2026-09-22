# Utility function

↑ **Parent:** [Mathematical finance](mathematical-finance.md)

In expected-utility portfolio choice, an increasing utility function prefers greater wealth, while concavity models aversion to risk.

A [utility function](utility-function.md) assigns numerical values to outcomes consistently with preference comparisons. It represents [utility](mathematics.md#utility); the representation and the preference concept are distinct.

**Table of contents**

- [Risk seeking](#risk-seeking)
- [Risk aversion](#risk-aversion)
  - [Relative risk aversion coefficient](#relative-risk-aversion-coefficient)
    - [Small multiplicative risk premium](#small-multiplicative-risk-premium)
- [Marginal utility](#marginal-utility)
- [Expected utility](#expected-utility)
  - [Risk premium](#risk-premium)
- [Affine utility on probability measures](#affine-utility-on-probability-measures)
  - [Expected utility representation on a finite measurable space](#expected-utility-representation-on-a-finite-measurable-space)
  - [Positive affine uniqueness of affine preference representations](#positive-affine-uniqueness-of-affine-preference-representations)
  - [Mixture solvability of affine preferences](#mixture-solvability-of-affine-preferences)
  - [Independence axiom for lottery preferences](#independence-axiom-for-lottery-preferences)
- [Inverse marginal utility](#inverse-marginal-utility)
- [Multiplicative habit utility](#multiplicative-habit-utility)
  - [Dual equation for multiplicative habit investment](#dual-equation-for-multiplicative-habit-investment)
  - [Effective consumption shadow price with habit](#effective-consumption-shadow-price-with-habit)
  - [Exponentially weighted consumption habit](#exponentially-weighted-consumption-habit)
- [Inada conditions](#inada-conditions)
  - [Inada utility with vanishing curvature](#inada-utility-with-vanishing-curvature)
- [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)
  - [Power-wealth investment with running utility](#power-wealth-investment-with-running-utility)
  - [Benchmark-relative power-utility portfolio](#benchmark-relative-power-utility-portfolio)
  - [Square-root investment-consumption value](#square-root-investment-consumption-value)
  - [Logarithmic utility](#logarithmic-utility)
    - [Two-state logarithmic portfolio with a borrowing constraint](#two-state-logarithmic-portfolio-with-a-borrowing-constraint)
    - [Log-optimal investment with Gaussian drift learning](#log-optimal-investment-with-gaussian-drift-learning)
  - [Volatility-penalized terminal fee](#volatility-penalized-terminal-fee)
  - [Risk aversion recovered from an optimal two-state payoff](#risk-aversion-recovered-from-an-optimal-two-state-payoff)
- [Quasilinear utility](#quasilinear-utility)
- [Risk neutrality](#risk-neutrality)
- [Constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility)
  - [Binomial exponential-utility terminal wealth](#binomial-exponential-utility-terminal-wealth)
  - [Finite-horizon exponential-utility portfolio](#finite-horizon-exponential-utility-portfolio)
  - [Exponential-utility risk sharing](#exponential-utility-risk-sharing)
  - [Exponential-utility portfolio with nonnegative cash](#exponential-utility-portfolio-with-nonnegative-cash)
- [Expected utility hypothesis](#expected-utility-hypothesis)
  - [Expected utility maximization](#expected-utility-maximization)
    - [Unbounded linear terminal-wealth utility](#unbounded-linear-terminal-wealth-utility)
    - [Complete-market terminal utility optimizer](#complete-market-terminal-utility-optimizer)
      - [Binomial power-utility terminal wealth](#binomial-power-utility-terminal-wealth)
    - [Proportional transaction cost](#proportional-transaction-cost)
    - [Secant domination for expected utility derivatives](#secant-domination-for-expected-utility-derivatives)
    - [Terminal wealth floor](#terminal-wealth-floor)
      - [Floored marginal utility optimizer](#floored-marginal-utility-optimizer)
    - [Discounted infinite-horizon utility integrability](#discounted-infinite-horizon-utility-integrability)
    - [Hedge fund incentive utility](#hedge-fund-incentive-utility)
      - [Concavification of incentive utility](#concavification-of-incentive-utility)
        - [Fair-game gambling induced by an incentive fee](#fair-game-gambling-induced-by-an-incentive-fee)
        - [Common tangent for exponential incentive utility](#common-tangent-for-exponential-incentive-utility)
    - [Investment-consumption problem](#investment-consumption-problem)
      - [Finite-horizon power-utility investment and consumption](#finite-horizon-power-utility-investment-and-consumption)
      - [Finite-horizon logarithmic investment and consumption](#finite-horizon-logarithmic-investment-and-consumption)
      - [Investment with fixed debt service](#investment-with-fixed-debt-service)
        - [Dual ruin boundary with debt service](#dual-ruin-boundary-with-debt-service)
      - [Constant market price of risk investment](#constant-market-price-of-risk-investment)
      - [Consumption satisfaction stock](#consumption-satisfaction-stock)
        - [Singular consumption control](#singular-consumption-control)
        - [Gradient constraint for unbounded consumption](#gradient-constraint-for-unbounded-consumption)
        - [Wealth-to-satisfaction reduction](#wealth-to-satisfaction-reduction)
      - [Investment value transversality condition](#investment-value-transversality-condition)
      - [State-dependent correlation investment problem](#state-dependent-correlation-investment-problem)
        - [Power transformation of a complete-market investment equation](#power-transformation-of-a-complete-market-investment-equation)
      - [Intertemporal hedging demand](#intertemporal-hedging-demand)
        - [Learning hedge in a binary-drift investment model](#learning-hedge-in-a-binary-drift-investment-model)
      - [High-water mark investment taxation](#high-water-mark-investment-taxation)
        - [Wealth-cap investment boundary](#wealth-cap-investment-boundary)
        - [High-water mark tax boundary condition](#high-water-mark-tax-boundary-condition)
      - [Merton consumption-investment problem](#merton-consumption-investment-problem)
        - [Regime-switching Merton equations](#regime-switching-merton-equations)
        - [Retirement boundary with an income option](#retirement-boundary-with-an-income-option)
        - [Merton consumption constant](#merton-consumption-constant)
        - [Maximal squared Sharpe ratio value bound](#maximal-squared-sharpe-ratio-value-bound)
        - [Exponential interest-rate switch](#exponential-interest-rate-switch)
    - [Certainty equivalent](#certainty-equivalent)
    - [Expected utility of a Gaussian location-scale family](#expected-utility-of-a-gaussian-location-scale-family)
    - [Indifference price](#indifference-price)
      - [Periodic utility indifference payment for Gaussian income](#periodic-utility-indifference-payment-for-gaussian-income)
    - [Optimized affine shift of concave utility](#optimized-affine-shift-of-concave-utility)
    - [Scaled centered risk under concave utility](#scaled-centered-risk-under-concave-utility)
    - [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)
      - [Logarithmic terminal wealth in a complete market](#logarithmic-terminal-wealth-in-a-complete-market)
      - [Optimal marginal utility as a one-period pricing density](#optimal-marginal-utility-as-a-one-period-pricing-density)
        - [Marginal utility price](#marginal-utility-price)
        - [Marginal utility pricing with proportional transaction costs](#marginal-utility-pricing-with-proportional-transaction-costs)
      - [One-period marginal-utility certificate of optimality](#one-period-marginal-utility-certificate-of-optimality)
      - [Marginal-utility verification of optimal consumption](#marginal-utility-verification-of-optimal-consumption)
      - [Wealth-variable Legendre dual](#wealth-variable-legendre-dual)

## Risk seeking

↑ **Parent:** [Utility function](utility-function.md)

An increasing convex [utility function](utility-function.md) prefers a nondegenerate lottery to its sure mean by the [Jensen inequality](real-analysis.md#jensen-s-inequality). Its [relative risk aversion coefficient](#relative-risk-aversion-coefficient) is negative when its second derivative is strictly positive. This differs from [risk neutrality](#risk-neutrality), which corresponds to affine utility.

## Risk aversion

↑ **Parent:** [Utility function](utility-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Risk_aversion)

For increasing [expected utility](#expected-utility) preferences, an investor is risk-averse when a sure mean is at least as desirable as the corresponding lottery. A concave [utility function](utility-function.md) gives this preference by the [Jensen inequality](real-analysis.md#jensen-s-inequality); a strictly concave utility gives strict preference for nondegenerate risks. Local risk aversion is measured by $-U''/U'$ and its relative counterpart $-WU''/U'$.

### Relative risk aversion coefficient

↑ **Parent:** [Risk aversion](#risk-aversion)

For positive wealth and increasing twice differentiable [utility function](utility-function.md), this dimensionless coefficient measures sensitivity to proportional wealth risk. If it is constant, integration gives $U'(W)=cW^{-\alpha}$ with $c>0$, and hence $U(W)=cW^{1-\alpha}/(1-\alpha)+d$ for $\alpha\ne1$ or $c\log W+d$ for $\alpha=1$. Positive, zero and negative coefficients correspond respectively to [risk aversion](#risk-aversion), [risk neutrality](#risk-neutrality) and [risk seeking](#risk-seeking). The usual [CRRA utility](#constant-relative-risk-aversion-utility) subclass takes $\alpha>0$.

#### Small multiplicative risk premium

↑ **Parent:** [Relative risk aversion coefficient](#relative-risk-aversion-coefficient)

Compare expected utility of $W(1+\phi)$, where $\mathbb E\phi=0$, with the certainty equivalent $W(1-\psi)$. A second-order [Taylor expansion](calculus.md#taylor-expansion) gives $U(W)+W^2U''(W)\mathbb E\phi^2/2$ for the risky side and $U(W)-WU'(W)\psi$ for the sure side. Equality gives the displayed proportional [risk premium](#risk-premium). This requires a genuinely small-shock family with controlled remainders; small variance alone does not control rare large wealth shocks.

## Marginal utility

↑ **Parent:** [Utility function](utility-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Marginal_utility)

The additional [utility function](utility-function.md) obtained per additional unit of [consumption](mathematical-finance.md#consumption) or [portfolio wealth](mathematical-finance.md#portfolio-wealth). For a differentiable [utility function](utility-function.md) it is its [derivative](calculus.md#derivative); for a [concave](real-analysis.md#concave-function) [utility function](utility-function.md) it is nonincreasing. In a complete-market allocation, equating marginal utility to a multiplier times the [state-price density](mathematical-finance.md#state-price-density) compares the utility benefit of a payoff with its financing cost. The [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality) makes this comparison a global optimality certificate rather than only a local first-order condition.

## Expected utility

↑ **Parent:** [Utility function](utility-function.md)

The [expected value](probability-theory.md#expected-value) of the [utility function](utility-function.md) applied to a random outcome, using the decision-maker's probabilities. For a finite lottery it is $\sum_xp(x)u(x)$. Under [risk neutrality](#risk-neutrality) and [quasilinear utility](#quasilinear-utility), auction utility is valuation minus payment upon winning and zero upon losing, so its expectation is the winning probability times the payoff conditional on winning.

### Risk premium

↑ **Parent:** [Expected utility](#expected-utility)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Risk_premium)

In [expected utility](#expected-utility) theory, the risk premium is the difference between expected wealth and its certainty equivalent: $U(\operatorname{CE}(W))=\mathbb E U(W)$. For increasing concave [utility functions](utility-function.md) it is nonnegative by the [Jensen inequality](real-analysis.md#jensen-s-inequality). In financial asset pricing, risk premium also refers to expected return above a specified risk-free benchmark; the benchmark and whether the premium is monetary or proportional must therefore be stated.

## Affine utility on probability measures

↑ **Parent:** [Utility function](utility-function.md)

An [affine utility on probability measures](#affine-utility-on-probability-measures) functional satisfies $U_0(p\lambda+(1-p)\mu)=pU_0(\lambda)+(1-p)U_0(\mu)$ on mixtures of [probability measures](probability-theory.md#probability-measure). Strict preferences are represented by comparing its real values, and indifference means equal values. This is cardinal utility on lotteries rather than merely an ordinal ordering of deterministic outcomes.

### Expected utility representation on a finite measurable space

↑ **Parent:** [Affine utility on probability measures](#affine-utility-on-probability-measures)

Set $U(x)=U_0(\delta_x)$. On a finite measurable space, points in the same [atom of a sigma-algebra](measure-theory.md#atom-of-a-sigma-algebra) give the same [Dirac measure](measure-theory.md#dirac-measure), so $U$ is a [measurable function](measure-theory.md#measurable-function) and constant on atoms. Every [probability measure](probability-theory.md#probability-measure) is a finite mixture of representative [Dirac measures](measure-theory.md#dirac-measure) with its atom masses as weights. Affineness then proves the expected-utility representation, even when the [sigma-algebra](measure-theory.md#sigma-algebra) is smaller than the [power set](set.md#power-set).

### Positive affine uniqueness of affine preference representations

↑ **Parent:** [Affine utility on probability measures](#affine-utility-on-probability-measures)

Two real affine functionals on a [convex set](mathematical-optimization.md#convex-set) of lotteries that represent the same strict preferences differ by $V=aU+b$ with $a>0$. Equal utility values must first be shown to give equal values of the other functional. The induced function on the [real interval](real-analysis.md#interval-mathematics) of utility values preserves mixtures; anchor interpolation, including exterior points represented through an anchor, makes it linear throughout. Constant representations are handled separately and still admit a positive slope.

### Mixture solvability of affine preferences

↑ **Parent:** [Affine utility on probability measures](#affine-utility-on-probability-measures)

For three strictly ordered affine-utility values $u>v>w$, the middle lottery is indifferent to the mixture of the extreme lotteries with weight $p=(v-w)/(u-w)$ on the best one. This weight lies strictly between zero and one. It is the exact mixture-indifference property underlying cardinal utility comparisons.

### Independence axiom for lottery preferences

↑ **Parent:** [Affine utility on probability measures](#affine-utility-on-probability-measures)

Mixing two lotteries with the same third lottery and the same positive weight preserves their strict preference order. For [affine utility on probability measures](#affine-utility-on-probability-measures), the difference of the two mixed utilities is the original difference multiplied by that weight. At weight zero the strict preference disappears, so positivity is essential.

## Inverse marginal utility

↑ **Parent:** [Utility function](utility-function.md)

For an increasing differentiable strictly [concave](real-analysis.md#concave-function) [utility function](utility-function.md) satisfying the [Inada conditions](#inada-conditions), the inverse marginal utility maps each positive shadow price to the unique positive payoff with that marginal utility. For normalized [CRRA utility](#constant-relative-risk-aversion-utility), $I(y)=y^{-1/R}$.

## Multiplicative habit utility

↑ **Parent:** [Utility function](utility-function.md)

Multiplicative habit utility modifies current consumption utility through its ratio to habit $h>0$. With $U(c)=c^{1-R}/(1-R)$, $R>1$, and $\alpha>0$, it is $h^\alpha c^{1-R-\alpha}/(1-R)$. Its [homogeneity](real-analysis.md#homogeneity) in $(c,h)$ has degree $1-R$, while consumption holding habit fixed has effective relative risk aversion $R+\alpha$.

### Dual equation for multiplicative habit investment

↑ **Parent:** [Multiplicative habit utility](#multiplicative-habit-utility)

After scaling wealth by habit and applying the [wealth-variable Legendre dual](#wealth-variable-legendre-dual), the effective consumption shadow price is proportional to $\mathcal D=z-\lambda RzJ^\prime+\lambda(R-1)J$. Its power in the utility conjugate keeps the dual equation nonlinear. When $\lambda=0$, habit is fixed and the dual equation is a linear [Euler differential equation](differential-equation.md#cauchy-euler-equation) with effective relative risk aversion $R+\alpha$.

### Effective consumption shadow price with habit

↑ **Parent:** [Multiplicative habit utility](#multiplicative-habit-utility)

When habit evolves by $dh=\lambda(c-h)dt$, increasing consumption both costs wealth and increases future habit. Consequently the consumption coefficient in the [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) is $V_w-\lambda V_h$. A finite interior optimum requires this effective shadow price to be positive.

### Exponentially weighted consumption habit

↑ **Parent:** [Multiplicative habit utility](#multiplicative-habit-utility)

An exponentially weighted consumption habit is $h_t=e^{-\lambda t}h_0+\int_0^t\lambda e^{-\lambda(t-s)}c_sds$. Differentiation gives $dh_t=\lambda(c_t-h_t)dt$. The state remains positive from positive initial habit and nonnegative consumption.

## Inada conditions

↑ **Parent:** [Utility function](utility-function.md)

The Inada conditions specify infinite marginal utility at zero consumption or wealth and zero marginal utility at infinity. For an increasing strictly [concave](real-analysis.md#concave-function) [utility function](utility-function.md), they make the inverse marginal utility map cover all positive shadow prices, facilitating the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) method.

### Inada utility with vanishing curvature

↑ **Parent:** [Inada conditions](#inada-conditions)

This smooth utility has $U'(x)=x^{-1}-x^{-2}+x^{-3}/3>0$ and $U''(x)=-(x-1)^2/x^4$. Its [derivative](calculus.md#derivative) is strictly decreasing, diverges at zero and tends to zero at infinity, so the utility is [strictly concave](real-analysis.md#strictly-concave-function) and satisfies the [Inada conditions](#inada-conditions). Yet its curvature vanishes at one. The [inverse marginal utility](#inverse-marginal-utility) cannot have a finite [derivative](calculus.md#derivative) at $y=1/3$, since differentiating $U'(I(y))=y$ there would give zero equal to one. Its dual is differentiable but not twice differentiable at that price.

## Constant relative risk aversion utility

↑ **Parent:** [Utility function](utility-function.md)

A constant relative risk aversion utility has $-cU^{\prime\prime}(c)/U^\prime(c)=R>0$. Up to a positive scale and an additive constant, it is $U(c)=c^{1-R}/(1-R)$ for $R\ne1$ and $U(c)=\log c$ for $R=1$. Power utility gives multiplicative [homogeneity](real-analysis.md#homogeneity) of an investment value; logarithmic utility gives additive scaling.

### Power-wealth investment with running utility

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

For a [self-financing portfolio](mathematical-finance.md#self-financing-portfolio) earning both running reward $e^{-\rho t}W^\gamma$ and terminal reward $W_T^\gamma$, $0<\gamma<1$, with no consumption withdrawals, [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) gives $J(W,t)=A(t)W^\gamma$ and the displayed constant risky fraction. The coefficient satisfies $A'+\kappa A+e^{-\rho t}=0$, $A(T)=1$, where $\kappa=\gamma r+\gamma(\mu-r)^2/(2(1-\gamma)\sigma^2)$. Its positive solution is $e^{\kappa(T-t)}+\int_t^T e^{\kappa(s-t)-\rho s}ds$. Risk aversion is $1-\gamma$; increasing $\gamma$ raises risky investment and can require borrowing.

### Benchmark-relative power-utility portfolio

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

In a Brownian [complete market](mathematical-finance.md#complete-market) with constant coefficients and nonsingular $\sigma$, maximize expected [CRRA utility](#constant-relative-risk-aversion-utility) of terminal [portfolio wealth](mathematical-finance.md#portfolio-wealth) divided by a [geometric stock index](mathematical-finance.md#geometric-stock-index). Writing $p=1/R$ and $q=n^{-1}\mathbf1$, the pointwise marginal condition gives $w_T^*=\lambda^{-p}\zeta_T^{-p}J_T^{1-p}$. Its [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) determines $\lambda^{-p}=w_0/\mathbb E[(\zeta_TJ_T)^{1-p}]$. Conditional lognormal moments and replication then give the displayed constant dollar fractions. The first term is ordinary optimal risk exposure; the second hedges the random benchmark. The bank holds the remaining fraction, which can be negative when borrowing is allowed.

### Square-root investment-consumption value

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

For zero cash interest, constant excess drift $\mu$, volatility $\sigma$, and both terminal and consumption utility $2\sqrt{x}$, set $A=\sigma\sigma^T$ and assume $\mu$ belongs to the [image of a linear map](vector-space.md#image-of-a-linear-map) $A$. Let $A^+$ be the [Moore-Penrose inverse](linear-algebra.md#moore-penrose-inverse) and $q=\mu^T A^+\mu$. Then $h'+qh+1=0$, $h(T)=1$, so $h(t)=e^{q(T-t)}+(e^{q(T-t)}-1)/q$ for $q>0$, and $h(t)=1+T-t$ for $q=0$. The [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) has the displayed solution. Maximizing dollar investment and consumption are $\theta_t=2X_t A^+\mu$ and $C_t=X_t/h(t)$. The resulting positive [portfolio wealth](mathematical-finance.md#portfolio-wealth) is a [geometric Brownian motion](stochastic-calculus.md#geometric-brownian-motion) with a deterministic time-dependent drift, and finite-horizon moment bounds justify equality in verification.

### Logarithmic utility

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

[Logarithmic utility](#logarithmic-utility) on positive [portfolio wealth](mathematical-finance.md#portfolio-wealth) has [derivative](calculus.md#derivative) $1/x$ and relative risk aversion one. Its [utility conjugate](convex-optimization.md#utility-conjugate) is $V(y)=-\log y-1$, since the maximizing wealth is $1/y$. It satisfies the [Inada conditions](#inada-conditions).

#### Two-state logarithmic portfolio with a borrowing constraint

↑ **Parent:** [Logarithmic utility](#logarithmic-utility)

Let a [portfolio](mathematical-finance.md#investment-portfolio) hold $x\in[0,T]$ in a [risk-free asset](mathematical-finance.md#risk-free-asset) with net return $r$ and $T-x$ in an asset returning $g$ or $b$, with probabilities $p$ and $1-p$. Assume $T>0$, $-1<b<r<g$, $0<p<1$, and $pg+(1-p)b>r$. Its state wealths are $w_g=T(1+g)-(g-r)x$ and $w_b=T(1+b)+(r-b)x$. The [expected utility](#expected-utility) $p\log w_g+(1-p)\log w_b$ has strictly negative second [derivative](calculus.md#derivative). Setting its first [derivative](calculus.md#derivative) to zero gives the displayed unconstrained root; the [derivative](calculus.md#derivative) at $x=T$ is negative, so only the lower constraint can bind. Thus the displayed formula is the unique optimum. All equity is optimal exactly when $p\ge (r-b)(1+g)/[(g-b)(1+r)]$. The positivity of both state wealths is part of the [logarithmic utility](#logarithmic-utility) domain.

#### Log-optimal investment with Gaussian drift learning

↑ **Parent:** [Logarithmic utility](#logarithmic-utility)

For a [stock](mathematical-finance.md#stock) with observed dynamics $dS_t/S_t=\sigma d\widehat W_t+\sigma m_tdt$ and constant riskless [interest rate](mathematical-finance.md#interest-rate) $r$, the [finite-horizon pricing density for Gaussian drift learning](time-series.md#finite-horizon-pricing-density-for-gaussian-drift-learning) with $k=r/\sigma$ gives $\zeta_t=e^{-rt}D_t$. The terminal [logarithmic utility](#logarithmic-utility) condition $1/w_T^*=\lambda\zeta_T$ and the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) give $\lambda=1/w_0$. Replication then gives $w_t^*=w_0/\zeta_t$ at every time. The [Itô formula](stochastic-calculus.md#ito-s-lemma) for $1/\zeta$ makes the optimal dollar stock fraction $(m_t-r/\sigma)/\sigma$. Its finite expected log return follows from finite posterior second moments on finite horizons.

### Volatility-penalized terminal fee

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

A fee proportional to terminal [portfolio wealth](mathematical-finance.md#portfolio-wealth) but reduced by accumulated portfolio [quadratic variation](stochastic-calculus.md#quadratic-variation) changes the optimal risk exposure of a manager with [constant relative risk aversion utility](#constant-relative-risk-aversion-utility). Write $A=\sigma\sigma^T$, $b=\mu-r\mathbf1$ and assume $A$ is invertible. The fee process has drift $r+b^T\pi-\varepsilon\pi^TA\pi/2$ and volatility $\sigma^T\pi$. Its [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) therefore maximizes $b^T\pi-(R+\varepsilon)\pi^TA\pi/2$, giving $\pi^*=A^{-1}b/(R+\varepsilon)$. The fee increases effective relative risk aversion from $R$ to $R+\varepsilon$, independently of its positive scale $a$.

There is also a direct global bound. Put $p=1-R$, $v^*=\sigma^T\pi^*$, and tilt probability by $\exp(pv^*\cdot W_T-p^2|v^*|^2T/2)$. Under this probability let $Z$ be the [stochastic exponential](stochastic-calculus.md#doleans-dade-exponential) of $(1+\varepsilon)\int(\sigma^T\pi-v^*)\cdot dW^*$. The terminal fee ratio satisfies $(y_T/y_T^*)^p=Z_T^{p/(1+\varepsilon)}$. A nonnegative [local martingale](martingale.md#local-martingale) has expectation at most one. The [Jensen inequality](real-analysis.md#jensen-s-inequality), applied to a concave positive power when $p>0$ and a convex negative power when $p<0$, proves that the constant exposure maximizes expected [CRRA utility](#constant-relative-risk-aversion-utility). Effective risk aversion one uses logarithmic utility.

### Risk aversion recovered from an optimal two-state payoff

↑ **Parent:** [Constant relative risk aversion utility](#constant-relative-risk-aversion-utility)

For an interior optimal payoff in a complete two-state market under [CRRA utility](#constant-relative-risk-aversion-utility), $W_u^{-R}/W_d^{-R}=Z_u/Z_d$. If the two positive payoffs differ, taking logarithms gives the displayed coefficient. The multiplier can then be recovered from either state. A positive coefficient requires the price-density and payoff orders to be compatible with decreasing marginal utility.

## Quasilinear utility

↑ **Parent:** [Utility function](utility-function.md)

This utility is linear in the monetary transfer: allocation value minus payment. It supports the incentive comparisons and payment identities used in [mechanism design](game-theory.md#mechanism-design).

## Risk neutrality

↑ **Parent:** [Utility function](utility-function.md)

Risk neutrality means evaluating uncertain monetary gains by their expected value. For auction payment identities, [quasilinear utility](#quasilinear-utility) gives a bidder's expected utility as its value times its winning probability minus expected payment.

## Constant absolute risk aversion utility

↑ **Parent:** [Utility function](utility-function.md)

Constant absolute risk aversion utility has $-U''(x)/U'(x)=\gamma>0$. For Gaussian wealth $W$, maximizing $\mathbb E[-e^{-\gamma W}]$ is equivalent to maximizing

$$
\mathbb EW-\frac{\gamma}{2}\operatorname{Var}(W).
$$

### Binomial exponential-utility terminal wealth

↑ **Parent:** [Constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility)

For unrestricted final [portfolio wealth](mathematical-finance.md#portfolio-wealth) in an $n$-period [binomial market](mathematical-finance.md#discrete-time-binomial-market), write $R$ for the bank growth factor, $a>0$ for absolute risk aversion, and $Z=dQ/dP$ for the [binomial-market probability density](mathematical-finance.md#binomial-market-probability-density). The displayed optimizer has the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) $\mathbb E_QH^*=R^nw_0$. Its [exponential utility](#constant-absolute-risk-aversion-utility) derivative satisfies $e^{-aH^*}=\lambda Z$ for a constant $\lambda>0$. The [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality) bounds any competing [expected utility](#expected-utility) by this value, because the expected linear error is $\lambda\mathbb E_Q(H-H^*)=0$. Strict [concavity](real-analysis.md#concave-function) proves uniqueness, and [market completeness](mathematical-finance.md#complete-market) supplies replication. The formula is altered by a constraint requiring nonnegative final wealth. With physical up probability $p$ and [risk-neutral probability](mathematical-finance.md#risk-neutral-probability) $q$, $\mathbb E_Q\log Z=n[q\log(q/p)+(1-q)\log((1-q)/(1-p))]$.

### Finite-horizon exponential-utility portfolio

↑ **Parent:** [Constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility)

For [exponential utility](#constant-absolute-risk-aversion-utility) $(1-e^{-ax})/a$ on unrestricted terminal [portfolio wealth](mathematical-finance.md#portfolio-wealth) in the [Black-Scholes model](mathematical-finance.md#black-scholes-model), the optimal dollar holding in the [stock](mathematical-finance.md#stock) is the displayed deterministic amount. Set $\vartheta=(\mu-\rho)/\sigma$ and let $W^Q=W+\vartheta t$ be the [Brownian motion](brownian-motion.md) under the [risk-neutral measure](mathematical-finance.md#risk-neutral-measure). The terminal optimizer is $X^*=w_0e^{\rho T}+\vartheta W_T^Q/a$. Its [marginal utility](#marginal-utility) is proportional to the [state-price density](mathematical-finance.md#state-price-density), and the [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality) proves global optimality under the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint). The [expected utility](#expected-utility) at the optimum is $(1-\exp(-aw_0e^{\rho T}-\vartheta^2T/2))/a$. A nonnegative-wealth constraint changes this optimizer.

### Exponential-utility risk sharing

↑ **Parent:** [Constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility)

With positive welfare weights $a_j$, maximize $\sum_ja_j\beta_j^t[-e^{-\gamma_jc_j}/\gamma_j]$ subject to $\sum_jc_j=d$. Interior [first-order conditions](mathematical-optimization.md#first-order-optimality-condition) give $a_j\beta_j^te^{-\gamma_jc_j}=\nu$. Put $\Gamma=(\sum_j\gamma_j^{-1})^{-1}$, $\log\bar\beta=\Gamma\sum_j\gamma_j^{-1}\log\beta_j$ and $\log A=\Gamma\sum_j\gamma_j^{-1}\log a_j$. Then

$$
\nu=A\bar\beta^te^{-\Gamma d},\qquad
c_j=\frac\Gamma{\gamma_j}d+\frac{t}{\gamma_j}(\log\beta_j-\log\bar\beta)+\frac1{\gamma_j}(\log a_j-\log A).
$$

If [consumption](mathematical-finance.md#consumption) must be nonnegative, the interior formula is replaced by $c_j=\max\{0,(\log a_j+t\log\beta_j-\log\nu)/\gamma_j\}$, with $\nu$ determined by resource clearing. These are Pareto allocations; realizing them as a [competitive equilibrium with one productive asset](mathematical-finance.md#competitive-equilibrium-with-one-productive-asset) requires feasible financing. For common $\beta_j=\beta$ and initial ownership $\Gamma/\gamma_j$, constant holdings and $C_t^j=(\Gamma/\gamma_j)d_t$ give such an equilibrium whenever fundamental prices and the utility sums are finite.

### Exponential-utility portfolio with nonnegative cash

↑ **Parent:** [Constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility)

For Gaussian terminal prices with positive definite covariance $V$, set $M=(\gamma V)^{-1}$ and $\eta=(S_0^TM\mu-w_0)/(S_0^TMS_0)$, assuming $S_0\ne0$. The normal moment-generating function turns expected exponential utility into a strictly concave mean-minus-variance objective. Its free optimum has cash $S_0^TMS_0(1+r-\eta)$. If this is positive, keep the free optimum; otherwise the cash constraint binds and the multiplier becomes $\eta$. Thus zero optimal cash is equivalent to $\eta\geq1+r$, including equality.

## Expected utility hypothesis

↑ **Parent:** [Utility function](utility-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Expected_utility_hypothesis)

The [expected utility hypothesis](#expected-utility-hypothesis) ranks uncertain outcomes by the [expected value](probability-theory.md#expected-value) of a [utility function](utility-function.md). When these preference assumptions hold, [expected utility maximization](#expected-utility-maximization) selects an admissible outcome with greatest expected utility.

### Expected utility maximization

↑ **Parent:** [Expected utility hypothesis](#expected-utility-hypothesis)

Expected utility maximization chooses an admissible random payoff $X$ to maximize $\mathbb E[U(X)]$.

#### Unbounded linear terminal-wealth utility

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

If a positive terminal [state-price density](mathematical-finance.md#state-price-density) has essential infimum zero, let $A_n=\{\zeta_T<1/n\}$ and $X_n=w_0\mathbf1_{A_n}/\mathbb E[\zeta_T\mathbf1_{A_n}]$. Whenever $\mathbb P(A_n)>0$, these claims cost $w_0$ and satisfy $\mathbb EX_n>nw_0$. In a Brownian [complete market](mathematical-finance.md#complete-market) with constant nonzero [market price of risk](mathematical-finance.md#market-price-of-risk), $\zeta_T$ has a [lognormal distribution](probability-theory.md#log-normal-distribution) and all these events have positive probability. Thus bounded market coefficients and an increasing [concave](real-analysis.md#concave-function) utility do not alone ensure a finite attained optimum: the linear utility $U(x)=x$ already fails. Usual inverse-marginal-utility formulas require further utility and integrability hypotheses.

#### Complete-market terminal utility optimizer

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

For an increasing strictly concave [utility function](utility-function.md) satisfying the [Inada conditions](#inada-conditions), put $I=(U')^{-1}$ and let $\zeta$ be the positive terminal [state-price density](mathematical-finance.md#state-price-density). In a finite complete market, select $y>0$ so that $\mathbb E[\zeta I(y\zeta)]$ equals initial wealth. The displayed payoff is optimal under that budget: the supporting-line inequality for utility has marginal slope $y\zeta$, and its expected linear error vanishes on the budget constraint. [Market completeness](mathematical-finance.md#complete-market) supplies its replicating strategy.

##### Binomial power-utility terminal wealth

↑ **Parent:** [Complete-market terminal utility optimizer](#complete-market-terminal-utility-optimizer)

In a complete $n$-period [binomial market](mathematical-finance.md#discrete-time-binomial-market) with riskless gross return $R$, pricing density $Z$ and [utility function](utility-function.md) $U(x)=\gamma x^{1/\gamma}$, put $\eta=\gamma/(\gamma-1)$. The optimal terminal payoff is $X^*=R^nw_0Z^{-\eta}/\mathbb E[Z^{1-\eta}]$. Its marginal utility is proportional to $Z$; the supporting-line inequality for the strictly concave [utility function](utility-function.md) proves optimality using the pricing [budget constraint](mathematical-finance.md#budget-constraint).

#### Proportional transaction cost

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

A holding-dependent cost proportional to the absolute position size. In a one-period gain objective it changes the sample payoff to $\theta X-\varepsilon|\theta|$, giving gain parameter $X-\varepsilon$ for positive holdings and $X+\varepsilon$ for negative holdings. The objective is concave but can have a kink at zero.

#### Secant domination for expected utility derivatives

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

If a negative differentiable concave [utility function](utility-function.md) satisfies $\mathbb EU(\theta X)>-\infty$ on an open interval, outer secants at four points bound the sample derivative on a smaller compact interval. Negativity makes the endpoint values absolutely integrable. The [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) then gives $d\mathbb EU(\theta X)/d\theta=\mathbb E[XU'(\theta X)]$ and continuous derivative when $U'$ is continuous. This is a justification of differentiation, rather than an assumption of [integrability](measure-theory.md#integrability) of marginal utility.

#### Terminal wealth floor

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

A terminal [portfolio wealth](mathematical-finance.md#portfolio-wealth) floor is a prescribed lower bound, possibly a [random variable](random-variable.md), on terminal portfolio [portfolio wealth](mathematical-finance.md#portfolio-wealth). In a [complete market](mathematical-finance.md#complete-market), its [state-price density](mathematical-finance.md#state-price-density) cost cannot exceed initial [portfolio wealth](mathematical-finance.md#portfolio-wealth). Nonnegative admissibility replaces a possibly negative floor by its positive part.

##### Floored marginal utility optimizer

↑ **Parent:** [Terminal wealth floor](#terminal-wealth-floor)

For a nonnegative [terminal wealth floor](#terminal-wealth-floor) whose [state-price density](mathematical-finance.md#state-price-density) cost is strictly below the available budget, pointwise maximization of $U(y)-\lambda\zeta_Ty$ over $y\geq\xi$ gives the displayed payoff. The positive multiplier exhausts the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint). This requires the usual utility and integrability hypotheses ensuring that the multiplier exists and the payoff is replicable.

#### Discounted infinite-horizon utility integrability

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

Finite lower and upper utility bounds together with a positive discount rate bound the absolute time integral by $\max(|L|,|R|)/b$. This justifies [expectation](probability-theory.md#expected-value) and integration in marginal-utility verification. Bounded utility alone on an undiscounted infinite horizon does not prevent both positive and negative parts from having infinite integral.

#### Hedge fund incentive utility

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

An incentive fee above a hurdle changes a manager’s [utility function](utility-function.md) into $F(y)=U(\varepsilon y+\alpha(y-w_0)_+)$. For [constant absolute risk aversion utility](#constant-absolute-risk-aversion-utility), each branch is strictly [concave](real-analysis.md#concave-function), but the marginal reward jumps upward at the hurdle. Thus the effective terminal-wealth utility is not concave, and [concavification of incentive utility](#concavification-of-incentive-utility) can reveal optimal risk-taking lotteries.

##### Concavification of incentive utility

↑ **Parent:** [Hedge fund incentive utility](#hedge-fund-incentive-utility)

Concavification replaces a nonconcave incentive [utility function](utility-function.md) by its least [concave majorant](real-analysis.md#concave-majorant). In a [complete market](mathematical-finance.md#complete-market) with an atomless [state-price density](mathematical-finance.md#state-price-density), the optimizing payoff may avoid all intervals where the majorant strictly exceeds the original utility, making the relaxed optimum exactly attainable. At a pricing atom corresponding to a linear segment, a lottery between contact points can attain the same value at unchanged cost.

###### Fair-game gambling induced by an incentive fee

↑ **Parent:** [Concavification of incentive utility](#concavification-of-incentive-utility)

With zero interest and zero risk premium, a manager whose current wealth lies between common-tangent contacts $\ell,h$ can improve [expected utility maximization](#expected-utility-maximization) through a fair lottery paying those two values. The probability of $h$ is $(w_0-\ell)/(h-\ell)$. In a [Brownian filtration](brownian-motion.md#brownian-filtration), replicating a bounded terminal lottery gives a nonnegative wealth [martingale](martingale.md) throughout.

###### Common tangent for exponential incentive utility

↑ **Parent:** [Concavification of incentive utility](#concavification-of-incentive-utility)

For $F(y)=-e^{-ay}$ below hurdle $w_0$ and $F(y)=-e^{(b-a)w_0-by}$ above it, with $b>a>0$, an interior common tangent touches at $\ell=w_0-[b/a-1-\log(b/a)]/(b-a)$ and $h=w_0+[\log(b/a)-1+a/b]/(b-a)$. The slope is $ae^{-a\ell}$ and $h-\ell=1/a-1/b$. The formula requires $\ell\geq0$; a smaller hurdle gives a different endpoint-at-zero concavification.

#### Investment-consumption problem

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

An investment-consumption problem chooses portfolio holdings and consumption to maximize discounted [expected utility maximization](#expected-utility-maximization) subject to a [self-financing portfolio](mathematical-finance.md#self-financing-portfolio) wealth equation and admissibility constraints. A [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) or [utility duality with martingale deflators](#utility-duality-with-martingale-deflators) characterizes the optimum when the value is finite.

##### Finite-horizon power-utility investment and consumption

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

For [constant relative risk aversion utility](#constant-relative-risk-aversion-utility) with parameter $\gamma>0$, terminal weight $\eta>0$ and utility discount rate $\delta$, in a [Black-Scholes model](mathematical-finance.md#black-scholes-model) put $\lambda=(\mu-r)/\sigma$, $k=[\delta+(\gamma-1)(r+\lambda^2/(2\gamma))]/\gamma$ and $b(\tau)=\int_0^\tau e^{-ks}\,ds+\eta^{1/\gamma}e^{-k\tau}$. The displayed optimal [consumption](mathematical-finance.md#consumption) and dollar stock position follow by [inverse marginal utility](#inverse-marginal-utility) and the [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint). For $\gamma\ne1$ the value is $b(T-t)^\gamma W_t^{1-\gamma}/(1-\gamma)$ with discount measured from $t$. Finite horizons do not require $k>0$. The [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality) and replication of the optimal budget prove global optimality, rather than only a formal differential-equation solution.

##### Finite-horizon logarithmic investment and consumption

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

For terminal [logarithmic utility](#logarithmic-utility) $a\log V_T$ and running [logarithmic utility](#logarithmic-utility) $b\log c_t$, with $a,b,w_0>0$, constant [Black-Scholes model](mathematical-finance.md#black-scholes-model) coefficients give $\lambda=(a+bT)/w_0$ and $V_t=[a+b(T-t)]/(\lambda\xi_t)$, where $\xi$ is the [state-price density](mathematical-finance.md#state-price-density). The optimal terminal wealth and [consumption](mathematical-finance.md#consumption) are $a/(\lambda\xi_T)$ and $b/(\lambda\xi_t)$. Their discounted budget adds to $(a+bT)/\lambda=w_0$. The [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality), integrated over time, proves optimality; the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives the displayed dollar stock holding. The time-dependent consumption-to-wealth ratio reflects both remaining consumption opportunities and the terminal utility weight.

##### Investment with fixed debt service

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

A fixed loan principal contributes a constant interest outflow $h$. If the objective stops when available [portfolio wealth](mathematical-finance.md#portfolio-wealth) reaches zero, the [value function](mathematical-optimization.md#value-function) has an absorbing boundary $V(0)=0$. This differs from requiring the portfolio to finance the debt service forever.

###### Dual ruin boundary with debt service

↑ **Parent:** [Investment with fixed debt service](#investment-with-fixed-debt-service)

For the [wealth-variable Legendre dual](#wealth-variable-legendre-dual) $J(z)=\sup_{w\geq0}[V(w)-zw]$, a finite slope $z_*=V'(0+)$ at an absorbing zero-wealth boundary makes $J$ identically zero for $z\geq z_*$. Matching gives $J(z_*)=J'(z_*)=0$. It does not generally give $J''(z_*^-)=0$: killing at ruin permits the dual curvature to jump.

##### Constant market price of risk investment

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

When the [market price of risk](mathematical-finance.md#market-price-of-risk) is constant and nonzero [spot volatility](mathematical-finance.md#spot-volatility) gives access to the driving [Brownian motion](brownian-motion.md), changes in volatility only rescale the dollar holding needed for fixed [Brownian portfolio exposures](mathematical-finance.md#brownian-portfolio-exposures). With unrestricted holdings and constant interest and discount rates, the [CRRA utility](#constant-relative-risk-aversion-utility) value is consequently independent of the factor state. Zero volatility requires separate treatment.

##### Consumption satisfaction stock

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

A [consumption satisfaction stock](#consumption-satisfaction-stock) smooths past [consumption](mathematical-finance.md#consumption) by $\xi_t=e^{-\lambda t}\xi_0+\int_0^t e^{-\lambda(t-s)}c_sds$. Unlike [multiplicative habit utility](#multiplicative-habit-utility), the running [utility function](utility-function.md) may depend on this stock alone. A unit of present [consumption](mathematical-finance.md#consumption) raises future [consumption satisfaction](#consumption-satisfaction-stock) while costing one unit of financial [portfolio wealth](mathematical-finance.md#portfolio-wealth).

###### Singular consumption control

↑ **Parent:** [Consumption satisfaction stock](#consumption-satisfaction-stock)

In [singular stochastic control](control-theory.md#singular-stochastic-control), an unrestricted [consumption](mathematical-finance.md#consumption) rate can approximate instantaneous transfers from [portfolio wealth](mathematical-finance.md#portfolio-wealth) into a [consumption satisfaction stock](#consumption-satisfaction-stock). In the relaxed problem a nondecreasing control $C$ records these transfers. A transfer $\Delta C$ decreases [portfolio wealth](mathematical-finance.md#portfolio-wealth) and increases [consumption satisfaction](#consumption-satisfaction-stock) by the same amount. Rate controls need not attain the supremum when the relaxed optimum has a jump.

###### Gradient constraint for unbounded consumption

↑ **Parent:** [Consumption satisfaction stock](#consumption-satisfaction-stock)

If [consumption](mathematical-finance.md#consumption) contributes $c(V_\xi-V_w)$ to the [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) and has no finite upper bound, finite value requires $V_\xi\leq V_w$. Strict inequality makes zero [consumption](mathematical-finance.md#consumption) optimal locally. Equality describes an active transfer boundary, often reached through [singular consumption control](#singular-consumption-control).

###### Wealth-to-satisfaction reduction

↑ **Parent:** [Consumption satisfaction stock](#consumption-satisfaction-stock)

For [CRRA utility](#constant-relative-risk-aversion-utility) of a [consumption satisfaction stock](#consumption-satisfaction-stock), jointly scaling initial [portfolio wealth](mathematical-finance.md#portfolio-wealth), [consumption satisfaction](#consumption-satisfaction-stock) and controls gives [homogeneity](real-analysis.md#homogeneity) of degree $1-R$. The [value function](mathematical-optimization.md#value-function) therefore depends on one dimensionless ratio after factoring out $\xi^{1-R}$. The effective [consumption](mathematical-finance.md#consumption) coefficient becomes $\xi^{-R}[(1-R)v-(x+1)v']$.

##### Investment value transversality condition

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

A discounted-value transversality condition rules out residual value at infinity in an infinite-horizon [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) verification. Under appropriate integrability, admissibility, and localization assumptions, $\mathbb E[e^{-\rho T}V(w_T,s_T)]\to0$ identifies the economic value among formal differential-equation solutions.

##### State-dependent correlation investment problem

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

When asset correlation varies with a traded market index, the index is both an asset and a state variable. Writing $m=\log M$ and optimizing [Brownian portfolio exposures](mathematical-finance.md#brownian-portfolio-exposures) accounts for the cross derivative between wealth and $m$. Power [homogeneity](real-analysis.md#homogeneity) reduces the [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) to an ordinary differential equation in $m$.

###### Power transformation of a complete-market investment equation

↑ **Parent:** [State-dependent correlation investment problem](#state-dependent-correlation-investment-problem)

For a complete-market [investment-consumption problem](#investment-consumption-problem) with [constant relative risk aversion utility](#constant-relative-risk-aversion-utility), the nonlinear wealth-homogeneity coefficient equation may contain $f^{\prime2}/f$. Writing $f=g^R$ cancels this gradient square against the one from $f^{\prime\prime}$. In the index-driven correlation model the result is $\sigma_0^2g^{\prime\prime}/2+Bg^\prime-\delta(m)g+1=0$, a [linear differential equation](differential-equation.md#linear-differential-equation); the positive economic solution gives consumption $w/g$.

##### Intertemporal hedging demand

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

Intertemporal hedging demand adjusts the myopic risky position when investment opportunities depend on a stochastic state. Shared noise between wealth and that state contributes a cross derivative to the [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation). In a complete diffusion market the optimal exposures combine the myopic [market price of risk](mathematical-finance.md#market-price-of-risk) term and the value-gradient hedge term.

###### Learning hedge in a binary-drift investment model

↑ **Parent:** [Intertemporal hedging demand](#intertemporal-hedging-demand)

With the [binary Brownian drift filter](time-series.md#binary-brownian-drift-filter), a stock of observed excess drift $b(x)=\mu-r+\sigma a\tanh(ax)$ is driven by the same [Brownian motion](brownian-motion.md) as its information state $X$. The [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) for [portfolio wealth](mathematical-finance.md#portfolio-wealth) $w$, dollar stock holding $\theta$ and value $J(w,x)$ includes $\sigma\theta J_{wx}$. Consequently $\theta^*=-[b(x)J_w+\sigma J_{wx}]/(\sigma^2J_{ww})$. For [CRRA utility](#constant-relative-risk-aversion-utility), [homogeneity](real-analysis.md#homogeneity) gives $J=K(x)w^{1-R}/(1-R)$ and hence the displayed stock fraction. The second term is [intertemporal hedging demand](#intertemporal-hedging-demand); replacing the unknown drift by its posterior mean while omitting this term does not generally give the optimal policy.

##### High-water mark investment taxation

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

A high-water mark investment tax charges increments of historical maximum wealth $\bar w_t=\max(\bar w_0,\sup_{s\leq t}w_s)$ rather than every positive instantaneous return. For the convention charging $\tau\,d\bar w$, the [high-water mark tax boundary condition](#high-water-mark-tax-boundary-condition) is $V_{\bar w}=\tau V_w$ when the optimal policy raises the maximum. At sufficiently high tax, a [wealth-cap investment boundary](#wealth-cap-investment-boundary) can make further maximum increases suboptimal.

###### Wealth-cap investment boundary

↑ **Parent:** [High-water mark investment taxation](#high-water-mark-investment-taxation)

A wealth-cap investment boundary prevents wealth from exceeding a fixed historical maximum. In the [wealth-variable Legendre dual](#wealth-variable-legendre-dual) for wealth normalized by that maximum, $J^\prime(z_*)=-1$ and vanishing optimal portfolio volatility gives $J^{\prime\prime}(z_*)=0$. For power utility and a high-water tax, the smooth tax-paying solution has boundary dual curvature $(1-\alpha\tau)/(Rz_*)$, so it cannot be admissible when $\alpha\tau>1$.

###### High-water mark tax boundary condition

↑ **Parent:** [High-water mark investment taxation](#high-water-mark-investment-taxation)

At an active maximum-raising boundary in [high-water mark investment taxation](#high-water-mark-investment-taxation), the finite-variation part of the [Itô formula](stochastic-calculus.md#ito-s-lemma) is $(V_{\bar w}-\tau V_w)d\bar w$, so smooth optimality sets this coefficient to zero. If the maximizing policy avoids increasing the maximum, the corresponding inequality $V_{\bar w}-\tau V_w\leq0$ is compatible with a [wealth-cap investment boundary](#wealth-cap-investment-boundary) instead.

##### Merton consumption-investment problem

↑ **Parent:** [Investment-consumption problem](#investment-consumption-problem)

For a constant-coefficient single-asset [investment-consumption problem](#investment-consumption-problem) with [constant relative risk aversion utility](#constant-relative-risk-aversion-utility), put $\kappa=(\mu-r)/\sigma$ and $\delta=[\rho-(1-R)(r+\kappa^2/(2R))]/R$. When $\delta>0$, the infinite-horizon value is $\delta^{-R}w^{1-R}/(1-R)$ and the optimal controls are $c^*=\delta w$ and $\theta^*=(\mu-r)w/(R\sigma^2)$. The case $R=1$ uses logarithmic utility.

###### Regime-switching Merton equations

↑ **Parent:** [Merton consumption-investment problem](#merton-consumption-investment-problem)

For an observed finite-state [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) with rate matrix $Q$, constant bank rate $r$, and state-dependent stock drifts $\mu_i$ and positive volatilities $\sigma_i$, [constant relative risk aversion utility](#constant-relative-risk-aversion-utility) gives $V_i(w)=A_iw^{1-R}/(1-R)$. Set $\kappa_i=(\mu_i-r)/\sigma_i$ and $d_i=\rho-(1-R)(r+\kappa_i^2/(2R))$. The [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) reduces to the displayed nonlinear algebraic system with $A_i>0$. Its feedback controls are $c_i=A_i^{-1/R}w$ and $\theta_i=(\mu_i-r)w/(R\sigma_i^2)$.

A damped [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) in the logarithmic variables $A_i=e^{x_i}$ preserves positivity. Solving these equations produces a candidate value; admissibility, stochastic-integral bounds and the [investment value transversality condition](#investment-value-transversality-condition) still need verification.

###### Retirement boundary with an income option

↑ **Parent:** [Merton consumption-investment problem](#merton-consumption-investment-problem)

Consider irreversible [optimal stopping](martingale.md#optimal-stopping) of employment paying income $\varepsilon>0$ and imposing disutility $\lambda>0$. Assume $r,\rho>0$, nonzero [market price of risk](mathematical-finance.md#market-price-of-risk) $\kappa$, a positive [Merton consumption constant](#merton-consumption-constant), and solvency allowing borrowing against perpetual income up to $\varepsilon/r$ before retirement. Let $m<0$ solve $\kappa^2m(m-1)/2+(\rho-r)m-\rho=0$. The retirement threshold is the displayed wealth level.

To derive it, apply the [wealth-variable Legendre dual](#wealth-variable-legendre-dual). The working dual equals the retired dual plus $h(z)=\varepsilon z/r-\lambda/\rho+Dz^m$. Excluding the growing homogeneous solution enforces the solvency asymptotic. Value matching and [smooth fit](martingale.md#smooth-pasting) at the retirement marginal value $z_*$ give $h(z_*)=h'(z_*)=0$, hence $z_*=(\lambda r/(\varepsilon\rho))m/(m-1)$ and $D=-\varepsilon z_*^{1-m}/(rm)>0$. The retired inverse marginal value gives $\overline w=\gamma_M^{-1}z_*^{-1/R}$.

The root equation implies $z_*/(\lambda/\varepsilon)=1+\kappa^2m/(2\rho)<1$. Thus the boundary exceeds the instantaneous gain-zero level $\gamma_M^{-1}(\varepsilon/\lambda)^{1/R}$. A tighter borrowing constraint changes this free-boundary problem. Smooth fit matches the first derivative; matching the second derivative would incorrectly remove the income option.

###### Merton consumption constant

↑ **Parent:** [Merton consumption-investment problem](#merton-consumption-investment-problem)

In the infinite-horizon [Merton consumption-investment problem](#merton-consumption-investment-problem) with [constant relative risk aversion utility](#constant-relative-risk-aversion-utility), this is the optimal ratio of [consumption](mathematical-finance.md#consumption) to wealth. A finite value requires $\gamma_M>0$. The [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) then fixes consumption's multiplier because $\mathbb E[\xi_t(ye^{\rho t}\xi_t)^{-1/R}]=y^{-1/R}e^{-\gamma_Mt}$, whose time integral is $y^{-1/R}/\gamma_M$. When this integral diverges, the value is $+\infty$ for $0<R<1$ and $-\infty$ for $R>1$.

###### Maximal squared Sharpe ratio value bound

↑ **Parent:** [Merton consumption-investment problem](#merton-consumption-investment-problem)

For $0<R<1$, common constant interest and volatility, and observed excess drift bounded in absolute value by $b_+>0$, let $V_+$ be the finite [Merton consumption-investment problem](#merton-consumption-investment-problem) value for excess drift $b_+$. In its [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation), optimizing the stock holding contributes $-b^2(V_+')^2/(2\sigma^2V_+'')$. Since $V_+''<0$, this contribution increases with $b^2$. Thus every admissible policy makes accumulated discounted [CRRA utility](#constant-relative-risk-aversion-utility) plus discounted $V_+$ a nonnegative [local supermartingale](martingale.md#local-supermartingale), hence a [supermartingale](martingale.md#supermartingale). Dropping its nonnegative terminal term and using the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) proves the value bound. The condition $[\rho-(1-R)(r+b_+^2/(2R\sigma^2))]/R>0$ is essential for the finite supermartingale construction.

###### Exponential interest-rate switch

↑ **Parent:** [Merton consumption-investment problem](#merton-consumption-investment-problem)

Consider an [investment-consumption problem](#investment-consumption-problem) with an independent one-way rate change of intensity $\lambda$ from $r_1$ to $r_0$. For a stock of constant drift $\mu$ and positive volatility $\sigma$, set $B_j=r_j+(\mu-r_j)^2/(2R\sigma^2)$, $\gamma_0=[\rho-(1-R)B_0]/R$, and $D_1=\rho+\lambda-(1-R)B_1$. In the finite-value regime $\gamma_0,D_1>0$, the prechange consumption coefficient is the unique positive root displayed above. The left side increases continuously from zero to infinity. Before the change, the value is $\gamma_1^{-R}w^{1-R}/(1-R)$, the stock fraction is $(\mu-r_1)/(R\sigma^2)$, and [consumption](mathematical-finance.md#consumption) is $\gamma_1w$. At the change these become the ordinary [Merton consumption-investment problem](#merton-consumption-investment-problem) controls for $r_0$. The jump term in the [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) is $\lambda(V_0-V_1)$; knowing only the marginal law of the change time does not justify that term without a conditional intensity assumption.

#### Certainty equivalent

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

A deterministic wealth level $c$ satisfying $U(c)=\mathbb E U(W)$. For normal wealth with [exponential utility](#constant-absolute-risk-aversion-utility) $U(x)=-e^{-\gamma x}$ it is $c=\mathbb EW-\gamma\operatorname{Var}(W)/2$.

#### Expected utility of a Gaussian location-scale family

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

For $X=\mu+\sigma Z$ with $Z$ having the [standard normal distribution](probability-theory.md#standard-normal-distribution) and an increasing concave [utility function](utility-function.md) $U$, define $f(\mu,\sigma)=\mathbb E[U(X)]$. Then $f_\mu=\mathbb E[U'(X)]>0$ and [Gaussian integration by parts](probability-theory.md#stein-s-lemma-probability) gives $f_\sigma=\sigma\mathbb E[U''(X)]\leq0$. Moreover

$$
\operatorname{Hess}f
=\mathbb E\left[U''(X)
\begin{pmatrix}1&Z\\Z&Z^2\end{pmatrix}\right]
$$

is negative semidefinite, so $f$ is jointly [concave](real-analysis.md#concave-function) in $\mu$ and $\sigma$.

#### Indifference price

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indifference_price)

A utility indifference price for a claim is the cash amount at which optimally buying the claim leaves the investor with the same maximal expected utility as trading without it.

##### Periodic utility indifference payment for Gaussian income

↑ **Parent:** [Indifference price](#indifference-price)

For [Gaussian](probability-theory.md#normal-distribution) income of mean $a$, standard deviation $b$ and tradable [correlation](variance.md#pearson-correlation-coefficient) $\rho$, exponential utility makes the maximum acceptable per-period fee equal to the mean minus the correlated-income hedge cost and the residual [variance](variance.md) penalty. Compare optimized utilities with and without the contract; a fee above this level makes the contract strictly inferior. At perfect [correlation](variance.md#pearson-correlation-coefficient) the residual penalty vanishes, leaving only the mean and hedge-cost terms.

#### Optimized affine shift of concave utility

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

Let $\mathcal X$ be a vector space of random variables and suppose

$$
F(y)=\sup_{X\in\mathcal X}\mathbb E[U(X+y)]
$$

has an optimizer for every $y$. If $U$ is increasing and concave, then $F$ is increasing and concave. For concavity, combine optimizers at two values using the same convex coefficient as the values themselves.

#### Scaled centered risk under concave utility

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

If $U$ is concave and $\mathbb E Z=0$, then

$$
G(s)=\mathbb E[U(m+sZ)]
$$

is concave in $s$. By [Jensen inequality](real-analysis.md#jensen-s-inequality), $G(s)\leq G(0)$; concavity then makes $G$ nonincreasing on $[0,\infty)$.

#### Utility duality with martingale deflators

↑ **Parent:** [Expected utility maximization](#expected-utility-maximization)

The concave conjugate $\widehat u(y)=\sup_{x>0}\{u(x)-xy\}$ gives the weak-duality bound $\mathbb Eu(X)\leq\mathbb E\widehat u(Y)+X_0Y_0$. Equality holds when $u'(X)=Y$ and the payoff exhausts the deflated budget.

##### Logarithmic terminal wealth in a complete market

↑ **Parent:** [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)

In a [complete market](mathematical-finance.md#complete-market) with a unit cash asset and normalized strictly positive [state-price density](mathematical-finance.md#state-price-density) $Z$, the optimal positive terminal [portfolio wealth](mathematical-finance.md#portfolio-wealth) is $x/Z$ whenever it is replicable in the admissible class. The [state-price budget constraint](mathematical-finance.md#state-price-budget-constraint) is an equality: $\mathbb E[Z(x/Z)]=x$. The [utility conjugate](convex-optimization.md#utility-conjugate) inequality gives $\mathbb E\log H\leq\log x-\mathbb E\log Z$ for every affordable positive claim. This value can be infinite, because $\mathbb E(\log Z)^+<\infty$ while $\mathbb E(\log Z)^-$ need not be finite. Even completeness for bounded claims suffices to approximate the value: set $b_n=\mathbb E[Z/(Z\vee n^{-1})]$ and $H_n=x/[b_n(Z\vee n^{-1})]$. Each claim is bounded and costs $x$, while its expected [logarithmic utility](#logarithmic-utility) tends to the displayed value by [monotone convergence](measure-theory.md#monotone-convergence-theorem) after an integrable lower bound is subtracted.

##### Optimal marginal utility as a one-period pricing density

↑ **Parent:** [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)

For a negative, strictly increasing, concave differentiable utility with finite expected utility at every holding, a gain having both signs makes the objective coercive at both ends. At a finite optimum its derivative is zero. [Secant domination for expected utility derivatives](#secant-domination-for-expected-utility-derivatives) gives [integrability](measure-theory.md#integrability) of $|X|U'(\theta_*X)$; boundedness of $U'$ on the remaining compact set gives [integrability](measure-theory.md#integrability) of the positive marginal utility itself. Its normalization has [expectation](probability-theory.md#expected-value) one and prices the gain at zero.

###### Marginal utility price

↑ **Parent:** [Optimal marginal utility as a one-period pricing density](#optimal-marginal-utility-as-a-one-period-pricing-density)

In a one-period utility problem with gross riskless return $R$, the marginal utility price is the infinitesimal claim price leaving optimized expected utility unchanged. If optimal terminal wealth is $W^*$, the pricing density is $Z=U'(W^*)/(R\mathbb E U'(W^*))$, and $p_H=\mathbb E[ZH]$. The denominator is the marginal utility of initial wealth. Under the standard first-order optimality conditions this density prices the traded assets and gives the [state-price density](mathematical-finance.md#state-price-density) associated with the investor.

###### Marginal utility pricing with proportional transaction costs

↑ **Parent:** [Optimal marginal utility as a one-period pricing density](#optimal-marginal-utility-as-a-one-period-pricing-density)

At a nonzero optimum, the derivative of expected utility of a [proportional transaction cost](#proportional-transaction-cost) payoff is zero. Normalized marginal utility therefore prices $X$ at $\varepsilon$ for a positive optimum or $-\varepsilon$ for a negative optimum. At a zero optimum the one-sided derivative inequalities put $\mathbb EX$ inside that interval, so density one works. The competing one-sided-payoff alternative prevents the coercive-maximizer argument from being assumed when a net gain has only one sign.

##### One-period marginal-utility certificate of optimality

↑ **Parent:** [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)

For a positive [state-price density](mathematical-finance.md#state-price-density) $Z$ pricing every attainable payoff, a feasible positive terminal payoff $W^*$ is optimal at its budget if its marginal utility is $yZ$ for some scalar $y>0$. The pointwise conjugate inequality gives $\mathbb EU(W)\leq\mathbb E\widehat U(yZ)+yx$ for every competitor; the marginal-utility identity makes equality hold for $W^*$. Finite states make integrability straightforward. In a [complete market](mathematical-finance.md#complete-market) an interior optimum also necessarily has this proportionality, by variations preserving the state-price budget.

##### Marginal-utility verification of optimal consumption

↑ **Parent:** [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)

For [concave](real-analysis.md#concave-function) increasing utility, the [concave supporting-tangent inequality](real-analysis.md#concave-supporting-tangent-inequality) gives $e^{-bt}[U(\hat c_t)-U(c_t)]\leq Y_t(\hat c_t-c_t)$. If the proposed [consumption](mathematical-finance.md#consumption) exhausts the state-price budget and every competitor has no larger budget, integration proves optimality. The objective must be well defined; a positive discount rate and finite utility bounds are a convenient sufficient condition.

##### Wealth-variable Legendre dual

↑ **Parent:** [Utility duality with martingale deflators](#utility-duality-with-martingale-deflators)

For increasing strictly [concave](real-analysis.md#concave-function) wealth value $v$, the dual $J(z)=\sup_x[v(x)-xz]$ is convex. At an interior optimum $z=v^\prime(x)$, $J^\prime=-x$, $J^{\prime\prime}=-1/v^{\prime\prime}>0$, and $v=J-zJ^\prime$. This sign convention is the negative of the [concave Legendre dual](convex-optimization.md#concave-legendre-dual). It can turn the optimized portfolio term of a [Hamilton-Jacobi-Bellman equation](mathematical-optimization.md#hamilton-jacobi-bellman-equation) into a linear second derivative.

## ↑ Ancestors (5)

1. [Mathematical finance](mathematical-finance.md)
2. [Mathematical optimization](mathematical-optimization.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (52)

- [Binomial power-utility terminal wealth](#binomial-power-utility-terminal-wealth)
- [Competitive equilibrium with one productive asset](mathematical-finance.md#competitive-equilibrium-with-one-productive-asset)
- [Complete-market terminal utility optimizer](#complete-market-terminal-utility-optimizer)
- [Concavification of incentive utility](#concavification-of-incentive-utility)
- [Consumption satisfaction stock](#consumption-satisfaction-stock)
- [Demand correspondence](mathematics.md#demand-correspondence)
- [Expected utility](#expected-utility)
- [Expected utility hypothesis](#expected-utility-hypothesis)
- [Expected utility of a Gaussian location-scale family](#expected-utility-of-a-gaussian-location-scale-family)
- [Hedge fund incentive utility](#hedge-fund-incentive-utility)
- [Inada conditions](#inada-conditions)
- [Inverse marginal utility](#inverse-marginal-utility)
- [Marginal utility](#marginal-utility)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-36.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#29i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#5/with-transaction-costs/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-40.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-41.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#30k/a/solution)
- [Relative-consumption share equilibrium](mathematical-finance.md#relative-consumption-share-equilibrium)
- [Relative risk aversion coefficient](#relative-risk-aversion-coefficient)
- [Risk aversion](#risk-aversion)
- [Risk premium](#risk-premium)
- [Risk seeking](#risk-seeking)
- [Secant domination for expected utility derivatives](#secant-domination-for-expected-utility-derivatives)
- [Singular-volatility drift arbitrage](mathematical-finance.md#singular-volatility-drift-arbitrage)
- [Uniform utility convergence need not preserve closed preference convergence](set-theory.md#uniform-utility-convergence-need-not-preserve-closed-preference-convergence)
- [Utility](mathematics.md#utility)
- [Utility function](utility-function.md)
