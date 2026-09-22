<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the [exponential distribution](../../../../../../exponential-distribution.md) change time as an exogenous time independent of the [stock](../../../../../../stock.md)'s [Brownian motion](../../../../../../brownian-motion-split.md), or, equivalently for this calculation, as having constant conditional intensity $\lambda$ while the rate remains high. Its marginal distribution alone would not imply that conditional intensity if the change time carried information about [stock](../../../../../../stock.md) returns. Write $r_1=r+\varepsilon$, $p=1-R$, $B_1=B(r_1)$, and let $V_1$ be the prechange [value function](../../../../../../value-function.md).

Over a short interval $dt$, a rate change occurs with probability $\lambda dt+o(dt)$ and changes continuation value from $V_1(w)$ to $V_0(w)$. The [dynamic programming](../../../../../../dynamic-programming.md) equation is consequently

$$
0=\sup_{c>0,\,\pi}\left\{\frac{c^p}{p}+\bigl[r_1w+\pi w(\mu-r_1)-c\bigr]V_1'(w)
+\frac12\sigma^2\pi^2w^2V_1''(w)-\rho V_1(w)+\lambda[V_0(w)-V_1(w)]\right\}.
$$

This jump term distinguishes the [exponential interest-rate switch](../../../../../../exponential-interest-rate-switch.md) from a permanent higher bank rate.

By the [homogeneity](../../../../../../homogeneity.md) of [CRRA utility](../../../../../../constant-relative-risk-aversion-utility.md), put $V_1(w)=K_1w^p/p$, with $K_1>0$. Differentiating the strictly [concave](../../../../../../concave-function.md) expressions in $c$ and $\pi$ gives

$$
c=K_1^{-1/R}w=\gamma_1w,
\qquad
\pi_1^*=\frac{\mu-r_1}{R\sigma^2}.
$$

The optimized [consumption](../../../../../../consumption.md) terms contribute $RK_1^{1-1/R}w^p/p$, and the optimized investment terms contribute $K_1B_1w^p$. With $K_0=\gamma_0^{-R}$, the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) reduces to

$$
D_1K_1=RK_1^{1-1/R}+\lambda K_0,
\qquad
D_1=\rho+\lambda-pB_1.
$$

Equivalently,

$$
\boxed{R\gamma_1+\lambda\left(\frac{\gamma_1}{\gamma_0}\right)^R=D_1,
\qquad
V_1(w)=\frac{\gamma_1^{-R}w^{1-R}}{1-R}.}
$$

The left side is continuous and strictly increasing for $\gamma_1>0$, with limits zero and infinity. Thus $D_1>0$ gives one and only one positive root. This scalar equation is an explicit characterization for arbitrary real $R$; elementary closed forms are not generally available. For example, when $R=2$,

$$
\gamma_1=\frac{\gamma_0^2}{\lambda}\left(\sqrt{1+\frac{\lambda D_1}{\gamma_0^2}}-1\right).
$$

**Use $(\pi_1^*,\gamma_1)$ until the rate changes, and $(\pi_0^*,\gamma_0)$ afterwards.** If the two rates coincide, the root is $\gamma_1=\gamma_0$; as $\lambda$ tends to infinity, it also tends to $\gamma_0$.

For a direct attainability check, use the proposed prechange constant fractions. The [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) moment is $E[w_t^p]=w^p\exp[p(B_1-\gamma_1)t]$ on the prechange evolution. Conditioning on the independent [exponential distribution](../../../../../../exponential-distribution.md) time therefore gives

$$
E\left[\int_0^\tau e^{-\rho t}\frac{(\gamma_1w_t)^p}{p}dt+e^{-\rho\tau}V_0(w_\tau)\right]
=\frac{w^p}{p}\frac{\gamma_1^p+\lambda K_0}{D_1+p\gamma_1}
=\frac{K_1w^p}{p}.
$$

The denominator is positive because the scalar equation gives $D_1+p\gamma_1=\gamma_1+\lambda K_0/K_1>0$. Hence the candidate policy actually achieves the stated value.

One can also verify the upper bound for both signs of $p$ without relying on a sign-sensitive terminal-value argument. Let $j_t$ be the current regime, $w^*$ the candidate [portfolio wealth](../../../../../../portfolio-wealth.md), and

$$
M_t=e^{-\rho t}K_{j_t}(w_t^*)^{-R}=e^{-\rho t}(c_t^*)^{-R}.
$$

If $N_t=\mathbf1_{\{\tau\leq t\}}$ and $\widetilde N_t=N_t-\lambda(t\wedge\tau)$, the [Itô formula](../../../../../../ito-s-lemma.md) and the scalar equation give

$$
\frac{dM_t}{M_{t-}}=-r_{j_t}dt-\frac{\mu-r_{j_t}}{\sigma}dW_t
+\left(\frac{K_0}{K_1}-1\right)d\widetilde N_t,
$$

where the jump term stops after the switch and continuous coefficients are understood predictably. Thus $M$ is a positive [martingale deflator](../../../../../../martingale-deflator.md): for any admissible [portfolio wealth](../../../../../../portfolio-wealth.md) $w$, the process $M_tw_t+\int_0^tM_sc_sds$ is a nonnegative [local martingale](../../../../../../local-martingale.md). It follows that

$$
E\int_0^\infty M_tc_tdt\leq M_0w_0.
$$

For the candidate policy, $E[M_tw_t^*]\to0$. Indeed its surviving prechange term decays at rate $D_1+p\gamma_1>0$, and its postchange terms decay at rate $\gamma_0>0$; integrating over the switch time preserves convergence to zero. The finite-time moment computations also make its budget equality exact. Consequently $E\int_0^\infty M_tc_t^*dt=M_0w_0$. Apply the [concave supporting-tangent inequality](../../../../../../concave-supporting-tangent-inequality.md)

$$
U(c_t)\leq U(c_t^*)+(c_t^*)^{-R}(c_t-c_t^*)
$$

and integrate in time and [expectation](../../../../../../expected-value.md). The budget inequality proves that no admissible policy exceeds the candidate. This verifies the [value function](../../../../../../value-function.md), including when $R>1$.

Both $\gamma_0>0$ and $D_1>0$ are needed for a finite prechange answer. If the postchange value is already infinite, that problem persists after the almost surely finite switch. If $\gamma_0>0$ but $D_1\leq0$, then for $p>0$ a small constant prechange [consumption](../../../../../../consumption.md) fraction makes the expected [utility function](../../../../../../utility-function-split.md) before the switch diverge, or makes its supremum diverge when $D_1=0$. For $p<0$, the optimal no-consumption terminal moment before the switch is $w^p e^{pB_1t}$; withdrawals only increase this negative-power moment. The expected magnitude of the negative postchange continuation [utility function](../../../../../../utility-function-split.md) therefore contains the divergent integral $\lambda K_0w^p\int_0^\infty e^{-D_1t}dt/|p|$. Thus these cases yield respectively $+\infty$ or $-\infty$, rather than a positive-root solution.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
