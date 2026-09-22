# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper40.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $\kappa=(\mu-r)/\sigma$, assuming $\sigma>0$, and let

$$
\xi_t=\exp\bigl(-rt-\kappa W_t-\tfrac12\kappa^2t\bigr).
$$

This [state-price density](../../../mathematical-finance.md#state-price-density) prices the [bank account](../../../mathematical-finance.md#bank-account) and the risky asset. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d(\xi_tw_t)+\xi_tc_t\,dt=\xi_t(\sigma\theta_t-\kappa w_t)\,dW_t.
$$

Nonnegative wealth and consumption make the deflated cumulative gains a nonnegative [local martingale](../../../martingale.md#local-martingale), hence a [supermartingale](../../../martingale.md#supermartingale). Every admissible consumption stream therefore satisfies the [state-price budget constraint](../../../mathematical-finance.md#state-price-budget-constraint) $\mathbb E\int_0^\infty\xi_tc_t\,dt\leq w_0$.

Write $I=(U')^{-1}$ for the [inverse marginal utility](../../../utility-function.md#inverse-marginal-utility). The [Inada conditions](../../../utility-function.md#inada-conditions) make $I$ decreasing from infinity to zero. A positive [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) $y$ for the budget gives the pointwise condition $e^{-\rho t}U'(c_t)=y\xi_t$. Thus, whenever a finite optimum exists and a multiplier exhausts the budget,

$$
\boxed{c_t^*=I(ye^{\rho t}\xi_t),\qquad\mathbb E\int_0^\infty\xi_tI(ye^{\rho t}\xi_t)\,dt=w_0.}
$$

The [concave supporting-tangent inequality](../../../real-analysis.md#concave-supporting-tangent-inequality), integrated against the budget, proves optimality. These curvature and endpoint assumptions alone do not ensure that the infinite-horizon value is finite; part (b) gives the exact additional condition for power utility.

The optimal wealth is the conditional price of remaining consumption:

$$
w_t^*=\xi_t^{-1}\mathbb E\left[\left.\int_t^\infty\xi_sc_s^*\,ds\right|\mathcal F_t\right].
$$

It is nonnegative. Apply the [Martingale representation theorem](../../../brownian-motion.md#martingale-representation-theorem) to the integrable total discounted consumption claim:

$$
M_t=\mathbb E\left[\left.\int_0^\infty\xi_sc_s^*\,ds\right|\mathcal F_t\right]
=w_0+\int_0^t\phi_s\,dW_s.
$$

Comparing $M_t=\xi_tw_t^*+\int_0^t\xi_sc_s^*ds$ with the deflated wealth equation yields

$$
\boxed{\theta_t^*=\frac1\sigma\left(\frac{\phi_t}{\xi_t}+\kappa w_t^*\right).}
$$

This constructs the portfolio without assuming extra smoothness of the [value function](../../../mathematical-optimization.md#value-function). If the stationary value $V$ is twice differentiable with $V''<0$, optimization of its [Hamilton-Jacobi-Bellman equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) instead gives $\theta^*(w)=-(\mu-r)V'(w)/(\sigma^2V''(w))$ and $c^*(w)=I(V'(w))$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For [constant relative risk aversion utility](../../../utility-function.md#constant-relative-risk-aversion-utility), $I(z)=z^{-1/R}$. Define the [Merton consumption constant](../../../utility-function.md#merton-consumption-constant)

$$
\gamma_M=\frac{\rho-(1-R)(r+\kappa^2/(2R))}{R}.
$$

The Gaussian exponential moment gives

$$
\mathbb E[\xi_t(ye^{\rho t}\xi_t)^{-1/R}]=y^{-1/R}e^{-\gamma_Mt}.
$$

When $\gamma_M>0$, the budget is $w_0=y^{-1/R}/\gamma_M$. Conditional pricing then gives $c_t^*=\gamma_Mw_t^*$, and the [Merton consumption-investment problem](../../../utility-function.md#merton-consumption-investment-problem) has

$$
\boxed{V(w)=\frac{\gamma_M^{-R}w^{1-R}}{1-R},\qquad c_t^*=\gamma_Mw_t^*,\qquad\theta_t^*=\frac{\mu-r}{R\sigma^2}w_t^*.}
$$

The resulting wealth is a [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion), so positive initial wealth remains positive. Substitution in the [Hamilton-Jacobi-Bellman equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) verifies the first-order conditions and the value; the budget argument in part (a) supplies global optimality.

**The problem has a finite value precisely when $\gamma_M>0$.** For $0<R<1$ and $\gamma_M\leq0$, the supremum is $+\infty$. Indeed, use the displayed risky fraction and consumption $c_t=kw_t$, $k>0$. Its expected utility is

$$
\frac{w^{1-R}k^{1-R}}{1-R}\int_0^\infty e^{-[R\gamma_M+(1-R)k]t}\,dt.
$$

For $\gamma_M<0$, sufficiently small $k$ already gives infinite utility. For $\gamma_M=0$, the finite values tend to infinity as $k\downarrow0$.

For $R>1$ and $\gamma_M\leq0$, every admissible stream has utility $-\infty$. To see this, put $q=(R-1)/R$ and apply [Holder inequality](../../../functional-analysis.md#holder-inequality) on $[0,T]\times\Omega$:

$$
\int_0^T e^{-\gamma_Mt}\,dt
=\mathbb E\int_0^T(e^{-\rho t}c_t^{1-R})^{1/R}(\xi_tc_t)^{(R-1)/R}\,dt
\leq\left(\mathbb E\int_0^T e^{-\rho t}c_t^{1-R}dt\right)^{1/R}w_0^{(R-1)/R}.
$$

The left side diverges as $T\to\infty$, forcing the positive utility-cost integral to diverge. Thus there is no finite-value optimization problem in either ill-posed case.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

In a price-taking equilibrium, market clearing fixes aggregate consumption at the dividend $\delta_t$, so $c_t^i=p_t^i\delta_t$ and $\sum_i p_t^i=1$. Each agent takes this aggregate benchmark as given when varying their own consumption. Let $\xi_t$ be a common [state-price density](../../../mathematical-finance.md#state-price-density) and $y_i>0$ their budget multipliers. Marginal pricing gives

$$
e^{-\rho_it}\frac{U_i'(p_t^i)}{\delta_t}=y_i\xi_t.
$$

Write $I_i=(U_i')^{-1}$ and $b_t=\xi_t\delta_t$. Then

$$
p_t^i=I_i(y_ie^{\rho_it}b_t),\qquad\sum_i I_i(y_ie^{\rho_it}b_t)=1.
$$

For fixed $t$, the second left side is continuous and strictly decreasing from infinity to zero, so it determines a unique positive number $b(t)$. Every coefficient in that equation is deterministic. Consequently

$$
\boxed{p_t^i=I_i(y_ie^{\rho_it}b(t))\text{ is deterministic},\qquad\xi_t=\frac{b(t)}{\delta_t}.}
$$

This is the [relative-consumption share equilibrium](../../../mathematical-finance.md#relative-consumption-share-equilibrium). The absolute consumption streams remain random through $\delta_t$.

Assuming finite fundamental prices, the ex-dividend price of the productive asset follows from conditional pricing:

$$
\boxed{S_t=\xi_t^{-1}\mathbb E_t\int_t^\infty\xi_s\delta_s\,ds
=\frac{\delta_t}{b(t)}\int_t^\infty b(s)\,ds.}
$$

The initial [state-price budget constraints](../../../mathematical-finance.md#state-price-budget-constraint) determine the multipliers up to a common normalization:

$$
\int_0^\infty b(t)I_i(y_ie^{\rho_it}b(t))\,dt
=\pi_0^i\int_0^\infty b(t)\,dt,\qquad i=1,\ldots,J.
$$

Together with the scalar market-clearing equation these characterize the equilibrium. A common scaling of all $y_i$ is offset by the reciprocal scaling of $b$. At least one redundant budget equation can be removed, since the initial fractions sum to one.

For completeness, define $B(t)=\int_t^\infty b(s)ds$ and $B_i(t)=\int_t^\infty b(s)p_s^i ds$. The consumption-financing wealth is $w_t^i=\delta_tB_i(t)/b(t)$. Its stochastic exposure and that of $S_t$ are both proportional to $\delta_t$. Thus holding $B_i(t)/B(t)$ units of the productive asset, with no bank-account balance, finances this wealth and consumption. Indeed, the holding's deterministic changes and dividend consumption balance because $B_i'=-bp^i$ and $B'=-b$.

If all $\rho_i=\rho$ and $U_i=U$, market clearing gives $b(t)=ke^{-\rho t}$ for a constant $k>0$, and $p_t^i=I(y_ik)$ is constant. The budget equations then imply

$$
\boxed{p_t^i=\pi_0^i,\qquad c_t^i=\pi_0^i\delta_t,\qquad S_t=\delta_t/\rho.}
$$

For differentiable $b$, the general equilibrium has short rate $r_t=\mu-\sigma^2-b'(t)/b(t)$ and risky-asset total expected return $r_t+\sigma^2$; its volatility is $\sigma$. These follow directly from $\xi_t=b(t)/\delta_t$ and the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma). In the identical-agent case, $r=\mu-\sigma^2+\rho$.

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $\kappa=(\mu-r)/\sigma$ and $\gamma_M$ from Question 1, and take the finite-value case $\gamma_M>0$. After retirement the value is $V_M(w)=\gamma_M^{-R}w^{1-R}/(1-R)$. Working for an infinitesimal extra interval while using the retired portfolio and consumption produces a gain $\varepsilon V_M'(w)-\lambda$. Its zero is

$$
w_{\mathrm{myopic}}=\gamma_M^{-1}(\varepsilon/\lambda)^{1/R}.
$$

This proves **the instantaneous indifference level** appearing in the question. For the stated irreversible [optimal stopping](../../../martingale.md#optimal-stopping) problem it is generally a lower bound on the retirement boundary, rather than the boundary itself: retaining the opportunity to keep working has value. The following explicit [wealth-variable Legendre dual](../../../utility-function.md#wealth-variable-legendre-dual) calculation exhibits the correction. In particular, imposing continuity of $V''$ at retirement would discard that option value; [smooth fit](../../../martingale.md#smooth-pasting) requires continuity of $V'$.

Assume the usual borrowing-against-income solvency condition: $w> -\varepsilon/r$ while working, with nonnegative wealth after retirement, and take $r>0$, $\rho>0$, $\kappa\ne0$. The question does not specify a tighter borrowing constraint. Let $J(z)=\sup_w\{V(w)-zw\}$, so $w=-J'(z)$ and $V=J-zJ'$. The working [Hamilton-Jacobi-Bellman equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) becomes the linear [Cauchy-Euler equation](../../../differential-equation.md#cauchy-euler-equation)

$$
\tfrac12\kappa^2z^2J''+(\rho-r)zJ'-\rho J+
\frac{R}{1-R}z^{1-1/R}+\varepsilon z-\lambda=0.
$$

The retired dual is $J_M(z)=Rz^{1-1/R}/[(1-R)\gamma_M]$. Let $m<0$ be the negative root of

$$
\tfrac12\kappa^2m(m-1)+(\rho-r)m-\rho=0.
$$

The other root exceeds one. Its growing term is excluded by the solvency asymptotic as $z\to\infty$. Therefore the working dual has the form

$$
J(z)=J_M(z)+\frac{\varepsilon}{r}z-\frac{\lambda}{\rho}+Dz^m.
$$

Retirement corresponds to $z\leq z_*$, where $J=J_M$. Value matching and [smooth fit](../../../martingale.md#smooth-pasting) give

$$
\frac{\varepsilon z_*}{r}-\frac{\lambda}{\rho}+Dz_*^m=0,\qquad
\frac{\varepsilon}{r}+Dmz_*^{m-1}=0.
$$

Consequently the [retirement boundary with an income option](../../../utility-function.md#retirement-boundary-with-an-income-option) is

$$
\boxed{z_* =\frac{\lambda r}{\varepsilon\rho}\frac{m}{m-1},\qquad
D=-\frac{\varepsilon}{rm}z_*^{1-m}>0,\qquad
\overline w=\gamma_M^{-1}z_*^{-1/R}.}
$$

Using the root equation, $z_*/(\lambda/\varepsilon)=1+\kappa^2m/(2\rho)$, which lies strictly between zero and one. Thus $\overline w>w_{\mathrm{myopic}}$ for a nonzero risk premium. For example, $r=\rho=\varepsilon=\lambda=\kappa=1$ and $R=2$ give $m=-1$, $\gamma_M=9/8$, and

$$
\overline w=\frac{8\sqrt2}{9},\qquad w_{\mathrm{myopic}}=\frac89.
$$

These parameters give an explicit counterexample to identifying the printed level with the irreversible retirement boundary.

For $-\varepsilon/r<w<\overline w$, find the unique $z>z_*$ from

$$
w=\gamma_M^{-1}z^{-1/R}-\frac{\varepsilon}{r}-Dmz^{m-1}.
$$

This right side decreases strictly from $\overline w$ to $-\varepsilon/r$, since $J''>0$. Recover the value and controls by

$$
\boxed{V(w)=J(z)+zw,\qquad c^*(w)=z^{-1/R},\qquad
\theta^*(w)=\frac{\mu-r}{\sigma^2}zJ''(z).}
$$

For $w\geq\overline w$, retire immediately and use the Merton controls. Along the working strategy, $z_t$ satisfies $dz_t=(\rho-r)z_tdt-\kappa z_tdW_t$, and the optimal retirement time is its first hitting time of $z_*$, equivalently wealth's first hitting time of $\overline w$.

To check the [optimal stopping](../../../martingale.md#optimal-stopping) inequalities, write $h=J-J_M$. It satisfies $h(z_*)=h'(z_*)=0$ and $h''(z)=Dm(m-1)z^{m-2}>0$ for $z>z_*$. Hence continuation has positive option value there. On $z\leq z_*$ the stopping candidate has working residual $\varepsilon z-\lambda\leq0$. The matched dual is continuously differentiable, so the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) introduces no boundary local-time term. Localization, the state-price budget, and the appropriate infinite-horizon transversality justify verification.

If nonnegative financial wealth is imposed during employment as an additional constraint, the working dual also has an upper boundary, and that extra constraint must be included in the free-boundary problem. It cannot be recovered by assuming the printed myopic equality.

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Assume the regime is observed and $\sigma_i=\sigma(i)>0$. With $\mu_i=\mu(i)$, the wealth dynamics are

$$
\boxed{dw_t=[rw_t+(\mu_{\xi_t}-r)\theta_t-c_t]dt+\sigma_{\xi_t}\theta_t\,dW_t.}
$$

Let $V_i(w)$ be the [value function](../../../mathematical-optimization.md#value-function) conditional on the [continuous-time Markov chain](../../../markov-process.md#continuous-time-markov-chain) being in state $i$. Its generator adds $\sum_jq_{ij}V_j(w)$ to the diffusion generator. The [Hamilton-Jacobi-Bellman equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) is

$$
0=\sup_{c>0,\theta}\left\{U(c)+(rw+(\mu_i-r)\theta-c)V_i'
+\tfrac12\sigma_i^2\theta^2V_i''\right\}+\sum_jq_{ij}V_j-\rho V_i.
$$

For $V_i'>0$, $V_i''<0$, the maximizing controls are $c=I(V_i')$ and $\theta=-(\mu_i-r)V_i'/(\sigma_i^2V_i'')$. Put $\kappa_i=(\mu_i-r)/\sigma_i$. The optimized equation is

$$
0=\widehat U(V_i')+rwV_i'-\frac{\kappa_i^2(V_i')^2}{2V_i''}+\sum_jq_{ij}V_j-\rho V_i.
$$

Here $\widehat U$ is the [utility conjugate](../../../convex-optimization.md#utility-conjugate).

Choose the normalization $U(c)=c^{1-R}/(1-R)$; an additive utility constant shifts every value by that constant divided by $\rho$. Homogeneity gives $V_i(w)=A_iw^{1-R}/(1-R)$ with $A_i>0$. The [regime-switching Merton equations](../../../utility-function.md#regime-switching-merton-equations) reduce the differential system to one nonlinear algebraic equation per regime:

$$
\boxed{\left[\rho-(1-R)\left(r+\frac{\kappa_i^2}{2R}\right)\right]A_i
-\sum_jq_{ij}A_j-R A_i^{1-1/R}=0.}
$$

The candidate feedback controls are

$$
\boxed{c_i^*(w)=A_i^{-1/R}w,\qquad\theta_i^*(w)=\frac{\mu_i-r}{R\sigma_i^2}w.}
$$

Changing the regime changes consumption's wealth coefficient, while the risky fraction uses the current regime's risk premium and volatility.

Numerically solve these finite-dimensional equations by a damped [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization), using $A_i=e^{x_i}$ to enforce positivity. For $d_i=\rho-(1-R)(r+\kappa_i^2/(2R))$, the Jacobian in the $A$ variables is

$$
\frac{\partial F_i}{\partial A_j}=d_i\mathbf1_{\{i=j\}}-q_{ij}-(R-1)A_i^{-1/R}\mathbf1_{\{i=j\}}.
$$

Multiply its $j$th column by $A_j$ in the logarithmic variables. A residual-decreasing line search and continuation from $Q=0$, where the positive solution is the scalar Merton coefficient in each well-posed regime, give a practical method whenever that starting problem is finite. More generally use a positive initialization for the coupled system, and check residuals, positivity and conditioning rather than accepting an arbitrary algebraic root.

Verification requires constructing admissible feedback controls, proving the resulting wealth stays nonnegative, and establishing the stochastic-integral and transversality bounds needed at infinite horizon. Apply the [Itô formula for semimartingales with jumps](../../../stochastic-calculus.md#ito-formula-for-semimartingales-with-jumps) to $e^{-\rho t}V_{\xi_t}(w_t)$, stopping before wealth leaves a compact interval. The [Hamilton-Jacobi-Bellman equation](../../../mathematical-optimization.md#hamilton-jacobi-bellman-equation) makes accumulated utility plus discounted candidate value a [local supermartingale](../../../martingale.md#local-supermartingale) for every admissible policy and a [local martingale](../../../martingale.md#local-martingale) under the feedback. Justify removal of localization and let the terminal discounted value vanish under the candidate. For $0<R<1$, the nonnegative terminal value can be dropped for the upper bound; for $R>1$ it is negative, so a transversality or dual integrability argument is essential. This establishes the global value bound and attainment, rather than just stationarity of the algebraic equations. The boundary is $V_i(0)=0$ for $R<1$ and the limiting value $-\infty$ for $R>1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
