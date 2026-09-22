<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Wealth and admissibility.** The dollar holding $\theta$ earns the risky return, while $w-\theta$ earns the [continuous-time bank account](../../../../../continuous-time-bank-account.md) return. Removing [consumption](../../../../../consumption.md) therefore gives

$$
\boxed{dw_t=\sigma\theta_t\,dW_t+\bigl[rw_t+(\mu-r)\theta_t-c_t\bigr]dt.}
$$

Here $\theta$ is a dollar amount, not a number of shares; the number of shares is $\theta_t/S_t$. Both controls must use available information: take $\theta$ [predictable](../../../../../predictable-process.md) and $c\geq0$ [progressively measurable](../../../../../progressive-measurability.md), with

$$
\int_0^t(\sigma\theta_s)^2ds<\infty,\qquad
\int_0^t\bigl(|(\mu-r)\theta_s|+c_s\bigr)ds<\infty
$$

almost surely on every finite interval. Require a well-defined objective and an [admissible trading strategy](../../../../../admissible-trading-strategy.md) satisfying $w_t\geq0$. At zero [portfolio wealth](../../../../../portfolio-wealth.md) this excludes continued risky gambling or positive [consumption](../../../../../consumption.md). The [state-price budget constraint](../../../../../state-price-budget-constraint.md) rules out doubling strategies. Throughout the diffusion calculations take $\sigma\ne0$, positive discount $\rho$, positive decay $\lambda$, and finite value; degeneracies are discussed where they affect the conclusions.

**Satisfaction and dynamic programming.** Write the [consumption satisfaction stock](../../../../../consumption-satisfaction-stock.md) as

$$
\xi_t=e^{-\lambda t}\left(\xi_0+\int_0^t e^{\lambda s}c_sds\right).
$$

The [product rule](../../../../../product-rule.md) gives, almost everywhere in time,

$$
\boxed{d\xi_t=(c_t-\lambda\xi_t)\,dt.}
$$

This state is a [finite-variation process](../../../../../finite-variation-process.md), so it has no [quadratic covariation](../../../../../quadratic-covariation.md) with [portfolio wealth](../../../../../portfolio-wealth.md). Applying the [Itô formula](../../../../../ito-s-lemma.md) to the discounted [value function](../../../../../value-function.md) over a short interval, then using [dynamic programming](../../../../../dynamic-programming.md), gives the interior [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md)

$$
0=U(\xi)-\rho V+rwV_w-\lambda\xi V_\xi
+\sup_{\theta\in\mathbb R}\left\{(\mu-r)\theta V_w+\frac{\sigma^2\theta^2}{2}V_{ww}\right\}
+\sup_{c\geq0}c(V_\xi-V_w).
$$

Assuming $V_{ww}<0$, completing the square gives

$$
\theta^*=-\frac{\mu-r}{\sigma^2}\frac{V_w}{V_{ww}},
\qquad
\sup_\theta\{\cdots\}=-\frac{\kappa^2}{2}\frac{V_w^2}{V_{ww}},
\qquad
\kappa=\frac{\mu-r}{\sigma}.
$$

