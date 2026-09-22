<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the primitive $U(c)=c^{1-R}/(1-R)$, as in Question 3, and the usual positive [spot volatility](../../../../../../spot-volatility.md) convention $\sigma>0$. An additive [utility function](../../../../../../utility-function-split.md) constant shifts both agents' [value functions](../../../../../../value-function.md) equally and does not affect their policies or the comparison. Set

$$
h(x)=a\tanh(ax),\qquad b(x)=\mu-r+\sigma h(x).
$$

The [Itô formula](../../../../../../ito-s-lemma.md) applied to the [stock](../../../../../../stock.md) price and the [binary Brownian drift filter](../../../../../../binary-brownian-drift-filter.md) gives

$$
\frac{dS_t}{S_t}=\sigma d\widehat W_t+[\mu+\sigma h(X_t)]dt.
$$

Let $\theta_t$ denote the dollar [stock](../../../../../../stock.md) holding. The separated state equations are

$$
dw_t=[rw_t+\theta_tb(X_t)-c_t]dt+\sigma\theta_t\,d\widehat W_t,
\qquad
dX_t=h(X_t)dt+d\widehat W_t.
$$

Both states use the same observed [Brownian motion](../../../../../../brownian-motion-split.md). In particular, their [quadratic covariation](../../../../../../quadratic-covariation.md) is $d[w,X]_t=\sigma\theta_tdt$.

Let $J(w,x)$ be the Bayesian [value function](../../../../../../value-function.md). Its [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) is

$$
\rho J=\sup_{c>0,\,\theta}\left\{\frac{c^{1-R}}{1-R}+(rw+\theta b(x)-c)J_w+h(x)J_x
+\frac12J_{xx}+\frac12\sigma^2\theta^2J_{ww}+\sigma\theta J_{wx}\right\}.
$$

The cross derivative is necessary: learning and [portfolio wealth](../../../../../../portfolio-wealth.md) are correlated through the same observation shock. At a smooth, finite, strictly [concave](../../../../../../concave-function.md) value, the optimal [consumption](../../../../../../consumption.md) and [stock](../../../../../../stock.md) holding are

$$
\boxed{c^*=(J_w)^{-1/R},\qquad
\theta^*=-\frac{b(x)J_w+\sigma J_{wx}}{\sigma^2J_{ww}}.}
$$

The number of shares is $\theta^*/S$, and the wealth fraction is $\theta^*/w$.

More explicitly, [homogeneity](../../../../../../homogeneity.md) gives $J(w,x)=K(x)w^p/p$, where $p=1-R$. Then

