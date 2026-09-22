# Paper 23

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper23.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper23.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The no-borrowing [portfolio](../../../mathematical-finance.md#investment-portfolio) constraint is $0\le x\le T$. Net [asset returns](../../../mathematical-finance.md#financial-return) must be added to the original principal. Thus the two final [portfolio wealths](../../../mathematical-finance.md#portfolio-wealth) are

$$
\boxed{w_g=x(1+r)+(T-x)(1+g)=T(1+g)-(g-r)x,\qquad w_b=x(1+r)+(T-x)(1+b)=T(1+b)+(r-b)x.}
$$

The [expected utility](../../../utility-function.md#expected-utility) is

$$
\boxed{U(x)=p\,u(w_g)+(1-p)u(w_b).}
$$

The probabilities are those of the investor's beliefs; no [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) is being used in this preference calculation.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

[Risk neutrality](../../../utility-function.md#risk-neutrality) means indifference between a random [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) and its certain [expected value](../../../probability-theory.md#expected-value). For increasing twice differentiable [expected utility](../../../utility-function.md#expected-utility) preferences, this corresponds to an [affine function](../../../vector-space.md#affine-function) $u(w)=Aw+C$ with $A>0$ on the relevant wealth interval. Maximizing [expected utility](../../../utility-function.md#expected-utility) then amounts to maximizing [expected return](../../../mathematical-finance.md#expected-return):

$$
\mathbb Ew=T[1+pg+(1-p)b]+x[r-pg-(1-p)b].
$$

The coefficient of $x$ is strictly negative. Consequently **the unique optimum is $x_*=0$: invest all initial wealth in equity**. [Risk neutrality](../../../utility-function.md#risk-neutrality) here is a preference property, distinct from the pricing use of a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

[Risk aversion](../../../utility-function.md#risk-aversion) means that a sure mean is preferred to the corresponding risky [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth). An increasing [concave](../../../real-analysis.md#concave-function) [utility function](../../../utility-function.md), with $u'>0$ and $u''\le0$, has this property by the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality); [strictly concave](../../../real-analysis.md#strictly-concave-function) utility gives strict preference for nondegenerate risks. Differentiating the [expected utility](../../../utility-function.md#expected-utility) from part (a) gives

$$
U'(x)=-p(g-r)u'(w_g)+(1-p)(r-b)u'(w_b),\qquad U''(x)=p(g-r)^2u''(w_g)+(1-p)(r-b)^2u''(w_b)\le0.
$$

An interior optimum therefore satisfies

$$
\boxed{p(g-r)u'(w_g)=(1-p)(r-b)u'(w_b).}
$$

This balances the expected loss of [marginal utility](../../../utility-function.md#marginal-utility) in the good state against its expected gain in the bad state. The borrowing constraint also requires checking the endpoints: $x_*=0$ if $U'(0)\le0$, while $x_*=T$ would require $U'(T)\ge0$. At $x=T$ both state wealths equal $T(1+r)$, so

$$
U'(T)=[r-pg-(1-p)b]u'(T(1+r))<0.
$$

Hence an optimum never puts all wealth into deposits. If $U'(0)>0$, continuity and the displayed endpoint sign give an interior root, and [concavity](../../../real-analysis.md#concave-function) makes every such root globally optimal. Under [strict concavity](../../../real-analysis.md#strict-concavity) it is unique.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Assume first that $T>0$ and $-1<b<r<g$, so the [logarithmic utility](../../../utility-function.md#logarithmic-utility) is defined throughout the allowed [portfolio](../../../mathematical-finance.md#investment-portfolio) interval. Put $A=g-r>0$ and $B=r-b>0$. Then

$$
U'(x)=-\frac{pA}{T(1+g)-Ax}+\frac{(1-p)B}{T(1+b)+Bx}.
$$

Equating this to zero and clearing the positive denominators gives

$$
x_0=T\left[\frac{(1-p)(1+g)}{g-r}-\frac{p(1+b)}{r-b}\right].
$$

The second [derivative](../../../calculus.md#derivative) is strictly negative, and $U'(T)<0$ by part (c), so $x_0<T$. The [two-state logarithmic portfolio with a borrowing constraint](../../../utility-function.md#two-state-logarithmic-portfolio-with-a-borrowing-constraint) is therefore

$$
\boxed{x_*=\max\{0,x_0\},\qquad\text{equity investment}=T-x_*.}
$$

In particular, the threshold for all equity is

$$
p\ge p_c:=\frac{(r-b)(1+g)}{(r-b)(1+g)+(g-r)(1+b)}
=\frac{(r-b)(1+g)}{(g-b)(1+r)}.
$$

For $p<p_c$ the optimum is interior. The probability bound printed in the PDF has $1+r$ where the all-equity threshold has $1+b$. Since $1+r>1+b$, that printed lower bound is strictly below $p_c$ and does not determine which of these two cases occurs. For example, with $(b,r,g)=(0,0.1,0.3)$ its lower bound is $13/35$, while $p_c=13/33$. At $p=0.38$ all the given inequalities hold and $x_*=0.23T$; at $p=0.4$ they also hold and $x_*=0$. Thus the boxed constrained formula applies to the printed data without replacing its probability assumption.

If bad-state gross wealth can be nonpositive, the [logarithmic utility](../../../utility-function.md#logarithmic-utility) domain must instead be imposed explicitly. With $1+r>0$, $b\le-1$, and $0<p<1$, admissibility requires $x>-T(1+b)/(r-b)$; the same stationary root lies inside this positive-wealth interval and is optimal. If even the fully safe gross return is nonpositive, there is no admissible positive-wealth [portfolio](../../../mathematical-finance.md#investment-portfolio). These domain issues are implicit in using $\log w$.

## 2

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use unrestricted long and short [portfolios](../../../mathematical-finance.md#investment-portfolio), as required by the usual [arbitrage pricing theory](../../../mathematical-finance.md#arbitrage-pricing-theory) argument. A vector $v\in\mathbb R^n$ of initial monetary positions with $\mathbf1^Tv=0$ costs zero. Its terminal [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff), in the exact one-factor model, is

$$
v^T(\mathbf1+r)=v^Ta+(v^Tb)f.
$$

If also $v^Tb=0$, the [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) is the constant $v^Ta$. A nonzero value would be an [arbitrage](../../../mathematical-finance.md#arbitrage) after choosing the sign of $v$. Absence of [arbitrage](../../../mathematical-finance.md#arbitrage) thus says that $a$ annihilates $\ker[\mathbf1\ b]^T$. By finite-dimensional [linear algebra](../../../linear-algebra.md),

$$
a\in(\ker[\mathbf1\ b]^T)^\perp=\operatorname{span}\{\mathbf1,b\}.
$$

Write $a=\lambda_0\mathbf1+\kappa b$. Taking [expectations](../../../probability-theory.md#expected-value), assuming the factor has finite mean, proves

$$
\boxed{\bar r_i=\lambda_0+b_i\lambda_1,\qquad\lambda_1=\kappa+\mathbb Ef.}
$$

This is [exact factor pricing without a traded risk-free asset](../../../mathematical-finance.md#exact-factor-pricing-without-a-traded-risk-free-asset). The PDF prints an asset-indexed $\lambda_i$; the stronger valid result has the same $\lambda_1$ for every asset, so it also satisfies the printed relation by taking all its $\lambda_i$ equal. If every loading is equal, the spanning vectors are dependent and the coefficients need not be unique. For a nondegenerate factor and a zero-exposure unit-cost [portfolio](../../../mathematical-finance.md#investment-portfolio), $\lambda_0$ is that [portfolio](../../../mathematical-finance.md#investment-portfolio)'s certain return; if a [risk-free asset](../../../mathematical-finance.md#risk-free-asset) is explicitly traded, [law of one price](../../../mathematical-finance.md#law-of-one-price) makes it the [risk-free asset](../../../mathematical-finance.md#risk-free-asset)'s return. No equilibrium preferences are needed for this argument.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [capital asset pricing model](../../../mathematical-finance.md#capital-asset-pricing-model) gives

$$
\mathbb Er_i=r_f+\beta_i(\mathbb Er_M-r_f),\qquad
\beta_i=\frac{\operatorname{Cov}(r_i,r_M)}{\operatorname{Var}(r_M)}.
$$

Thus it has the same affine relation between [expected returns](../../../mathematical-finance.md#expected-return) and a single systematic exposure. When the factor is the [market portfolio](../../../mathematical-finance.md#market-portfolio)'s excess return, the loadings are the [beta of an asset](../../../mathematical-finance.md#beta-of-an-asset), $\lambda_0=r_f$, and $\lambda_1=\mathbb Er_M-r_f$. More generally, for a nondegenerate exact one-factor model and a [market portfolio](../../../mathematical-finance.md#market-portfolio) with loading $b_M\ne0$, $\beta_i=b_i/b_M$, and the pricing relation can be rewritten using that exposure.

The interpretations and assumptions differ. The [CAPM](../../../mathematical-finance.md#capital-asset-pricing-model) is an equilibrium relation obtained with a [mean-variance optimization](../../../mathematical-finance.md#modern-portfolio-theory) framework, common beliefs, and suitable borrowing/lending and market-clearing assumptions. [Arbitrage pricing theory](../../../mathematical-finance.md#arbitrage-pricing-theory) uses absence of [arbitrage](../../../mathematical-finance.md#arbitrage), factor structure, and in realistic models [diversification](../../../mathematical-finance.md#portfolio-diversification); it does not identify a generic factor with the [market portfolio](../../../mathematical-finance.md#market-portfolio). Moreover the [CAPM](../../../mathematical-finance.md#capital-asset-pricing-model) permits asset-specific risk, whereas the exact model in part (a) has no residual risk. **The two formulas coincide for a suitable market factor, but no-arbitrage factor pricing by itself does not establish the CAPM's equilibrium assumptions.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $B$ be the $n\times m$ matrix of [factor loadings](../../../statistical-modelling.md#factor-loading), so $r=a+Bf$. A zero-cost [portfolio](../../../mathematical-finance.md#investment-portfolio) $v$ with $\mathbf1^Tv=0$ and $B^Tv=0$ again has constant [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) $v^Ta$. Absence of [arbitrage](../../../mathematical-finance.md#arbitrage) implies

$$
a\in\operatorname{col}[\mathbf1\ B],\qquad
a=\lambda_0\mathbf1+B\kappa.
$$

Taking [expectations](../../../probability-theory.md#expected-value) gives

$$
\boxed{\mathbb Er_i=\lambda_0+\sum_{j=1}^m b_{ij}\lambda_j,\qquad
\lambda_j=\kappa_j+\mathbb Ef_j.}
$$

If $[\mathbf1\ B]$ has full column [rank](../../../linear-algebra.md#rank-one-quadratic-form), a unit-cost [portfolio](../../../mathematical-finance.md#investment-portfolio) with zero exposure to all factors exists and earns the certain rate $\lambda_0$. For each $j$, choose a zero-cost [portfolio](../../../mathematical-finance.md#investment-portfolio) with loading one on factor $j$ and zero on the others; its [expected return](../../../mathematical-finance.md#expected-return) is $\lambda_j$. Hence these coefficients are the rewards per unit systematic exposure, or factor [risk premiums](../../../utility-function.md#risk-premium), with the [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) measured per unit of the chosen factor normalization. A traded [risk-free asset](../../../mathematical-finance.md#risk-free-asset) fixes $\lambda_0$ to its return. Changing the scale or basis of the factors changes the coordinates of the [risk premiums](../../../utility-function.md#risk-premium) but leaves asset prices unchanged. With deficient [rank](../../../linear-algebra.md#rank-one-quadratic-form), only the spanned factor directions are identified and the coefficients need not be unique.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For weights summing to one, collect the exact [portfolio](../../../mathematical-finance.md#investment-portfolio) return as

$$
r^{(n)}=a^{(n)}+\sum_{j=1}^m b_j^{(n)}f_j+e_n,\qquad
a^{(n)}=\sum_iw_i a_i,\quad b_j^{(n)}=\sum_iw_ib_{ij},\quad e_n=\sum_iw_i\epsilon_i.
$$

The desired approximation means that $e_n\to0$, for example in [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2). Centering the residuals gives $\mathbb Ee_n=0$, but its [variance](../../../variance.md) is

$$
\operatorname{Var}(e_n)=\sum_{i,k}w_iw_k\operatorname{Cov}(\epsilon_i,\epsilon_k).
$$

This identifies an omission in the printed hypotheses: bounded individual [variances](../../../variance.md) do not control the cross terms. Indeed, take $\epsilon_i=Z$ for every $i$, where $Z$ is a nondegenerate centered [random variable](../../../random-variable.md) with $\operatorname{Var}Z<s^2$. Equal weights $1/n<W/n$ for any $W>1$ retain $e_n=Z$ at every $n$. **The claimed diversification conclusion does not follow from the printed assumptions alone.**

Under the usual extra assumption that the residuals are pairwise uncorrelated and the weights are nonnegative, the advertised calculation is

$$
\mathbb Ee_n^2=\sum_iw_i^2\sigma_i^2
\le s^2\left(\max_iw_i\right)\sum_iw_i
\le\frac{s^2W}{n}\longrightarrow0.
$$

The [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) then gives $\Pr(|e_n|>\delta)\le s^2W/(n\delta^2)\to0$. Alternatively, signed weights satisfying $|w_i|\le W/n$ give the bound $s^2W^2/n$. These are instances of the [covariance criterion for diversification of factor residuals](../../../mathematical-finance.md#covariance-criterion-for-diversification-of-factor-residuals). More generally, with that absolute weight bound, $\sum_{i,k}|\operatorname{Cov}(\epsilon_i,\epsilon_k)|=o(n^2)$ suffices.

If [short selling](../../../mathematical-finance.md#short-finance) are allowed, the printed one-sided weight bound is another insufficiency. Choose $0<c<W-1$, put $w_1=-c$ and $w_i=(1+c)/(n-1)$ for $i\ge2$, and let only $\epsilon_1$ be a nondegenerate centered residual. For all sufficiently large $n$ the one-sided bounds hold, but $e_n=-c\epsilon_1$ never vanishes. Thus nonnegative weights or an absolute bound is needed.

With the repaired assumptions, **well-diversified [portfolios](../../../mathematical-finance.md#investment-portfolio) become approximately exposed only to the common factors**, and their residual [standard deviation](../../../variance.md#standard-deviation) is $O(n^{-1/2})$ in the uncorrelated case. The averaged coefficients may depend on $n$; convergence to fixed coefficients needs additional assumptions. In the associated asymptotic [arbitrage pricing theory](../../../mathematical-finance.md#arbitrage-pricing-theory), diversifiable risk cannot command a persistent premium in well-diversified [portfolios](../../../mathematical-finance.md#investment-portfolio) under absence of asymptotic [arbitrage](../../../mathematical-finance.md#arbitrage), while common-factor exposure can. This does not prove an exact pricing equation for every individual noisy asset from the finite-market hypotheses alone.

## 3

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

On a [filtered probability space](../../../stochastic-process.md#filtered-probability-space) carrying a standard [Brownian motion](../../../brownian-motion.md) $W$ with independent increments relative to the [filtration](../../../stochastic-process.md#filtration-probability-theory), a strictly positive security price follows [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) with constant drift $\mu$ and volatility $\sigma$ if it solves the [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation)

$$
\boxed{dS_t=\mu S_t\,dt+\sigma S_t\,dW_t,\qquad S_0>0.}
$$

Here $W_t-W_s$ is independent of $\mathcal F_s$ and has the [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,t-s)$ for $s<t$. The solution is

$$
S_t=S_0\exp\{(\mu-\sigma^2/2)t+\sigma W_t\}.
$$

Indeed applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to this exponential gives the specified drift and volatility. Consequently the price is positive and continuous, and

$$
\log(S_t/S_s)\mid\mathcal F_s\sim
N((\mu-\sigma^2/2)(t-s),\sigma^2(t-s)).
$$

Thus disjoint log-return increments are independent and stationary. The parameter $\mu$ is the instantaneous expected relative return under the physical [probability measure](../../../probability-theory.md#probability-measure), not the mean log-return. Under the pricing [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) it becomes the risk-free rate for a non-dividend-paying [stock](../../../mathematical-finance.md#stock).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

One alternative is a [stochastic volatility model](../../../mathematical-finance.md#stochastic-volatility-model), such as the [Heston model](../../../mathematical-finance.md#heston-model):

$$
dS_t=\mu S_tdt+\sqrt{v_t}S_tdW_t^{(1)},\qquad
dv_t=\kappa(\theta-v_t)dt+\xi\sqrt{v_t}\,dW_t^{(2)},\qquad
d\langle W^{(1)},W^{(2)}\rangle_t=\rho\,dt.
$$

The parameters satisfy $\kappa,\theta,\xi>0$ and $|\rho|\le1$, and $v_0\ge0$. The square-root [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion) has a nonnegative solution; $2\kappa\theta\ge\xi^2$ is a standard sufficient condition for the positive initial [variance](../../../variance.md) not to hit zero. Mean reversion of $v_t$ allows persistent high- and low-volatility episodes, and negative $\rho$ can produce the empirical association between falling prices and rising volatility. Mixtures of conditional return distributions produce richer tails and option [implied volatility](../../../mathematical-finance.md#implied-volatility) shapes than constant-volatility [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion).

For data showing [volatility clustering](../../../time-series.md#volatility-clustering) and option smiles, this is often a more useful fit. It is not universally superior: more parameters create estimation and calibration uncertainty, the model is more expensive to use, and its continuous price paths still exclude price jumps. With two independent noise directions and only a [stock](../../../mathematical-finance.md#stock) and a [bank account](../../../mathematical-finance.md#bank-account), the market is generally incomplete, so a volatility [risk premium](../../../utility-function.md#risk-premium) or an extra traded instrument is needed for unique [contingent claim](../../../mathematical-finance.md#contingent-claim) pricing. **The alternative improves flexibility at the cost of calibration and hedging complexity.**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For an [Itô process](../../../stochastic-calculus.md#ito-process) $dX_t=a_tdt+b_tdW_t$ and $F\in C^{1,2}$, the differential [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) is

$$
\boxed{dF(t,X_t)=\left(F_t+a_tF_x+\frac12b_t^2F_{xx}\right)dt+b_tF_x\,dW_t,}
$$

where the [derivatives](../../../calculus.md#derivative) are evaluated at $(t,X_t)$. A multidimensional version replaces $b_t^2F_{xx}$ by the contraction of the [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion) [covariance matrix](../../../variance.md#covariance-matrix) with the spatial [Hessian](../../../calculus.md#hessian-matrix).

For a heuristic derivation, partition time and use the Euler increment $\Delta X=a\,\Delta t+b\sqrt{\Delta t}\,Z$, where $Z$ is standard normal. A second-order [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
\Delta F=F_t\Delta t+F_x\Delta X+\frac12F_{xx}(\Delta X)^2+\text{higher-order terms}.
$$

The term $b^2(\Delta W)^2$ has order $\Delta t$, so it survives summation; ordinary first-order calculus would incorrectly discard it. For independent [Brownian motion](../../../brownian-motion.md) increments,

$$
\mathbb E\sum_k[(\Delta W_k)^2-\Delta t_k]=0,\qquad
\operatorname{Var}\left(\sum_k[(\Delta W_k)^2-\Delta t_k]\right)
=2\sum_k(\Delta t_k)^2\longrightarrow0.
$$

This gives the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $[W]_t=t$. The summed mixed $dt\,dW$ terms and $dt^2$ terms vanish, while the linear random increments converge to an [Itô integral](../../../stochastic-calculus.md#ito-integral). After localizing bounded coefficients and [derivatives](../../../calculus.md#derivative), Taylor remainders are negligible and the surviving terms give the formula. Thus $(dW)^2=dt$ is shorthand for a statement about summed [quadratic variation](../../../stochastic-calculus.md#quadratic-variation), not an equality of individual random increments.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Assume a frictionless market with no taxes or transaction costs, unrestricted [short selling](../../../mathematical-finance.md#short-finance) and borrowing/lending at the same constant rate $r$, continuous trading, and absence of [arbitrage](../../../mathematical-finance.md#arbitrage). The non-dividend-paying [stock](../../../mathematical-finance.md#stock) has [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion) dynamics $dS=\mu Sdt+\sigma SdW$ with constant $\sigma>0$, and the [bank account](../../../mathematical-finance.md#bank-account) satisfies $dB=rBdt$. A [contingent claim](../../../mathematical-finance.md#contingent-claim) with no interim cash flows has sufficiently regular value $f(t,S)$, meaning $f\in C^{1,2}$ before maturity; terminal [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) kinks can be handled by the smooth value for earlier times. Trading strategies are [adapted](../../../stochastic-process.md#adapted-process), [self-financing portfolios](../../../mathematical-finance.md#self-financing-portfolio), and [admissible trading strategies](../../../mathematical-finance.md#admissible-trading-strategy) so that doubling strategies are excluded.

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
df=\left(f_t+\mu Sf_S+\frac12\sigma^2S^2f_{SS}\right)dt+\sigma Sf_SdW.
$$

Choose $\Delta=f_S$ shares and put the remaining value $f-Sf_S$ in the [bank account](../../../mathematical-finance.md#bank-account). Its self-financing gain is

$$
\Delta\,dS+r(f-S\Delta)dt
=\{\mu Sf_S+r(f-Sf_S)\}dt+\sigma Sf_SdW.
$$

Matching the [contingent claim](../../../mathematical-finance.md#contingent-claim)'s gain to this replicating gain cancels the random increment and equates the drifts:

$$
\boxed{f_t+\frac12\sigma^2S^2f_{SS}+rSf_S-rf=0.}
$$

This is the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation). The argument uses the self-financing gain $\Delta\,dS$, not a product differential that incorrectly treats a changing $\Delta$ as free cash. Rebalancing purchases are financed from the [bank account](../../../mathematical-finance.md#bank-account). Conversely, a smooth solution with suitable growth and [boundary conditions](../../../differential-equation.md#boundary-condition) defines a [delta hedge](../../../mathematical-finance.md#delta-hedge) whose value replicates the [contingent claim](../../../mathematical-finance.md#contingent-claim); [law of one price](../../../mathematical-finance.md#law-of-one-price) identifies this value with the [contingent claim](../../../mathematical-finance.md#contingent-claim) price. Here $S$ is the current [stock](../../../mathematical-finance.md#stock) price, $t$ is time, $\sigma$ is proportional volatility, $r$ is the risk-free rate, and $f$ is the [contingent claim](../../../mathematical-finance.md#contingent-claim) price. The physical [expected return](../../../mathematical-finance.md#expected-return) $\mu$ cancels because exposure to price risk has been hedged.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For strike $K>0$ and maturity $T$, a [European call option](../../../mathematical-finance.md#european-call-option) and a [European put option](../../../mathematical-finance.md#european-put-option) have [boundary conditions](../../../differential-equation.md#boundary-condition)

$$
C(T,S)=(S-K)^+,\qquad P(T,S)=(K-S)^+.
$$

The [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) is solved backward from these conditions. At zero [stock](../../../mathematical-finance.md#stock) price, the zero state is absorbing in [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion), so

$$
C(t,0)=0,\qquad P(t,0)=Ke^{-r(T-t)}.
$$

At the other boundary, with $\tau=T-t>0$,

$$
C(t,S)-[S-Ke^{-r\tau}]\longrightarrow0,\qquad P(t,S)\longrightarrow0
\quad(S\to\infty).
$$

These conditions and a suitable growth bound select the financial solution and provide boundary data for numerical truncations. In the constant-coefficient model, under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure),

$$
S_T=S\exp\{(r-\sigma^2/2)\tau+\sigma\sqrt{\tau}\,Z\},\qquad Z\sim N(0,1).
$$

For $d_1=[\log(S/K)+(r+\sigma^2/2)\tau]/(\sigma\sqrt{\tau})$ and $d_2=d_1-\sigma\sqrt{\tau}$, the exercise event is $Z>-d_2$. Completing the square in $e^{\sigma\sqrt{\tau}Z}$ times the normal density gives the truncated first moment and hence

$$
\boxed{C=S\Phi(d_1)-Ke^{-r\tau}\Phi(d_2),\qquad
P=Ke^{-r\tau}\Phi(-d_2)-S\Phi(-d_1),}
$$

where $\Phi$ is the standard normal [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function). These are the [Black-Scholes formula](../../../mathematical-finance.md#black-scholes-formula) values and satisfy the specified terminal and [boundary conditions](../../../differential-equation.md#boundary-condition).

[Put-call parity](../../../mathematical-finance.md#put-call-parity) is the relation

$$
\boxed{C-P=S-Ke^{-r(T-t)}.}
$$

A call minus a put has terminal [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) $S_T-K$. A [portfolio](../../../mathematical-finance.md#investment-portfolio) of one share minus a [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) paying $K$ has the same [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff), so absence of [arbitrage](../../../mathematical-finance.md#arbitrage) and [law of one price](../../../mathematical-finance.md#law-of-one-price) equate their current values. The formula here assumes the same strike and maturity and no dividends; known dividends modify the stock-side value.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

An [American option](../../../mathematical-finance.md#american-option) allows exercise at a [stopping time](../../../martingale.md#stopping-time) $\tau\in[t,T]$. For its exercise [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) $H$, the pricing problem is

$$
\boxed{V(t,S)=\sup_{\tau\in[t,T]}\mathbb E_Q[e^{-r(\tau-t)}H(S_\tau)\mid S_t=S].}
$$

The discounted value is the [Snell envelope](../../../martingale.md#snell-envelope) of discounted exercise payoffs. Define the pricing operator

$$
\mathcal LV=V_t+\frac12\sigma^2S^2V_{SS}+rSV_S-rV.
$$

In the continuation region the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) holds, $\mathcal LV=0$. In the exercise region $V=H$, while the ability to wait and the [supermartingale](../../../martingale.md#supermartingale) property give $\mathcal LV\le0$. Together these conditions are the [obstacle problem](../../../partial-differential-equation.md#obstacle-problem)

$$
\boxed{\max\{H-V,\mathcal LV\}=0,\qquad V(T,S)=H(S).}
$$

Thus an unknown exercise boundary must be found alongside the value. At a regular boundary in the nondegenerate [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion), value matching is $V=H$, and [smooth pasting](../../../martingale.md#smooth-pasting) is $V_S=H'$ where the [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) is differentiable. A [finite difference method](../../../finite-difference.md#finite-difference-method) or a [binomial options pricing model](../../../mathematical-finance.md#binomial-options-pricing-model) steps backward taking the larger of continuation and immediate exercise values at each node.

For a non-dividend-paying [American call option](../../../mathematical-finance.md#american-call-option) with $r\ge0$, [no early exercise of a call without dividends](../../../mathematical-finance.md#no-early-exercise-of-a-call-without-dividends) follows directly from the European lower bound

$$
C_E(t,S)\ge\max\{S-Ke^{-r(T-t)},0\}\ge(S-K)^+.
$$

At every candidate exercise time, keeping the European call has value at least the immediate exercise [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff), so early exercise cannot improve the value; the American and European prices coincide. The first inequality follows from [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) or [put-call parity](../../../mathematical-finance.md#put-call-parity) and nonnegative put value. With $r>0$ an [American put option](../../../mathematical-finance.md#american-put-option) can benefit from early receipt of its strike at sufficiently low [stock](../../../mathematical-finance.md#stock) prices, so its exercise boundary is generally nontrivial and its value is at least the European put value. Dividends can make call exercise worthwhile, and negative interest invalidates the stated no-early-exercise call argument.

## 4

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a continuous strictly increasing [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) $F$ and a [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) $U$ on $(0,1)$, monotonicity gives

$$
\Pr(F^{-1}(U)\le y)=\Pr(U\le F(y))=F(y).
$$

Thus **each transformed draw has distribution function $F$**. This is [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling). The conclusion extends to discontinuous or non-strictly increasing $F$ by its [quantile function](../../../probability-theory.md#quantile-function) $Q(u)=\inf\{x:F(x)\ge u\}$: right continuity gives $Q(u)\le y$ exactly when $u\le F(y)$. Independent uniforms produce independent transformed draws, but marginal uniformity alone does not establish [independence](../../../random-variable.md#independent-random-variables).

If “uniformly distributed sequence” instead means deterministic equidistribution, the empirical fraction of $\eta_i\le y$ is the empirical fraction of $\xi_i\le F(y)$ and tends to $F(y)$. That is an empirical distribution statement, not a claim that the deterministic sequence consists of independent [random variables](../../../random-variable.md).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

One method applies [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) to the standard normal [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function): $Z_i=\Phi^{-1}(U_i)$, followed by $X_i=\mu+\sigma Z_i$ for mean $\mu$ and [standard deviation](../../../variance.md#standard-deviation) $\sigma>0$. Numerical approximations to $\Phi^{-1}$ are needed, and the endpoints $U=0,1$ must be avoided.

A convenient alternative is the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform). From independent uniforms $U_1,U_2\in(0,1)$ set

$$
R=\sqrt{-2\log U_1},\quad\Theta=2\pi U_2,\qquad
\boxed{Z_1=R\cos\Theta,\quad Z_2=R\sin\Theta.}
$$

The radial [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is $re^{-r^2/2}$ for $r>0$, and the angle is independently uniform on $[0,2\pi)$. Dividing their joint density by the polar-coordinate [Jacobian determinant](../../../calculus.md#jacobian-determinant) $r$ gives

$$
p(z_1,z_2)=\frac1{2\pi}e^{-(z_1^2+z_2^2)/2}
=\phi(z_1)\phi(z_2).
$$

Thus the outputs are independent standard [normal distribution](../../../probability-theory.md#normal-distribution) draws. Apply $\mu+\sigma Z_j$ to obtain other normal means and [variances](../../../variance.md). With finite [pseudorandom number generators](../../../probability-and-statistics.md#pseudorandom-number-generator), this is an approximation to the ideal independent-uniform model; poor dependence in the input stream is not cured by the transform.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $Y=h(U)$ have finite [variance](../../../variance.md) $v$ and mean $I$. An independent-sample [Monte Carlo estimator](../../../probability-and-statistics.md#monte-carlo-estimator) has [variance](../../../variance.md) $v/N$, so its root-mean-square random error is $\sqrt{v/N}$. Three techniques reduce the [variance](../../../variance.md) coefficient rather than changing this ordinary $N^{-1/2}$ rate.

For [antithetic variates](../../../probability-and-statistics.md#antithetic-variates), couple $Y=h(U)$ with $Y'=h(1-U)$ and average the pair. With $M$ independent pairs, the [variance](../../../variance.md) is $(v+\operatorname{Cov}(Y,Y'))/(2M)$, compared with $v/(2M)$ for $2M$ independent function evaluations. If $h$ is monotone in a scalar uniform, the [covariance](../../../variance.md#covariance) is nonpositive: for independent uniforms $U,V$,

$$
2\operatorname{Cov}(h(U),h(1-U))
=\mathbb E[(h(U)-h(V))(h(1-U)-h(1-V))]\le0.
$$

Opposite fluctuations therefore cancel. The reduction factor at equal evaluation count is $1+\rho$, where $\rho$ is the paired [correlation coefficient](../../../variance.md#pearson-correlation-coefficient); it can approach zero, but positive [covariance](../../../variance.md#covariance) would make the method worse. This is appropriate for monotone or otherwise negatively coupled payoffs, with cheap complementary paths.

For [control variates](../../../probability-and-statistics.md#control-variates), use a jointly simulated $C$ with known mean $m_C$ and average $Y-\beta(C-m_C)$. It remains an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) for fixed $\beta$, and

$$
\operatorname{Var}(Y-\beta C)=v-2\beta\operatorname{Cov}(Y,C)+\beta^2\operatorname{Var}C.
$$

Completing the square gives $\beta_*=\operatorname{Cov}(Y,C)/\operatorname{Var}C$ and minimal [variance](../../../variance.md) $v(1-\rho^2)$. For [contingent claim](../../../mathematical-finance.md#contingent-claim) simulation, an analytically priced related [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff), such as a simpler option or discounted terminal [stock](../../../mathematical-finance.md#stock), can be a useful control. It works best when correlation has large absolute value and simulation of the control adds little cost. A coefficient fixed from an independent pilot keeps the elementary unbiasedness argument valid; estimating it from the same sample can introduce finite-sample bias.

For [stratified sampling](../../../statistical-inference.md#stratified-sampling), partition the sampling space into strata $A_h$ of probabilities $p_h$, and independently simulate $N_h$ samples conditional on each stratum. The estimator $\sum_hp_h\bar Y_h$ is unbiased and has [variance](../../../variance.md)

$$
\sum_h\frac{p_h^2v_h}{N_h},\qquad v_h=\operatorname{Var}(Y\mid A_h).
$$

With proportional allocation $N_h=Np_h$, ignoring integer rounding, this equals $\sum_hp_hv_h/N$. The [law of total variance](../../../probability-theory.md#law-of-total-variance) shows the reduction from ordinary sampling is $\operatorname{Var}(\mathbb E[Y\mid A_h])/N$: fixed representation removes randomness in the stratum counts. At equal per-draw cost, minimizing the displayed [variance](../../../variance.md) gives $N_h\propto p_h\sqrt{v_h}$ and minimum $(\sum_hp_h\sqrt{v_h})^2/N$ for positive within-stratum [variances](../../../variance.md). This follows by [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and is useful when a low-dimensional coordinate strongly predicts the [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) and conditional simulation is easy.

**There is no universal ranking.** At comparable cost the [variance](../../../variance.md) factors depend respectively on paired [covariance](../../../variance.md#covariance), squared control correlation, and within-stratum variation. A nearly perfect control can outperform a weak antithetic pair; an appropriate stratification can be almost exact for a nearly stratum-constant [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff). Extra construction and sampling costs must be included in a fair accuracy comparison, and the methods can be combined.

## 5

↑ **Parent:** [Paper 23](paper-23.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) is defined by $f(t,T)=-\partial_T\log P(t,T)$, with $P(t,t)=1$. Integrating in maturity gives the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price and its diagonal [short rate](../../../mathematical-finance.md#short-rate):

$$
\boxed{P(t,T)=\exp\left(-\int_t^Tf(t,u)\,du\right),\qquad r_t=f(t,t).}
$$

The solution of the [continuous-time bank account](../../../mathematical-finance.md#continuous-time-bank-account) equation $dB_t=r_tB_tdt$, $B_0=1$, is $B_t=\exp(\int_0^tr_sds)$; the integration variable is time. Its discounted bond value is

$$
\boxed{Z_t(t,T)=B_t^{-1}P(t,T)
=\exp\left(-\int_0^tr_sds-\int_t^Tf(t,u)\,du\right).}
$$

All these are [adapted processes](../../../stochastic-process.md#adapted-process) when the [Heath-Jarrow-Morton model](../../../mathematical-finance.md#heath-jarrow-morton-model) coefficients are adapted and the integrals exist.

For [market completeness](../../../mathematical-finance.md#complete-market), stochastic integration over maturity gives

$$
d\log P(t,T)=\left[r_t-\int_t^T\alpha(t,u)\,du\right]dt+\Sigma(t,T)dW_t,\qquad
\Sigma(t,T)=-\int_t^T\sigma(t,u)\,du.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for the exponential then yields

$$
\frac{dP(t,T)}{P(t,T)}
=\left[r_t-\int_t^T\alpha(t,u)\,du+\frac12\Sigma(t,T)^2\right]dt+\Sigma(t,T)dW_t.
$$

Consequently under a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) the no-arbitrage drift restriction is

$$
\int_t^T\alpha^Q(t,u)\,du=\frac12\left(\int_t^T\sigma(t,u)\,du\right)^2,\qquad
\alpha^Q(t,T)=\sigma(t,T)\int_t^T\sigma(t,u)\,du.
$$

The last equality needs sufficient maturity regularity and has a positive sign despite the negative definition of $\Sigma$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Under the specified [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) and $d(B_t^{-1})=-r_tB_t^{-1}dt$ give

$$
d(B_t^{-1}P(t,T))=B_t^{-1}P(t,T)\Sigma(t,T)dW_t.
$$

Thus discounted traded [zero-coupon bonds](../../../mathematical-finance.md#zero-coupon-bond) have zero drift. Assume the usual integrability and admissibility conditions that make discounted replicating values true [martingales](../../../martingale.md), not merely [local martingales](../../../martingale.md#local-martingale). If $X$ is an attainable [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) with $\mathbb E_Q|B_T^{-1}X|<\infty$, its [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) value $V_t$ has terminal value $V_T=X$ and satisfies

$$
B_t^{-1}V_t=\mathbb E_Q[B_T^{-1}X\mid\mathcal F_t].
$$

Multiplying by $B_t$ yields

$$
\boxed{V_t=\mathbb E_Q\left[\exp\left(-\int_t^Tr_sds\right)X\mid\mathcal F_t\right].}
$$

This proves the requested conditional pricing formula. In a [Brownian filtration](../../../brownian-motion.md#brownian-filtration), the [Martingale representation theorem](../../../brownian-motion.md#martingale-representation-theorem) realizes the discounted conditional [expectation](../../../probability-theory.md#expected-value) as a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral). If an available bond has nonzero [Itô diffusion](../../../stochastic-calculus.md#ito-diffusion) exposure, its holdings can match that integral, with the remaining value in the [bank account](../../../mathematical-finance.md#bank-account), giving replication under the usual square-integrability conditions.

These attainability or [market completeness](../../../mathematical-finance.md#complete-market) hypotheses matter for a completely arbitrary [contingent claim](../../../mathematical-finance.md#contingent-claim): existence of a [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) alone need not imply a unique price for every unspanned [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff), and a zero-drift [local martingale](../../../martingale.md#local-martingale) alone need not satisfy the displayed terminal [expectation](../../../probability-theory.md#expected-value) identity. In the general path-dependent [Heath-Jarrow-Morton model](../../../mathematical-finance.md#heath-jarrow-morton-model), write the value as $V_t$; notation $V(t,r_t)$ is justified only when the current [short rate](../../../mathematical-finance.md#short-rate) is a sufficient state for the [financial payoff](../../../mathematical-finance.md#contingent-claim-payoff) and dynamics.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Suppose the forward field is differentiable in maturity with the stochastic integrability needed for differentiation. As time increases, both arguments of $r_t=f(t,t)$ increase. The [diagonal short-rate dynamics in the Heath-Jarrow-Morton model](../../../mathematical-finance.md#diagonal-short-rate-dynamics-in-the-heath-jarrow-morton-model) are therefore

$$
dr_t=[\partial_Tf(t,t)+\alpha^Q(t,t)]dt+\sigma(t,t)dW_t^Q.
$$

Under the HJM drift restriction from part (a), $\alpha^Q(t,t)=0$, giving

$$
\boxed{dr_t=\partial_Tf(t,t)\,dt+\sigma(t,t)dW_t^Q.}
$$

More explicitly the slope is

$$
\partial_Tf(t,t)=f_0'(t)+\int_0^t\partial_T\alpha^Q(s,t)\,ds
+\int_0^t\partial_T\sigma(s,t)\,dW_s^Q.
$$

It depends on the forward curve and potentially the whole history, not necessarily on $r_t$ alone. Without the stated maturity regularity, the original forward equations do not by themselves guarantee this classical [Itô process](../../../stochastic-calculus.md#ito-process) formula for the diagonal.

**The [short rate](../../../mathematical-finance.md#short-rate) need not be [Markov](../../../markov-process.md#markov-property), even with one Brownian factor and deterministic volatility.** An explicit example of [One Brownian factor does not imply a Markov short rate](../../../mathematical-finance.md#one-brownian-factor-does-not-imply-a-markov-short-rate) takes $f_0(T)=0$ and $\sigma(t,T)=T-t$. Its no-arbitrage forward drift is $\alpha^Q(t,T)=(T-t)^3/2$, so

$$
r_t=\frac{t^4}{8}+\int_0^t(t-s)dW_s
=\frac{t^4}{8}+I_t,\qquad I_t=\int_0^tW_sds.
$$

The continuous rate history determines $W_t$ from the left [derivative](../../../calculus.md#derivative) of $I_t$. Hence for $h>0$,

$$
\mathbb E[I_{t+h}\mid\mathcal F_t^r]=I_t+hW_t.
$$

But $W_t$ is not determined by $I_t$: joint normality, $\operatorname{Var}I_t=t^3/3$, and $\operatorname{Cov}(W_t,I_t)=t^2/2$ give

$$
\operatorname{Var}(W_t\mid I_t)=t-\frac{(t^2/2)^2}{t^3/3}=\frac t4>0.
$$

Thus the conditional mean of the future given the whole rate history cannot be a function of the current rate alone, contradicting the [Markov property](../../../markov-process.md#markov-property). Enlarging the state to $(I_t,W_t)$ gives a two-dimensional [Markov process](../../../markov-process.md); special HJM specifications can instead close on a single [short rate](../../../mathematical-finance.md#short-rate).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
