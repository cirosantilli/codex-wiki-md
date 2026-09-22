# Derivative-weighted call delta martingale

↑ **Parent:** [Call delta equation for a driftless local volatility diffusion](call-delta-equation-for-a-driftless-local-volatility-diffusion.md)

Suppose $a'$ is bounded and let $dZ_t=Z_ta'(S_t)dW_t$, $Z_0=1$. The [Novikov condition](novikov-s-condition.md) makes $Z$ a strictly positive true [martingale](martingale-split.md). For $\pi_t=U(t,S_t)$ solving the [call delta equation for a driftless local volatility diffusion](call-delta-equation-for-a-driftless-local-volatility-diffusion.md), the product formula gives

$$
d(Z_t\pi_t)=Z_t\bigl(a(S_t)U_S(t,S_t)+a'(S_t)U(t,S_t)\bigr)dW_t.
$$

The two drift terms cancel through [quadratic covariation](quadratic-covariation.md). Thus $Z\pi$ is a [local martingale](local-martingale.md). If it is a true [martingale](martingale-split.md) on the closed horizon, its terminal value is $Z_T\mathbf1_{\{S_T\ge K\}}$, so

$$
\pi_t=\frac{\mathbb E[Z_T\mathbf1_{\{S_T\ge K\}}\mid\mathcal F_t]}{Z_t},\qquad0\le\pi_t\le1.
$$

The upper bound uses $\mathbb E[Z_T\mid\mathcal F_t]=Z_t$. Equivalently, the [option delta](option-delta.md) is the terminal-exceedance probability under the measure with density $Z_T$.

## ↑ Ancestors (8)

1. [Call delta equation for a driftless local volatility diffusion](call-delta-equation-for-a-driftless-local-volatility-diffusion.md)
2. [Option delta](option-delta.md)
3. [Greeks (finance)](greeks-finance.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32/4/solution.md)