$$
\boxed{c^*=K(x)^{-1/R}w,\qquad
\pi^*(x)=\frac{b(x)+\sigma K'(x)/K(x)}{R\sigma^2}.}
$$

The additional term is the [learning hedge in a binary-drift investment model](../../../../../../learning-hedge-in-a-binary-drift-investment-model.md), a form of [intertemporal hedging demand](../../../../../../intertemporal-hedging-demand.md). Merely putting the [Bayesian posterior](../../../../../../bayesian-posterior.md) mean [drift](../../../../../../drift-coefficient.md) into a constant-coefficient investment formula would omit it. Eliminating the controls gives the coefficient equation

$$
\frac12K''+hK'+(pr-\rho)K+RK^{1-1/R}
+\frac{p(bK+\sigma K')^2}{2R\sigma^2K}=0.
$$

The economic solution is selected by admissibility and the infinite-horizon value condition, rather than by an arbitrary solution of this [ordinary differential equation](../../../../../../ordinary-differential-equation.md).

For the comparison, now suppose $0<R<1$ and $\mu>r$. Write $m=\mu-r>0$, $b_+=m+\sigma a$, and

$$
\gamma_+=\frac{\rho-(1-R)\left(r+\frac{b_+^2}{2R\sigma^2}\right)}{R}.
$$

When $\gamma_+>0$, the informed agent's [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md) has value

$$
V_+(w)=\frac{\gamma_+^{-R}w^{1-R}}{1-R},
\qquad
\pi_+=\frac{b_+}{R\sigma^2},\qquad c_+=\gamma_+w.
$$

These are the policies available to an agent who knows the true [drift](../../../../../../drift-coefficient.md) is $+a$.

For any admissible Bayesian policy, not only its optimum, define

$$
Y_t=\int_0^t e^{-\rho s}U(c_s)ds+e^{-\rho t}V_+(w_t).
$$

The integration variable is $s$ throughout the accumulated [utility function](../../../../../../utility-function-split.md). Applying the [Itô formula](../../../../../../ito-s-lemma.md) in the Bayesian observation [filtration](../../../../../../filtration-probability-theory.md) gives

$$
dY_t=e^{-\rho t}H_{b(X_t)}(w_t,c_t,\theta_t)dt
+e^{-\rho t}\sigma\theta_tV_+'(w_t)d\widehat W_t,
$$

where

$$
H_b(w,c,\theta)=U(c)-\rho V_+(w)+(rw+\theta b-c)V_+'(w)
+\frac12\sigma^2\theta^2V_+''(w).
$$

The informed-agent [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) says $\sup_{c,\theta}H_{b_+}=0$. Maximizing the [stock](../../../../../../stock.md) term at any excess [drift](../../../../../../drift-coefficient.md) $b$ gives

$$
\sup_\theta\left\{\theta bV_+'+\frac12\sigma^2\theta^2V_+''\right\}
=-\frac{b^2(V_+')^2}{2\sigma^2V_+''}.
$$

Since $V_+''<0$, this maximum increases with $b^2$. The [binary Brownian drift filter](../../../../../../binary-brownian-drift-filter.md) satisfies $|h(x)|\leq a$, and therefore

$$
|b(x)|=|m+\sigma h(x)|\leq m+\sigma a=b_+.
$$

It follows that $H_{b(x)}(w,c,\theta)\leq\sup_{c,\theta}H_{b(x)}\leq\sup_{c,\theta}H_{b_+}=0$. Thus $Y$ is a [local supermartingale](../../../../../../local-supermartingale.md). Because $0<R<1$, both accumulated [utility function](../../../../../../utility-function-split.md) and $V_+$ are nonnegative. A nonnegative [local supermartingale](../../../../../../local-supermartingale.md) is a genuine [supermartingale](../../../../../../supermartingale.md), by localization and the conditional [Fatou lemma](../../../../../../fatou-s-lemma.md). This proves the requested assertion under the Bayesian probability law, without conditioning that law on the favorable [drift](../../../../../../drift-coefficient.md).

Consequently

$$
E\int_0^t e^{-\rho s}U(c_s)ds\leq E[Y_t]\leq Y_0=V_+(w_0).
$$

The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) lets $t$ tend to infinity. Taking the supremum over Bayesian policies proves the [maximal squared Sharpe ratio value bound](../../../../../../maximal-squared-sharpe-ratio-value-bound.md)

$$
\boxed{J(w,x)\leq V_+(w).}
$$

In particular this holds at the equal-prior state $x=0$. No vanishing-terminal-value assumption is needed for this upper bound, because the terminal term is nonnegative and can simply be dropped.

The finite-value assumption $\gamma_+>0$ is missing from the printed comparison. Without it, $V_+=+\infty$ and the value inequality is trivial, but $Y$ is not a finite [supermartingale](../../../../../../supermartingale.md). For a concrete allowed example, take $r=0$, $\mu=1$, $\sigma=a=1$, $R=1/2$ and $\rho=1$. Then $b_+=2$ and $\gamma_+=-2$. For the informed agent, the constant [stock](../../../../../../stock.md) fraction $\pi=4$ and [consumption](../../../../../../consumption.md) $c=w/2$ give

$$
E[e^{-t}U(c_t)]=\sqrt2\,w_0^{1/2}e^{3t/4}.
$$

The time integral diverges, so his value is infinite. This is why the nontrivial finite-supermartingale proof above needs the stated qualification.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