The last supremum is zero if $V_\xi-V_w\leq0$ and infinite otherwise. Thus **the [gradient constraint for unbounded consumption](../../../../../gradient-constraint-for-unbounded-consumption.md) is $V_\xi\leq V_w$, and $c=0$ wherever the inequality is strict.** Since there is no direct penalty for a very large [consumption](../../../../../consumption.md) rate, an active boundary can involve [singular consumption control](../../../../../singular-consumption-control.md). In that relaxed interpretation the [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
\max\left\{U(\xi)-\rho V+rwV_w-\lambda\xi V_\xi
-\frac{\kappa^2}{2}\frac{V_w^2}{V_{ww}},\ V_\xi-V_w\right\}=0.
$$

With ordinary rate controls, this describes the supremum and its limiting transfer policy; it does not promise that an instantaneous transfer is attained by a finite rate.

**Power reduction.** An additive constant in the [utility function](../../../../../utility-function-split.md) only adds a control-independent constant divided by $\rho$ to the value, so normalize $U(\xi)=\xi^{1-R}/(1-R)$. Put $p=1-R$ and $x=w/\xi$ for $\xi>0$. Scaling [portfolio wealth](../../../../../portfolio-wealth.md), [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) and the controls by the same positive number gives the [wealth-to-satisfaction reduction](../../../../../wealth-to-satisfaction-reduction.md)

$$
V(\xi,w)=\xi^p v(x),\qquad
V_w=\xi^{-R}v',\quad
V_{ww}=\xi^{-R-1}v'',\quad
V_\xi=\xi^{-R}(pv-xv').
$$

Consequently the reduced [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
\boxed{\max\left\{
\frac1p-[\rho+\lambda p]v+(r+\lambda)xv'
-\frac{\kappa^2}{2}\frac{(v')^2}{v''},
\ pv-(x+1)v'
\right\}=0.}
$$

In the strict waiting region the first expression vanishes and [consumption](../../../../../consumption.md) is zero. On a transfer region the second vanishes; integrating it gives $v(x)=K(1+x)^p$. This reflects preservation of $w+\xi$ during an instantaneous wealth-to-satisfaction transfer.

**Why a waiting threshold is expected, and its qualification.** The [gradient constraint for unbounded consumption](../../../../../gradient-constraint-for-unbounded-consumption.md) compares the benefit of increasing [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) with the opportunity cost of spending financial [portfolio wealth](../../../../../portfolio-wealth.md). When [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) is already large relative to cash, waiting lets [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) decay while financial [portfolio wealth](../../../../../portfolio-wealth.md) earns returns; consuming immediately can be wasteful. [Homogeneity](../../../../../homogeneity.md) makes the comparison depend only on $x$. For fixed $s=w+\xi$, joint [concavity](../../../../../concave-function.md) of the [value function](../../../../../value-function.md) makes $q_s(a)=V(s-a,a)$ [concave](../../../../../concave-function.md) in financial [portfolio wealth](../../../../../portfolio-wealth.md) $a$. It is nondecreasing because an immediate transfer can reproduce any smaller financial allocation. Consequently its derivative $V_w-V_\xi$ is nonnegative and nonincreasing in $a$: a strict waiting region, if present, starts at zero financial [portfolio wealth](../../../../../portfolio-wealth.md) and ends at a single transfer boundary. [Homogeneity](../../../../../homogeneity.md) makes the corresponding boundary a ratio $x_*$. In the usual finite-boundary regime this gives $c=0$ for $x<x_*$, and transfers push a larger ratio down towards $x_*$. The condition is a comparison of marginal values, not the ordinary formula $c=(V_w)^{-1/R}$: current [utility function](../../../../../utility-function-split.md) here depends on [consumption satisfaction](../../../../../consumption-satisfaction-stock.md), not on current [consumption](../../../../../consumption.md).

A positive threshold is not guaranteed by the printed hypotheses alone. A useful sufficient local test illustrates the intended argument. Let $a=\rho+\lambda p>0$. At zero [portfolio wealth](../../../../../portfolio-wealth.md),

$$
V(\xi,0)=\frac{\xi^p}{pa},\qquad V_\xi(\xi,0)=\frac{\xi^{-R}}a.
$$

Starting with a small extra [portfolio wealth](../../../../../portfolio-wealth.md) $\varepsilon$, holding it in the [continuous-time bank account](../../../../../continuous-time-bank-account.md) until a fixed time $t$, then transferring it into [consumption satisfaction](../../../../../consumption-satisfaction-stock.md), has right derivative in $\varepsilon$ at zero equal to

$$
\frac{\xi^{-R}}a\,e^{(r-\rho+\lambda R)t}.
$$

Therefore, if $\rho<r+\lambda R$, the [portfolio wealth](../../../../../portfolio-wealth.md) marginal value is strictly larger than the [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) marginal value at zero. With the usual continuity of marginal values, there is a positive interval on which the [gradient constraint for unbounded consumption](../../../../../gradient-constraint-for-unbounded-consumption.md) is strict. The fixed-total-resource [concavity](../../../../../concave-function.md) argument then gives the threshold structure.

For a concrete counterexample to an unconditional positive threshold, take $R=1/2$, $\lambda=1$, $r=\mu=1/10$, $\sigma=1$ and $\rho=2$. There is zero [market price of risk](../../../../../market-price-of-risk.md). The relaxed value is

$$
F(\xi,w)=\frac{(\xi+w)^p}{pa},\qquad p=\frac12,\quad a=\frac52.
$$

Indeed $F_\xi=F_w$, $F_{ww}<0$, and the optimized waiting residual, after division by $\xi^p$, is

$$
-\int_0^x(1+s)^{-R}ds+\frac{r+\lambda}{a}x(1+x)^{-R}\leq0,
$$

because $(r+\lambda)/a<1$ and the integrand is decreasing. The [Itô formula](../../../../../ito-s-lemma.md) gives an upper bound by $F$, while transferring all [portfolio wealth](../../../../../portfolio-wealth.md) into [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) over intervals tending to zero attains that bound in the limit. Hence the transfer boundary is $x_*=0$ in this example. **The positive-threshold explanation needs a parameter regime supporting a genuine waiting region.** For $R>1$, even the zero-wealth value is finite only if $\rho>\lambda(R-1)$; otherwise decaying [consumption satisfaction](../../../../../consumption-satisfaction-stock.md) gives value $-\infty$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
