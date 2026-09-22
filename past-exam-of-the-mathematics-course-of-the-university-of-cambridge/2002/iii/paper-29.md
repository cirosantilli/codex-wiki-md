# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper29.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Normalize the riskless [financial asset](../../../mathematical-finance.md#financial-asset) to $B_0=1$, $B_1=b>0$, and write $S_0,S_1$ for the $s$ risky asset prices. Their discounted gain [random vector](../../../random-variable.md#random-vector) is $Y=S_1/b-S_0$. A zero-cost [portfolio](../../../mathematical-finance.md#investment-portfolio) holding $h\in\mathbb R^s$ in the risky assets and $-h\cdot S_0$ in the riskless asset has terminal value $b\,h\cdot Y$. Thus an [arbitrage](../../../mathematical-finance.md#arbitrage) means

$$
h\cdot Y\geq0\quad\text{almost surely},\qquad \mathbb P(h\cdot Y>0)>0.
$$

An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) is a [probability measure](../../../probability-theory.md#probability-measure) $Q$ with the same [null sets](../../../measure-theory.md#null-set) as $P$, under which $Y$ is [integrable](../../../measure-theory.md#integrability) and $\mathbb E_QY=0$. The discounted risky prices are then [martingales](../../../martingale.md) over the single trading period.

If such $Q$ exists, a nonnegative terminal gain has [expectation](../../../probability-theory.md#expected-value) zero under $Q$. A nonnegative [random variable](../../../random-variable.md) with zero [expectation](../../../probability-theory.md#expected-value) vanishes [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence): on $\{X\geq1/n\}$ its [expectation](../../../probability-theory.md#expected-value) is at least $\mathbb P(X\geq1/n)/n$, and the union of these events is $\{X>0\}$. Equivalence transfers this conclusion to $P$, excluding [arbitrage](../../../mathematical-finance.md#arbitrage).

For the converse we prove the needed [positive-density separation proof of the one-period asset-pricing theorem](../../../mathematical-finance.md#positive-density-separation-proof-of-the-one-period-asset-pricing-theorem). First make the gain [integrable](../../../measure-theory.md#integrability) without changing its [null sets](../../../measure-theory.md#null-set). Define an [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure) $P_0$ by

$$
\frac{dP_0}{dP}=\frac{k}{1+\|Y\|},\qquad
k^{-1}=\mathbb E_P\frac1{1+\|Y\|}.
$$

Let $N=\{h:h\cdot Y=0\text{ almost surely}\}$ and let $L=N^\perp$ be its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). Taking a finite [basis](../../../vector-space.md#basis) of $N$ shows $Y\in L$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). If $L=\{0\}$, the gain is zero and $P_0$ already gives the required measure. Otherwise consider the [positive-weight expectation cone](../../../mathematical-optimization.md#positive-weight-expectation-cone)

$$
C=\{\mathbb E_{P_0}[ZY]: Z\text{ bounded and }Z>0\text{ almost surely}\}\subset L.
$$

Positive combinations of weights show that $C$ is a [convex cone](../../../mathematical-optimization.md#convex-cone). It is open relative to $L$. Indeed, for any admissible weight $Z$, perturb it to

$$
Z_\varepsilon=Z\left(1+\frac{\varepsilon\cdot Y}{1+\|Y\|}\right),\qquad \varepsilon\in L,\quad \|\varepsilon\|<1.
$$

These weights remain bounded and strictly positive, while

$$
\mathbb E_{P_0}[Z_\varepsilon Y]=\mathbb E_{P_0}[ZY]+A_Z\varepsilon,
\qquad A_Z=\mathbb E_{P_0}\frac{ZYY^T}{1+\|Y\|}.
$$

For every nonzero $v\in L$, $v\cdot Y$ is nonzero on an event of positive [probability](../../../probability-theory.md#probability); otherwise $v\in N\cap L$. Consequently

$$
v^TA_Zv=\mathbb E_{P_0}\frac{Z(v\cdot Y)^2}{1+\|Y\|}>0.
$$

The [matrix](../../../vector-space.md#matrix) is finite because $\|Y\|^2/(1+\|Y\|)\leq\|Y\|$. The [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $A_Z$ on $L$ is zero, so it defines an [invertible matrix](../../../linear-algebra.md#invertible-matrix) on the [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) $L$. For any sufficiently small $\delta>0$, every $y$ with $\|y\|<\delta/\|A_Z^{-1}\|$ is the image of a vector in the radius-$\delta$ ball, since $\|A_Z^{-1}y\|<\delta$. Hence the perturbations give a [neighborhood](../../../topology.md#neighbourhood-mathematics) of zero, proving relative openness of $C$.

If $0\notin C$, the [hyperplane separation theorem](../../../mathematical-optimization.md#hyperplane-separation-theorem) gives a nonzero $h\in L$ with $h\cdot c\geq0$ for every $c\in C$. The separating constant can be taken to be zero because $C$ is a cone. Put $A=\{h\cdot Y<0\}$ and use the strictly positive weights $Z=\mathbf1_A+\varepsilon$. Taking the [limit](../../../calculus.md#limit-of-a-function) as $\varepsilon\downarrow0$ yields $\mathbb E_{P_0}[(h\cdot Y)\mathbf1_A]\geq0$, forcing $P_0(A)=0$. But $h\notin N$, so $P_0(h\cdot Y>0)>0$. This is an [arbitrage](../../../mathematical-finance.md#arbitrage), a contradiction. Hence $0\in C$: some bounded strictly positive $Z$ satisfies $\mathbb E_{P_0}[ZY]=0$. Normalize it by $dQ/dP_0=Z/\mathbb E_{P_0}Z$. This gives an [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) with [integrable](../../../measure-theory.md#integrability) gains, establishing the [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) here without any further existence theorem.

Now retain only the $m$ positive-probability states of the finite [probability space](../../../probability-theory.md#probability-space). Let $V\subseteq\mathbb R^m$ be the [linear span](../../../vector-space.md#linear-span) of the discounted terminal asset payoffs; it contains the constant vector $\mathbf1$. A [complete market](../../../mathematical-finance.md#complete-market) means $V=\mathbb R^m$. An [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure) is a vector $q$ of strictly positive state probabilities whose pairing with each asset payoff gives its initial price. By linearity it prices every attainable payoff. If $V=\mathbb R^m$, the [indicator functions](../../../measure-theory.md#indicator-function) of individual states are attainable, so these prices determine every $q_j$ uniquely.

If $V$ is proper, choose $0\ne v\in V^\perp$. Since $\mathbf1\in V$, $\sum_jv_j=0$. For sufficiently small $\varepsilon>0$, both $q+\varepsilon v$ and $q-\varepsilon v$ have strictly positive entries, sum to one, and give the same pairings with every asset payoff. They are distinct [equivalent martingale measures](../../../mathematical-finance.md#risk-neutral-measure). Therefore [market completeness](../../../mathematical-finance.md#complete-market) is equivalent to uniqueness of the [equivalent martingale measure](../../../mathematical-finance.md#risk-neutral-measure).

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Take bank-account values $B_k=R^k$ with $R>0$, and let the [stock](../../../mathematical-finance.md#stock) multiply independently by $u$ or $d$ at each step, where $0<d<R<u$. Under the physical [probability measure](../../../probability-theory.md#probability-measure) $P$, the up probability is $p\in(0,1)$; the [filtration](../../../stochastic-process.md#filtration-probability-theory) records the successive moves. These assumptions specify the standard [binomial market](../../../mathematical-finance.md#discrete-time-binomial-market). If $R$ lies outside the strict interval $(d,u)$, a long or short stock position financed through the [bank account](../../../mathematical-finance.md#bank-account) gives an [arbitrage](../../../mathematical-finance.md#arbitrage).

The [risk-neutral probability in a binomial market](../../../mathematical-finance.md#risk-neutral-probability-in-a-binomial-market) is fixed by $qu+(1-q)d=R$, giving

$$
\boxed{q=\frac{R-d}{u-d}\in(0,1).}
$$

For successor claim values $V_u,V_d$ at a node with current stock price $S$, solve the two replication equations. The current stock holding and current cash value are

$$
\Delta=\frac{V_u-V_d}{S(u-d)},\qquad
C=\frac{uV_d-dV_u}{R(u-d)}.
$$

The cost of this [replicating portfolio in a binomial market](../../../mathematical-finance.md#replicating-portfolio-in-a-binomial-market) is

$$
\Delta S+C=\frac{qV_u+(1-q)V_d}{R}.
$$

Apply this [backward option pricing](../../../mathematical-finance.md#backward-option-pricing) recursion from any terminal [contingent claim](../../../mathematical-finance.md#contingent-claim) $H$, including claims depending on the whole sequence of moves. It constructs a [self-financing portfolio](../../../mathematical-finance.md#self-financing-portfolio) and proves [market completeness](../../../mathematical-finance.md#complete-market) by induction on the remaining number of periods. Taking successive [conditional expectations](../../../measure-theory.md#conditional-expectation) under the measure $Q$ with independent up probability $q$ gives the unique [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) value

$$
V_k=R^{-(n-k)}\mathbb E_Q[H\mid\mathcal F_k].
$$

Any other price would give an [arbitrage](../../../mathematical-finance.md#arbitrage) by buying the cheaper of the claim and its replica and selling the dearer.

If $K$ is the number of up moves, a particular path has probabilities $p^K(1-p)^{n-K}$ under $P$ and $q^K(1-q)^{n-K}$ under $Q$. Therefore the [binomial-market probability density](../../../mathematical-finance.md#binomial-market-probability-density), namely the [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative), is

$$
\boxed{Z=\frac{dQ}{dP}=\left(\frac qp\right)^K\left(\frac{1-q}{1-p}\right)^{n-K},\qquad
K=\frac{\log(S_n/(S_0d^n))}{\log(u/d)}.}
$$

This last expression makes $Z$ a function of the terminal [stock](../../../mathematical-finance.md#stock) price. Summing over paths gives $\mathbb E_PZ=1$, and strict positivity proves equivalence of the two [probability measures](../../../probability-theory.md#probability-measure).

For unrestricted terminal [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) $H$, its initial replication cost is $R^{-n}\mathbb E_QH$. Hence feasible wealth satisfies the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) $\mathbb E_QH=R^nw_0$. For the stated [exponential utility](../../../utility-function.md#constant-absolute-risk-aversion-utility), $v'(x)=e^{-ax}$ and $v''(x)=-ae^{-ax}<0$. The [binomial exponential-utility terminal wealth](../../../utility-function.md#binomial-exponential-utility-terminal-wealth) is

$$
\boxed{H^*=R^nw_0+\frac{\mathbb E_Q\log Z-\log Z}{a},}
$$

where

$$
\mathbb E_Q\log Z
=n\left[q\log\frac qp+(1-q)\log\frac{1-q}{1-p}\right].
$$

It satisfies the budget, and its [marginal utility](../../../utility-function.md#marginal-utility) is $v'(H^*)=\lambda Z$ with $\lambda=\exp(-aR^nw_0-\mathbb E_Q\log Z)>0$. The [concave supporting-tangent inequality](../../../real-analysis.md#concave-supporting-tangent-inequality) gives

$$
v(H)\leq v(H^*)+\lambda Z(H-H^*).
$$

Taking [expectations](../../../probability-theory.md#expected-value) under $P$ makes the last term zero by the budget. Strict [concavity](../../../real-analysis.md#concave-function) makes equality possible only when $H=H^*$ in every positive-probability state. The already constructed [complete market](../../../mathematical-finance.md#complete-market) supplies its [replicating strategy](../../../mathematical-finance.md#replicating-strategy), so this proves global optimality and uniqueness. The formula allows negative final wealth, as permitted by the unrestricted trading problem.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $\phi_T(y)=(2\pi T)^{-1/2}e^{-y^2/(2T)}$ be the [normal distribution](../../../probability-theory.md#normal-distribution) density. The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives the killed endpoint density

$$
\mathbb P(W_T\in dy,\ \sup_{s\leq T}W_s<a)
=[\phi_T(y)-\phi_T(y-2a)]\,dy,\qquad y<a.
$$

Indeed, reflection after the first hit of $a$ maps paths ending below $a$ that have hit the barrier to paths ending at $2a-y$; symmetry gives $\phi_T(2a-y)=\phi_T(y-2a)$.

By the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), weighting the path law by $\exp(\nu W_T-\nu^2T/2)$ makes the coordinate process a [Brownian motion with drift](../../../brownian-motion.md#brownian-motion-with-drift) $\nu$. Completing the two squares yields

$$
e^{\nu y-\nu^2T/2}[\phi_T(y)-\phi_T(y-2a)]
=\phi_T(y-\nu T)-e^{2a\nu}\phi_T(y-2a-\nu T).
$$

Integration up to $x\leq a$ proves the [joint endpoint and maximum law for drifted Brownian motion](../../../brownian-motion.md#joint-endpoint-and-maximum-law-for-drifted-brownian-motion):

$$
\boxed{\mathbb P(W_T^\nu\leq x,M_T^\nu<a)
=\Phi\left(\frac{x-\nu T}{\sqrt T}\right)
-e^{2a\nu}\Phi\left(\frac{x-2a-\nu T}{\sqrt T}\right).}
$$

Here $\Phi$ is the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). Setting $x=a$ also gives a continuous barrier distribution, so equality at the barrier has zero [probability](../../../probability-theory.md#probability).

For the [up-and-in option](../../../mathematical-finance.md#up-and-in-claim), use the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) of the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) with [interest rate](../../../mathematical-finance.md#interest-rate) $\rho$ and [spot volatility](../../../mathematical-finance.md#spot-volatility) $\sigma>0$. Then

$$
S_t=S_0e^{\sigma(W_t+\nu t)},\qquad
\nu=\frac{\rho-\sigma^2/2}{\sigma},\qquad
a=\frac{\log(b/S_0)}{\sigma}>0.
$$

Above $a$, the barrier has certainly been reached. Below $a$, subtracting the killed density from the unrestricted endpoint density leaves $e^{2a\nu}\phi_T(y-2a-\nu T)$. Thus the discounted [expected value](../../../probability-theory.md#expected-value) of its payoff is

$$
e^{-\rho T}\left[\int_a^\infty f(S_0e^{\sigma y})\phi_T(y-\nu T)\,dy
+e^{2a\nu}\int_{-\infty}^a f(S_0e^{\sigma y})\phi_T(y-2a-\nu T)\,dy\right].
$$

In the second integral put $z=y-2a$, and define

$$
\boxed{\kappa=e^{-2\sigma a}=\left(\frac{S_0}{b}\right)^2.}
$$

Then $S_0e^{\sigma y}=S_0e^{\sigma z}/\kappa$, $z\leq-a$ means $S_0e^{\sigma z}\leq\kappa b$, and $e^{2a\nu}=\kappa^{-\nu/\sigma}$. Both integrals now use the unrestricted terminal [stock](../../../mathematical-finance.md#stock) distribution. This proves that the [reflected European payoff for an up-and-in option](../../../mathematical-finance.md#reflected-european-payoff-for-an-up-and-in-option) is

$$
\boxed{g(x)=f(x)\mathbf1_{\{x>b\}}+\kappa^{-\nu/\sigma}f(x/\kappa)\mathbf1_{\{x\leq\kappa b\}}.}
$$

Their initial [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) values agree for payoffs with finite absolute expectations in these integrals. The identity concerns prices; the two terminal payoffs need not agree along individual paths.

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $T=t_0$, $B_t=e^{-\rho(T-t)}$, and let $V_t=f(S_t,t)$ with $f(x,t)=xg(x,t)+B_th(x,t)$. The [portfolio](../../../mathematical-finance.md#investment-portfolio) holds $g(S_t,t)$ shares of [stock](../../../mathematical-finance.md#stock) and $h(S_t,t)$ units of the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond). It is [self-financing](../../../mathematical-finance.md#self-financing-portfolio) when all changes of holdings are funded within it, which is the gain identity

$$
dV_t=g(S_t,t)\,dS_t+h(S_t,t)\,dB_t.
$$

Under the physical [probability measure](../../../probability-theory.md#probability-measure), write $dS_t=\mu S_tdt+\sigma S_tdW_t$, where $\sigma>0$ and $dB_t=\rho B_tdt$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
df(S_t,t)=\left(f_t+\mu S_tf_x+\frac12\sigma^2S_t^2f_{xx}\right)dt
+\sigma S_tf_x\,dW_t.
$$

Matching the [Brownian motion](../../../brownian-motion.md) coefficients forces $f_x=g$. Since $f_x=g+xg_x+B_th_x$, this is precisely

$$
xg_x+B_th_x=0.
$$

Differentiating $f_x=g$ gives $f_{xx}=g_x$. Since $f_t=xg_t+\rho B_th+B_th_t$, matching the [drift](../../../stochastic-calculus.md#drift-coefficient) coefficients now gives

$$
xg_t+B_th_t+\frac12\sigma^2x^2g_x=0.
$$

These are the [self-financing conditions for smooth stock and bond holdings](../../../mathematical-finance.md#self-financing-conditions-for-smooth-stock-and-bond-holdings). Conversely, substituting both identities into the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives the gain identity, so they are sufficient as well. Smoothness and the positive [lognormal distribution](../../../probability-theory.md#log-normal-distribution) density of $S_t$ extend the identities along the price process to every $x>0$, with boundary times obtained by continuity.

The [portfolio with constant stock value in bond units](../../../mathematical-finance.md#portfolio-with-constant-stock-value-in-bond-units) must have $xg(x,t)=\theta B_t$, so $g(x,t)=\theta B_t/x$. The first condition then gives $h_x=\theta/x$, hence

$$
h(x,t)=\theta\log(x/S_0)+c(t).
$$

The second condition reduces to $c'(t)=\theta(\sigma^2/2-\rho)$. Initial [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) requires $h(S_0,0)=w_0/B_0-\theta=w_0e^{\rho T}-\theta$. Therefore the holdings are

$$
\boxed{g(x,t)=\frac{\theta e^{-\rho(T-t)}}x,\qquad
h(x,t)=w_0e^{\rho T}-\theta+\theta\log(x/S_0)+\theta(\sigma^2/2-\rho)t.}
$$

The corresponding [portfolio wealth](../../../mathematical-finance.md#portfolio-wealth) is

$$
\boxed{V_t=e^{-\rho(T-t)}\left[w_0e^{\rho T}+\theta\log(S_t/S_0)+\theta(\sigma^2/2-\rho)t\right].}
$$

Under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure), $\log(S_t/S_0)=(\rho-\sigma^2/2)t+\sigma W_t^Q$, so its value in [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) units is $V_t/B_t=w_0e^{\rho T}+\theta\sigma W_t^Q$. This also verifies the [self-financing](../../../mathematical-finance.md#self-financing-portfolio) gain equation after using the bond as [numéraire](../../../mathematical-finance.md#numeraire).

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $T=t_0$, $\tau=T-t$, and let $N$ have the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). For a twice [differentiable](../../../analysis.md#differentiable-function) payoff with enough growth control for the following [expectations](../../../probability-theory.md#expected-value) and derivatives, [risk-neutral pricing](../../../mathematical-finance.md#risk-neutral-pricing) in the dividend-free [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) gives

$$
\boxed{V(x,t)=e^{-\rho\tau}\mathbb E[f(xM)],\qquad
M=e^{(\rho-\sigma^2/2)\tau+\sigma\sqrt\tau N}.}
$$

The conditional discounted payoff is a [martingale](../../../martingale.md) under the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure). Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $e^{-\rho s}V(S_s,s)$ and setting its [drift](../../../stochastic-calculus.md#drift-coefficient) to zero therefore gives the [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation)

$$
\boxed{V_t+\frac12\sigma^2x^2V_{xx}+\rho xV_x-\rho V=0,\qquad V(x,T)=f(x).}
$$

The [delta hedge](../../../mathematical-finance.md#delta-hedge) holds $\Delta=V_x$ shares; the remaining bond value is $\beta=V-x\Delta$, or $h=\beta/e^{-\rho(T-t)}$ units of the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond). Substitution in the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and the displayed equation gives $dV=\Delta\,dS+h\,dB$, proving replication and [self-financing](../../../mathematical-finance.md#self-financing-portfolio).

Differentiating the pricing expectation in the current [stock](../../../mathematical-finance.md#stock) price gives its [option delta](../../../mathematical-finance.md#option-delta) and [option gamma](../../../mathematical-finance.md#option-gamma):

$$
\Delta=e^{-\rho\tau}\mathbb E[f'(xM)M],\qquad
\Gamma=e^{-\rho\tau}\mathbb E[f''(xM)M^2].
$$

Thus a nondecreasing payoff has a nondecreasing price; a nonincreasing payoff has a nonincreasing price. A [convex](../../../real-analysis.md#convex-function) payoff has $\Gamma\geq0$, and a [concave](../../../real-analysis.md#concave-function) payoff has $\Gamma\leq0$. This is [convexity preservation in Black-Scholes pricing](../../../mathematical-finance.md#convexity-preservation-in-black-scholes-pricing).

The [Black-Scholes parameter sensitivities](../../../mathematical-finance.md#black-scholes-parameter-sensitivities) follow directly from the same expectation. Differentiation in the [interest rate](../../../mathematical-finance.md#interest-rate) gives the [option rho](../../../mathematical-finance.md#option-rho)

$$
\boxed{V_\rho=\tau(x\Delta-V)=-\tau\beta.}
$$

For [spot volatility](../../../mathematical-finance.md#spot-volatility), differentiation first gives

$$
V_\sigma=e^{-\rho\tau}\mathbb E[f'(xM)xM(\sqrt\tau N-\sigma\tau)].
$$

The [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) identity $\mathbb E[N\psi(N)]=\mathbb E[\psi'(N)]$, applied to $\psi(N)=f'(xM)xM$, cancels the term containing $f'$ and gives the [option vega](../../../mathematical-finance.md#option-vega)

$$
\boxed{V_\sigma=\sigma\tau x^2\Gamma.}
$$

Consequently increasing [spot volatility](../../../mathematical-finance.md#spot-volatility) increases a [convex](../../../real-analysis.md#convex-function) payoff's value and decreases a [concave](../../../real-analysis.md#concave-function) payoff's value, with weak inequalities in affine or degenerate cases. A short bond position gives positive [option rho](../../../mathematical-finance.md#option-rho), while a long bond position gives negative [option rho](../../../mathematical-finance.md#option-rho). The physical [stock](../../../mathematical-finance.md#stock) [drift](../../../stochastic-calculus.md#drift-coefficient) $\mu$ does not enter these prices: the [risk-neutral measure](../../../mathematical-finance.md#risk-neutral-measure) replaces it by $\rho$.

The [option theta](../../../mathematical-finance.md#option-theta) is the calendar-time derivative at fixed current [stock](../../../mathematical-finance.md#stock) price. The [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation) gives

$$
\boxed{V_t=\rho\beta-\frac12\sigma^2x^2\Gamma.}
$$

For $\rho\geq0$, a [convex](../../../real-analysis.md#convex-function) payoff with $\beta<0$ therefore has $V_t\leq0$, while a [concave](../../../real-analysis.md#concave-function) payoff with $\beta>0$ has $V_t\geq0$. The signs are strict when $\rho>0$. At $\rho=0$, an affine payoff can give equality. Remaining-maturity sensitivity is $V_T=-V_t$ when the payoff is independent of $T$. All these time comparisons hold at fixed current [stock](../../../mathematical-finance.md#stock) price.

The stated time-monotonicity conclusion needs the nonnegative-rate condition. For example, the [convex](../../../real-analysis.md#convex-function) affine payoff $f(x)=x-K$ has

$$
V=x-Ke^{-\rho(T-t)},\qquad \beta=-Ke^{-\rho(T-t)}<0,\qquad
V_t=-\rho Ke^{-\rho(T-t)}>0\quad(\rho<0).
$$

Thus with negative [interest rates](../../../mathematical-finance.md#interest-rate) it provides an explicit counterexample even though the replica is short in bonds.

## 6

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Use $T$ for the fixed maturity and $s\leq T$ for the observation time. The original PDF's discounting uses the [instantaneous forward rate](../../../mathematical-finance.md#instantaneous-forward-rate) over $[s,T]$ and the [short rate](../../../mathematical-finance.md#short-rate) over $[0,s]$. Let $X(s,u)=F_{s,u}-\mu_{s,u}$ be the centered [Gaussian forward-rate field](../../../mathematical-finance.md#gaussian-forward-rate-field), and define

$$
A(s,T)=\int_0^s\mu_{u,u}\,du+\int_s^T\mu_{s,u}\,du,\qquad
Y(s,T)=\int_0^T X(s\wedge u,u)\,du.
$$

Assume the [covariance](../../../variance.md#covariance) and mean have the regularity needed for these [mean-square integrals](../../../measure-theory.md#mean-square-integral) and the maturity differentiation below. Splitting $Y$ at $u=s$ shows that the discounted [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is

$$
Z_{s,T}=\exp[-A(s,T)-Y(s,T)].
$$

This [integrated Gaussian forward-rate process](../../../mathematical-finance.md#integrated-gaussian-forward-rate-process) has deterministic [variance](../../../variance.md)

$$
v(s,T)=\int_0^T\int_0^T c(s\wedge u\wedge w,u,w)\,du\,dw.
$$

Its [independent increments](../../../stochastic-process.md#independent-increments) hold relative to the entire specified [filtration](../../../stochastic-process.md#filtration-probability-theory). Indeed, if $r\leq s$ and $z\leq r$, the [covariance](../../../variance.md#covariance) between $Y(s,T)-Y(r,T)$ and any earlier $X(z,w)$ is the integral of

$$
c((s\wedge u)\wedge z,u,w)-c((r\wedge u)\wedge z,u,w)=0.
$$

Since [uncorrelated jointly Gaussian variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent), the increment is independent of every finite family of earlier observations and hence of their generated [sigma-algebra](../../../measure-theory.md#sigma-algebra). The increment has [normal distribution](../../../probability-theory.md#normal-distribution) with mean zero and variance $v(s,T)-v(r,T)$. Also $Y(0,T)=0$ because $c(0,u,w)=0$.

The [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) now gives

$$
\mathbb E[Z_{s,T}\mid\mathcal F_r]
=\exp[-A(s,T)-Y(r,T)+\tfrac12(v(s,T)-v(r,T))].
$$

Therefore the [Gaussian forward-rate covariance drift restriction](../../../mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction) is exactly the deterministic condition

$$
\boxed{A(s,T)-A(0,T)=\frac12v(s,T).}
$$

It turns $Z_{s,T}/Z_{0,T}$ into a [Gaussian exponential martingale with deterministic variance](../../../stochastic-process.md#gaussian-exponential-martingale-with-deterministic-variance). The subparts establish the requested equivalent descriptions from this common calculation.

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

If the discounted [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) price is a [martingale](../../../martingale.md), its [expectation](../../../probability-theory.md#expected-value) is $Z_{0,T}=e^{-A(0,T)}$. The [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) applied to the representation above gives $\mathbb E Z_{s,T}=e^{-A(s,T)+v(s,T)/2}$, so

$$
A(s,T)-A(0,T)=\frac12v(s,T).
$$

Differentiate in maturity $T\geq s$. The two mean derivatives are $\mu_{s,T}$ and $\mu_{0,T}$. Symmetry of the [covariance](../../../variance.md#covariance) in its last two arguments makes the two boundary terms in the derivative of the double integral equal. Hence

$$
\frac12\partial_Tv(s,T)=\int_0^T c(s\wedge u,u,T)\,du.
$$

We obtain the [Gaussian forward-rate covariance drift restriction](../../../mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction)

$$
\boxed{\mu_{s,T}=\mu_{0,T}+\int_0^T c(s\wedge u,u,T)\,du,}
$$

which proves that the [martingale](../../../martingale.md) condition implies the mean restriction. Only maturity differentiation is used; a time derivative of the [covariance](../../../variance.md#covariance) is unnecessary.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Assume the displayed [Gaussian forward-rate covariance drift restriction](../../../mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction). Its diagonal instance gives

$$
\mu_{u,u}-\mu_{0,u}=\int_0^u c(w,w,u)\,dw.
$$

Using it on the two parts of the deterministic discounted exponent yields

$$
\begin{aligned}
A(s,T)-A(0,T)
&=\int_0^s\int_0^u c(w,w,u)\,dw\,du
+\int_s^T\int_0^u c(s\wedge w,w,u)\,dw\,du\\
&=\int_0^T\int_0^u c(s\wedge w,w,u)\,dw\,du\\
&=\frac12\int_0^T\int_0^T c(s\wedge u\wedge w,u,w)\,du\,dw
=\frac12v(s,T).
\end{aligned}
$$

The last equality uses [covariance](../../../variance.md#covariance) symmetry to reflect the triangular integration region across its diagonal. The [independent increments](../../../stochastic-process.md#independent-increments) of the [integrated Gaussian forward-rate process](../../../mathematical-finance.md#integrated-gaussian-forward-rate-process) and its conditional [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) then give, for $r\leq s\leq T$,

$$
\mathbb E[Z_{s,T}\mid\mathcal F_r]
=e^{-A(s,T)-Y(r,T)+(v(s,T)-v(r,T))/2}
=e^{-A(r,T)-Y(r,T)}=Z_{r,T}.
$$

All these prices are [integrable](../../../measure-theory.md#integrability) because their exponents are [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable) with finite [variance](../../../variance.md). Thus the mean restriction implies the discounted bond [martingale](../../../martingale.md) condition, completing the equivalence of the first two descriptions.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $D_s=\exp(-\int_0^sR_u\,du)$, where $R_u=F_{u,u}$ is the [short rate](../../../mathematical-finance.md#short-rate). At maturity the [zero-coupon bond](../../../mathematical-finance.md#zero-coupon-bond) pays one, so $Z_{T,T}=D_T$. If the discounted bond price is a [martingale](../../../martingale.md), its terminal [conditional expectation](../../../measure-theory.md#conditional-expectation) is

$$
D_sP_{s,T}=Z_{s,T}=\mathbb E[D_T\mid\mathcal F_s].
$$

The positive factor $D_s$ is measurable with respect to the current [filtration](../../../stochastic-process.md#filtration-probability-theory). Dividing it out gives

$$
\boxed{P_{s,T}=\mathbb E\left[\exp\left(-\int_s^TR_u\,du\right)\middle|\mathcal F_s\right].}
$$

Conversely, this identity says $Z_{s,T}=\mathbb E[D_T\mid\mathcal F_s]$. The [tower property](../../../measure-theory.md#law-of-total-expectation) gives $\mathbb E[Z_{s,T}\mid\mathcal F_r]=Z_{r,T}$ for every $r\leq s$, establishing the [martingale](../../../martingale.md) condition. The integrated [short rate](../../../mathematical-finance.md#short-rate) is a [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) with finite [variance](../../../variance.md), so the [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) proves that $D_T$ is [integrable](../../../measure-theory.md#integrability). Together with the preceding subparts, this proves all three descriptions equivalent.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
