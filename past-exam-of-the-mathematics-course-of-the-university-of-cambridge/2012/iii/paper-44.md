# Paper 44

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_44.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_44.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [affine function](../../../vector-space.md#affine-function) preserves mixtures, so

$$
U_0(p\lambda+(1-p)\nu)-U_0(p\mu+(1-p)\nu)=p[U_0(\lambda)-U_0(\mu)]>0.
$$

Therefore

$$
\boxed{p\lambda+(1-p)\nu\succ p\mu+(1-p)\nu.}
$$

The positive mixture weight preserves the strict sign; the common component cancels. This is the [independence axiom for lottery preferences](../../../utility-function.md#independence-axiom-for-lottery-preferences) for the [affine utility on probability measures](../../../utility-function.md#affine-utility-on-probability-measures).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Indifference means equality of the representing utility values. Since $U_0(\lambda)>U_0(\mu)>U_0(\nu)$, set

$$
\boxed{p=\frac{U_0(\mu)-U_0(\nu)}{U_0(\lambda)-U_0(\nu)}\in(0,1).}
$$

Applying the [affine function](../../../vector-space.md#affine-function) identity gives $U_0(p\lambda+(1-p)\nu)=U_0(\mu)$, so $\mu\sim p\lambda+(1-p)\nu$. This proves [mixture solvability of affine preferences](../../../utility-function.md#mixture-solvability-of-affine-preferences). The displayed weight is unique because the two endpoint utilities differ.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

First, equality of two $U_0$ values forces equality of the corresponding $V_0$ values: neither strict comparison holds for $U_0$, and the same is then true for $V_0$ in both directions. Thus $V_0=g\circ U_0$ for a well-defined [strictly increasing function](../../../calculus.md#strictly-increasing-function) $g$ on $J=U_0(\mathcal P)$. Since $\mathcal P$ is a [convex set](../../../mathematical-optimization.md#convex-set) and $U_0,V_0$ are [affine functions](../../../vector-space.md#affine-function), $J$ is a [real interval](../../../real-analysis.md#interval-mathematics) and

$$
g(pu+(1-p)v)=pg(u)+(1-p)g(v),\qquad u,v\in J,\quad0\leq p\leq1.
$$

If $J$ contains $u<v$, let $a=[g(v)-g(u)]/(v-u)>0$ and $b=g(u)-au$. The mixture identity gives $g(w)=aw+b$ for $w\in[u,v]$. For $w>v$, express $v$ as a [convex combination](../../../mathematical-optimization.md#convex-combination) of $u$ and $w$ and solve the same identity for $g(w)$; for $w<u$, express $u$ as a mixture of $w$ and $v$. Hence the formula holds on all of $J$, not merely between the chosen anchors. We obtain [positive affine uniqueness of affine preference representations](../../../utility-function.md#positive-affine-uniqueness-of-affine-preference-representations):

$$
\boxed{V_0(\lambda)=aU_0(\lambda)+b\quad\text{for every }\lambda\in\mathcal P,\qquad a>0.}
$$

If $U_0$ is constant, the same comparisons force $V_0$ to be constant; choose $a=1$ and the appropriate $b$. If the probability-measure set is empty, the assertion is vacuous. These degenerate cases do not require distinct anchors.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Define $U(x)=U_0(\delta_x)$, where $\delta_x$ is the [Dirac measure](../../../measure-theory.md#dirac-measure) at $x$. For the full [sigma-algebra](../../../measure-theory.md#sigma-algebra) of subsets of a finite $E$, affineness directly gives $U_0(\lambda)=\sum_{x\in E}\lambda(\{x\})U(x)$.

The statement also holds for an arbitrary [sigma-algebra](../../../measure-theory.md#sigma-algebra) on a [finite set](../../../set.md#finite-set). List each [atom of a sigma-algebra](../../../measure-theory.md#atom-of-a-sigma-algebra) as $A_1,\ldots,A_r$ and choose $x_j\in A_j$. Points in one atom have identical [Dirac measures](../../../measure-theory.md#dirac-measure) on this [sigma-algebra](../../../measure-theory.md#sigma-algebra), so $U$ is constant on each atom and is measurable. Every [probability measure](../../../probability-theory.md#probability-measure) decomposes as $\lambda=\sum_j\lambda(A_j)\delta_{x_j}$, whence

$$
\boxed{U_0(\lambda)=\sum_j\lambda(A_j)U(x_j)=\int_EU(x)\,\lambda(dx).}
$$

This is the [expected utility representation on a finite measurable space](../../../utility-function.md#expected-utility-representation-on-a-finite-measurable-space). It does not silently assume that each singleton is measurable.

## 2

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Inada conditions](../../../utility-function.md#inada-conditions) give $U'(0+)=\infty$ and $U'(\infty)=0$. [Differentiability](../../../analysis.md#differentiability) and [strict concavity](../../../real-analysis.md#strict-concavity) make $U'$ continuous and strictly decreasing, with range $(0,\infty)$. Hence the [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility) $I=(U')^{-1}$ exists. The unique maximizer in the [utility conjugate](../../../convex-optimization.md#utility-conjugate) is $x=I(y)$, and

$$
\widehat U(y)=U(I(y))-yI(y),\qquad\boxed{\widehat U'(y)=-I(y).}
$$

The [derivative](../../../calculus.md#derivative) formula does not require [differentiability](../../../analysis.md#differentiability) of $I$: compare the optimizing values at $y$ and $y+h$ to squeeze the [difference quotient](../../../calculus.md#difference-quotient) between $-I(y)$ and $-I(y+h)$, and use [continuity](../../../calculus.md#continuous-function) of $I$. Thus the dual is continuously differentiable, strictly decreasing, and [strictly convex](../../../real-analysis.md#strictly-convex-function), since $-I$ is strictly increasing.

For the requested second-derivative assertion, a curvature hypothesis is missing. Under the intended nondegeneracy $U''(x)<0$ for every $x>0$, inverse differentiation gives

$$
\boxed{\widehat U''(y)=-\frac1{U''(I(y))}>0,\qquad U''(x)\widehat U''(U'(x))=-1.}
$$

This proves the intended [dual differentiability with nonvanishing utility curvature](../../../convex-optimization.md#dual-differentiability-with-nonvanishing-utility-curvature). If $U$ is only twice differentiable, it gives pointwise twice [differentiability](../../../analysis.md#differentiability) of the dual; continuous second [derivatives](../../../calculus.md#derivative) additionally follow when $U\in C^2$.

Literal [strict concavity](../../../real-analysis.md#strict-concavity) does not imply nonvanishing curvature. An explicit [Inada utility with vanishing curvature](../../../utility-function.md#inada-utility-with-vanishing-curvature) is

$$
U(x)=\log x+\frac1x-\frac1{6x^2},\quad U'(x)=\frac1x-\frac1{x^2}+\frac1{3x^3},\quad U''(x)=-\frac{(x-1)^2}{x^4}.
$$

Its [derivative](../../../calculus.md#derivative) is positive, strictly decreasing, tends to infinity at zero and to zero at infinity. It is smooth and [strictly concave](../../../real-analysis.md#strictly-concave-function), but $U''(1)=0$. At $y_0=U'(1)=1/3$, a finite [derivative](../../../calculus.md#derivative) of $I$ would contradict differentiation of $U'(I(y))=y$, giving $0\cdot I'(y_0)=1$. Hence $\widehat U'$ is not differentiable there. **As printed, the twice-differentiable-dual claim is false; it is valid with $U''<0$.** The remaining [differentiability](../../../analysis.md#differentiability), monotonicity and strict-convexity conclusions above hold under the printed hypotheses.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Admissible terminal wealth must lie in $(0,\infty)$, the domain of the utility; alternatively extend $U$ by $-\infty$ outside that domain. A one-period [state-price density](../../../mathematical-finance.md#state-price-density) has $Z>0$ and $\mathbb E[ZP_1]=P_0$, componentwise. Therefore for $W=H\cdot P_1$, $\mathbb E[ZW]=H\cdot P_0=x$.

The dual definition gives the pointwise inequality $U(w)\leq\widehat U(z)+zw$ for $w,z>0$. Apply it with $z=yZ$ and take [expectations](../../../probability-theory.md#expected-value) on the finite state space:

$$
\boxed{\mathbb E U(H\cdot P_1)\leq\mathbb E\widehat U(yZ)+yx.}
$$

Equality holds precisely when $U'(w)=z$, because that is the unique maximizing payoff in the dual definition. If the feasible [portfolio](../../../mathematical-finance.md#investment-portfolio) $H^*$ has $U'(H^*\cdot P_1)=y^*Z^*$, then

$$
\mathbb E U(H^*\cdot P_1)=\mathbb E\widehat U(y^*Z^*)+y^*x.
$$

The same right side bounds every competing feasible [portfolio](../../../mathematical-finance.md#investment-portfolio). Thus **$H^*$ is optimal.** This is the [one-period marginal-utility certificate of optimality](../../../utility-function.md#one-period-marginal-utility-certificate-of-optimality); it does not require the erroneous second-differentiability assertion in part (a).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $z_u,z_d$ be the state-price-density values at the higher and lower risky payoff. Pricing the two assets gives

$$
\tfrac12\,6(z_u+z_d)=5,\qquad\tfrac12(7z_u+4z_d)=5.
$$

Solving yields

$$
\boxed{Z=\begin{cases}10/9&S_1=7,\\5/9&S_1=4.\end{cases}}
$$

Both values are positive, and the two independent equations make the solution unique. The payoff matrix has nonzero determinant, so this is a [complete two-state market](../../../mathematical-finance.md#complete-two-state-market). The actual [Arrow state prices](../../../mathematical-finance.md#arrow-debreu-state-price), including physical probabilities, are $q_u=5/9$ and $q_d=5/18$. Their sum is $5/6$, the [discount factor](../../../mathematical-finance.md#discount-factor). Normalizing gives [risk-neutral probabilities](../../../mathematical-finance.md#risk-neutral-probability) $2/3,1/3$. Thus $Z$ itself is not a probability density of mean one: its mean is $5/6$ because the riskless asset earns interest.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The stated [portfolio](../../../mathematical-finance.md#investment-portfolio) has initial wealth $5$ and terminal payoffs $W_u=4\cdot6-3\cdot7=3$ and $W_d=4\cdot6-3\cdot4=12$. For [CRRA utility](../../../utility-function.md#constant-relative-risk-aversion-utility), $U'(w)=w^{-R}$. The market is complete, and an interior optimum in its positive payoff domain has marginal utility proportional to the unique [state-price density](../../../mathematical-finance.md#state-price-density). Therefore

$$
\frac{3^{-R}}{12^{-R}}=\frac{10/9}{5/9}=2,\qquad4^R=2,\qquad\boxed{R=\frac12.}
$$

The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) is $y^*=9/(10\sqrt3)$, and both state equations $U'(W)=y^*Z$ are satisfied. Part (b) verifies sufficiency and [strict concavity](../../../real-analysis.md#strict-concavity) gives uniqueness of the optimal payoff. This illustrates [risk aversion recovered from an optimal two-state payoff](../../../utility-function.md#risk-aversion-recovered-from-an-optimal-two-state-payoff).

## 3

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $\beta_t$ be the cash position and $\pi_t$ the risky shares chosen using information at $t-1$. At the start of the period the [portfolio](../../../mathematical-finance.md#investment-portfolio) costs $\beta_t+\pi_tS_{t-1}=X_{t-1}$. With cash price fixed at one, its ending value is $\beta_t+\pi_tS_t$. Rebalancing cannot add or remove wealth under a [self-financing strategy](../../../mathematical-finance.md#self-financing-portfolio), so

$$
\boxed{X_t=X_{t-1}+\pi_t(S_t-S_{t-1}).}
$$

The holdings are [predictable](../../../martingale.md#predictable-process): they are chosen before the current price increment is observed. This is the [discounted wealth equation in discrete time](../../../mathematical-finance.md#discounted-wealth-equation-in-discrete-time) with cash as [numéraire](../../../mathematical-finance.md#numeraire).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Take the nondegenerate case $\sigma>0$ and an integer trading horizon $T$. For [exponential utility](../../../utility-function.md#constant-absolute-risk-aversion-utility), maximize the negative of the exponential loss, equivalently minimize its [expectation](../../../probability-theory.md#expected-value). Conditional on past information, a [predictable](../../../martingale.md#predictable-process) choice $\pi$ has

$$
\mathbb E[e^{-\gamma\pi\Delta S_t}\mid\mathcal F_{t-1}]=\exp\left(-\gamma\mu\pi+\tfrac12\gamma^2\sigma^2\pi^2\right).
$$

Complete the square:

$$
-\gamma\mu\pi+\tfrac12\gamma^2\sigma^2\pi^2=\tfrac12\gamma^2\sigma^2\left(\pi-\frac\mu{\gamma\sigma^2}\right)^2-\frac{\mu^2}{2\sigma^2}.
$$

Thus the minimum conditional multiplier is $e^{-\kappa}$ with $\kappa=\mu^2/(2\sigma^2)$. [Backward induction](../../../foundations-of-mathematics.md#backward-induction) starts with terminal loss $e^{-\gamma x}$ and gives the minimal continuation loss $e^{-\gamma x-\kappa(T-t)}$. [Independence](../../../random-variable.md#independent-random-variables) of the next increment justifies the same conditional minimization for every history, not just deterministic trading plans. Hence [exponential-utility trading with Gaussian increments](../../../mathematical-finance.md#exponential-utility-trading-with-gaussian-increments) gives

$$
\boxed{\pi_t^*=\frac\mu{\gamma\sigma^2},\quad1\leq t\leq T,\qquad V_0(x)=-\exp\left(-\gamma x-\frac{T\mu^2}{2\sigma^2}\right).}
$$

These are constant numbers of shares, not constant wealth fractions. Strategies with infinite exponential loss have expected utility $-\infty$ and cannot improve this finite value. If $\sigma=0$, the usual formula is inapplicable: with $\mu=0$ trading has no effect, while a nonzero deterministic increment admits unbounded riskless gains and no finite maximizing position.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a [predictable](../../../martingale.md#predictable-process) position $\pi$, the current net wealth increment $\pi\Delta S_t+Y_t-y$ is conditionally [Gaussian](../../../probability-theory.md#normal-distribution) with mean $\pi\mu+a-y$ and [variance](../../../variance.md) $\pi^2\sigma^2+2\pi\rho b\sigma+b^2$. Its exponential-loss multiplier is

$$
\exp\left[-\gamma(\pi\mu+a-y)+\tfrac12\gamma^2(\pi^2\sigma^2+2\pi\rho b\sigma+b^2)\right].
$$

Differentiate its quadratic exponent. The unique minimizing position is

$$
\boxed{\pi_t^{\mathrm{swap}}=\frac\mu{\gamma\sigma^2}-\frac{\rho b}{\sigma},\quad1\leq t\leq T.}
$$

The first term is the speculative demand; the second offsets the part of the income correlated with the tradable price increment. Independent period vectors and [backward induction](../../../foundations-of-mathematics.md#backward-induction) justify using this same position at every date. Completing the square gives minimal exponent $-\kappa-\gamma d(y)$, where

$$
d(y)=a-y-\frac{\mu\rho b}{\sigma}-\frac\gamma2b^2(1-\rho^2).
$$

Therefore [hedging a Gaussian income stream with exponential utility](../../../mathematical-finance.md#hedging-a-gaussian-income-stream-with-exponential-utility) has value

$$
\boxed{V_0^{\mathrm{swap}}(x;y)=-\exp[-\gamma x-T\kappa-\gamma T d(y)].}
$$

The residual [variance](../../../variance.md) is $b^2(1-\rho^2)$; it disappears for perfectly correlated income.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let

$$
\boxed{\overline y=a-\frac{\mu\rho b}{\sigma}-\frac\gamma2b^2(1-\rho^2).}
$$

Part (c) has $d(y)=\overline y-y$. Comparing the optimized values with and without the contract, $V_0^{\mathrm{swap}}=-e^{-\gamma x-T\kappa-\gamma T(\overline y-y)}$ and $V_0=-e^{-\gamma x-T\kappa}$, shows that $y>\overline y$ makes the swap value strictly more negative. Thus **The investor prefers not to enter when $y>\overline y$.** He is indifferent at equality and prefers entry for a smaller payment.

The [periodic utility indifference payment for Gaussian income](../../../utility-function.md#periodic-utility-indifference-payment-for-gaussian-income) equals the mean income less the cost of hedging its correlated component and the exponential-utility penalty for the residual unhedgeable [variance](../../../variance.md). Comparing unoptimized strategies would not justify this price threshold.

## 4

↑ **Parent:** [Paper 44](paper-44.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The marked-to-market value of the current holdings is $X_t=H_t\cdot P_t$. In a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio), purchases are paid for by sales within the [portfolio](../../../mathematical-finance.md#investment-portfolio), so rebalancing itself changes no net wealth. Asset price changes contribute $H_t\cdot dP_t$, and nonnegative [consumption](../../../mathematical-finance.md#consumption) removes $c_t\,dt$ from wealth. Hence

$$
\boxed{X_t=H_t\cdot P_t,\qquad dX_t=H_t\cdot dP_t-c_t\,dt.}
$$

The holdings must be [predictable](../../../martingale.md#predictable-process) and stochastically integrable. The second identity is the self-financing definition with withdrawals; it is not obtained by incorrectly setting the changes in the holdings themselves to zero.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Apply the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) and the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) rule for a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral). The [finite variation](../../../real-analysis.md#total-variation-of-a-function) [consumption](../../../mathematical-finance.md#consumption) term has zero [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) with $Z$, so

$$
d[Z,X]_t=\sum_iH_t^i\,d[Z,P^i]_t.
$$

Using $X=H\cdot P$ and the wealth equation,

$$
\begin{aligned}d(ZX)&=Z\,dX+X\,dZ+d[Z,X]\\&=H\cdot(Z\,dP+P\,dZ+d[Z,P])-Zc\,dt.
\end{aligned}
$$

Thus the [deflated wealth equation with consumption](../../../mathematical-finance.md#deflated-wealth-equation-with-consumption) is

$$
\boxed{d(Z_tX_t)=H_t\cdot d(Z_tP_t)-Z_tc_t\,dt.}
$$

No [finite variation](../../../real-analysis.md#total-variation-of-a-function) assumption on $H$ is needed: the self-financing equation and the stochastic-integral [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) rule already incorporate the [portfolio](../../../mathematical-finance.md#investment-portfolio)'s financing constraint.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use the usual normalization $Z_0=1$, finite deterministic initial wealth $x=X_0\geq0$, positive [state-price density](../../../mathematical-finance.md#state-price-density), and nonnegative [consumption](../../../mathematical-finance.md#consumption). The deflated asset prices $ZP$ are local [martingales](../../../martingale.md), so [predictable](../../../martingale.md#predictable-process) stochastic integrability makes $M=\int H\cdot d(ZP)$ a zero-starting [local martingale](../../../martingale.md#local-martingale). Integrating part (b) gives

$$
N_t:=x+M_t=Z_tX_t+\int_0^tZ_sc_s\,ds\geq0.
$$

A nonnegative [local martingale](../../../martingale.md#local-martingale) is a [supermartingale](../../../martingale.md#supermartingale): localize to [martingales](../../../martingale.md), apply [Conditional Fatou lemma](../../../measure-theory.md#conditional-fatou-lemma), and obtain the [conditional expectation](../../../measure-theory.md#conditional-expectation) inequality and integrability. Therefore $N$, and hence $M=N-x$, are [supermartingales](../../../martingale.md#supermartingale). In particular,

$$
\boxed{\mathbb E[M_t\mid\mathcal F_s]\leq M_s,\qquad s\leq t.}
$$

This is [supermartingale control of deflated consumption gains](../../../mathematical-finance.md#supermartingale-control-of-deflated-consumption-gains). Nonnegative [consumption](../../../mathematical-finance.md#consumption) is essential to the lower bound; it is the ordinary meaning of a [consumption](../../../mathematical-finance.md#consumption) rate here. Wealth nonnegativity alone would not supply that bound if arbitrary signed cash flows were allowed.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [supermartingale](../../../martingale.md#supermartingale) conclusion gives

$$
\mathbb E\left[Z_tX_t+\int_0^tZ_sc_s\,ds\right]\leq x.
$$

Discard the nonnegative terminal-wealth term and let $t\to\infty$. The cumulative deflated [consumption](../../../mathematical-finance.md#consumption) increases, so [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) yields the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint)

$$
\boxed{\mathbb E\int_0^\infty Z_tc_t\,dt\leq X_0.}
$$

The normalization is relevant: with $Z_0\ne1$ the right side is $Z_0X_0$; with random integrable initial deflated wealth its [expectation](../../../probability-theory.md#expected-value) is the unconditional budget bound.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Write $D=\mathbb E\int_0^\infty e^{-bt/R}Z_t^{1-1/R}\,dt$ and use the [product measure](../../../probability-theory.md#product-measure) $d\mathbb P\,dt$. For $0<R<1$, the [conjugate exponents](../../../functional-analysis.md#conjugate-exponents) are $p=1/(1-R)$ and $q=1/R$. Factor the utility integrand as

$$
e^{-bt}c_t^{1-R}=(Z_tc_t)^{1-R}\bigl(e^{-bt}Z_t^{R-1}\bigr).
$$

The [Holder inequality](../../../functional-analysis.md#holder-inequality) on this [product measure](../../../probability-theory.md#product-measure) gives

$$
\mathbb E\int_0^\infty e^{-bt}c_t^{1-R}\,dt\leq\left(\mathbb E\int_0^\infty Z_tc_t\,dt\right)^{1-R}D^R\leq X_0^{1-R}D^R.
$$

Divide by $1-R$ to obtain the [Hölder bound for discounted CRRA consumption](../../../mathematical-finance.md#holder-bound-for-discounted-crra-consumption):

$$
\boxed{\mathbb E\int_0^\infty e^{-bt}U(c_t)\,dt\leq U(X_0)\left[\mathbb E\int_0^\infty e^{-bt/R}Z_t^{1-1/R}\,dt\right]^R.}
$$

For a finite right side this is ordinary Hölder; on the infinite measure space one can first truncate time and then pass by [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem). If $D=\infty$ and $X_0>0$, the bound is valid but uninformative. If $X_0=0$, the budget forces $c=0$ almost everywhere, so the utility integral is zero; handle this separately instead of writing an undefined $0\cdot\infty$.

When $D$ is finite and the bound is attained, equality requires full budget use and $c_t=(X_0/D)e^{-bt/R}Z_t^{-1/R}$. This is the equality pattern of Hölder, not an assertion that every market can finance that process.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
