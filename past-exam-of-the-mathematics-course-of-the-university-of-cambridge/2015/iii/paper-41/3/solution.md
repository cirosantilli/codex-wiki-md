<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use dollar holdings $\theta_0,\ldots,\theta_n$, including the traded index, and let $m=\log M$. The [Itô formula](../../../../../ito-s-lemma.md) gives

$$
dm_t=a_0\,dt+\sigma_0\,dW_t^0,\qquad
a_0=\mu_0-\tfrac12\sigma_0^2.
$$

Define the state-dependent correlation $q(m)=\rho(e^m)$, $d(m)=\sqrt{1-q(m)^2}>0$, and constants $p_i=(\mu_i-r)/\sigma_i$. The [self-financing portfolio](../../../../../self-financing-portfolio.md) with consumption has **wealth equation**

$$
\boxed{dw=\left[rw-c+\sum_{i=0}^n(\mu_i-r)\theta_i\right]dt
+\left[\sigma_0\theta_0+q(m)\sum_{i=1}^n\sigma_i\theta_i\right]dW^0
+d(m)\sum_{i=1}^n\sigma_i\theta_i\,dW^i.}
$$

Since all these assets are traded and $d(m)>0$, the volatility map is invertible. It is useful to optimize over [Brownian portfolio exposures](../../../../../brownian-portfolio-exposures.md)

$$
y_0=\sigma_0\theta_0+q\sum_{i=1}^n\sigma_i\theta_i,\qquad
y_i=d\sigma_i\theta_i,
$$

whose [market price of risk](../../../../../market-price-of-risk.md) vector is

$$
\ell_0=p_0,\qquad \ell_i(m)=\frac{p_i-q(m)p_0}{d(m)},\quad i\geq1.
$$

Indeed $\sum_i(\mu_i-r)\theta_i=\ell\cdot y$. Put $L^2(m)=p_0^2+\sum_{i=1}^n\ell_i(m)^2$.

For $R\ne1$, normalize [constant relative risk aversion utility](../../../../../constant-relative-risk-aversion-utility.md) to $U(c)=c^{1-R}/(1-R)$. Scaling wealth, holdings, and consumption by $a>0$ leaves the index state unchanged and multiplies reward by $a^{1-R}$. Thus

$$
V(w,m)=\frac{w^{1-R}}{1-R}f(m),\qquad f(m)>0.
$$

For a finite smooth value with $V_{ww}<0$, the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md), including the shared-noise cross derivative, is

$$
0=-\beta V+a_0V_m+\tfrac12\sigma_0^2V_{mm}+rwV_w
+\sup_{c>0}\{U(c)-cV_w\}
+\sup_{y\in\mathbb R^{n+1}}\left\{
V_w\ell\cdot y+\tfrac12V_{ww}|y|^2+\sigma_0V_{wm}y_0\right\}.
$$

The last term is essential: index changes and the $W^0$ component of wealth are correlated. The first-order conditions yield

$$
c^*=V_w^{-1/R},\qquad
y^*=-\frac{V_w\ell+\sigma_0V_{wm}e_0}{V_{ww}}.
$$

Because $V_w=w^{-R}f$, $V_{ww}=-Rw^{-R-1}f$, and $V_{wm}=w^{-R}f'$, the optimized portfolio contribution is

$$
\frac{w^{1-R}}{2Rf}\left[(p_0f+\sigma_0f')^2
+f^2\sum_{i=1}^n\ell_i^2\right].
$$

Substitution gives **the requested second-order nonlinear equation**

$$
\boxed{0=\tfrac12\sigma_0^2f''+a_0f'
+[(1-R)r-\beta]f+Rf^{1-1/R}
+\frac{1-R}{2Rf}\left[(p_0f+\sigma_0f')^2
+f^2\sum_{i=1}^n\ell_i^2\right].}
$$

Recovering dollar holdings from the exposures gives **the optimal controls**

$$
\boxed{c^*=wf^{-1/R},\qquad
\theta_i^*=\frac{w[p_i-q p_0]}{R\sigma_i(1-q^2)}
\quad(i=1,\ldots,n),}
$$



$$
\boxed{\theta_0^*=\frac w{R\sigma_0}
\left[p_0+\sigma_0\frac{f'}f
-\frac q{1-q^2}\sum_{i=1}^n(p_i-q p_0)\right].}
$$

Only the index holding carries the extra [intertemporal hedging demand](../../../../../intertemporal-hedging-demand.md), because the index is the source of state variation. The stock positions hedge their common exposure through the index.

The [power transformation of a complete-market investment equation](../../../../../power-transformation-of-a-complete-market-investment-equation.md) gives a useful further simplification. Let $g=f^{1/R}$, and define

$$
B=a_0+\frac{1-R}{R}\sigma_0p_0,\qquad
\delta(m)=\frac{\beta-(1-R)[r+L^2(m)/(2R)]}{R}.
$$

Expanding the squared term and substituting $f=g^R$ cancels the two $(g')^2$ terms. **The power-transformed investment equation is linear**:

$$
\boxed{\tfrac12\sigma_0^2g''+Bg'-\delta(m)g+1=0.}
$$

Then $c^*=w/g$ and $f'/f=Rg'/g$. A practical [finite difference method](../../../../../finite-difference-method.md) solves this [linear differential equation](../../../../../linear-differential-equation.md) on an expanding truncated interval in $m$, enforcing the economically relevant positive solution and checking domain and mesh convergence. If correlation approaches limits strictly inside $(-1,1)$ and the corresponding $\delta_\pm>0$, the constant-coefficient [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md) gives endpoint approximations $g\to1/\delta_\pm$. Without such asymptotics one must determine appropriate growth/transversality conditions; arbitrary fixed endpoint values are not justified. The statement's smooth decreasing correlation alone does not ensure globally bounded [market prices of risk](../../../../../market-price-of-risk.md) or a finite value. Any numerical candidate must also satisfy admissibility and the [investment value transversality condition](../../../../../investment-value-transversality-condition.md).

The printed $R>0$ includes $R=1$. In that case choose $U(c)=\log c$, whose scaling is additive:

$$
V(w,m)=\frac{\log w}{\beta}+f(m).
$$

There is no shared-noise cross derivative because $V_{wm}=0$. **The logarithmic case is**

$$
\boxed{\tfrac12\sigma_0^2f''+a_0f'-\beta f
+\log\beta-1+\frac r\beta+\frac{L^2(m)}{2\beta}=0,\qquad
c^*=\beta w,\quad y^*=w\ell.}
$$

Thus the dollar holdings are the preceding formulas with $R=1$ and the $f'/f$ hedge term omitted. This [linear differential equation](../../../../../linear-differential-equation.md) can be solved by the same truncation and convergence strategy.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
