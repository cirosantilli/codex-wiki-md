<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [competitive equilibrium with one productive asset](../../../../../../competitive-equilibrium-with-one-productive-asset.md), the primitives are the probability law and information [filtration](../../../../../../filtration-probability-theory.md) of total output $d$, each agent's [utility function](../../../../../../utility-function-split.md) and discount factor, the initial ownership shares $\theta_0^j$ summing to one, and the permitted consumption and trading strategies. Prices are not primitives of the equilibrium problem. The derived objects are the ex-dividend price $S$, each agent's [consumption](../../../../../../consumption.md) $C^j$ and holdings $\theta^j$, and their marginal-utility pricing processes. At a common price, every agent solves the individual problem, and resource and share clearing require

$$
\sum_{j=1}^JC_t^j=d_t,\qquad\sum_{j=1}^J\theta_t^j=1.
$$

The individual [discrete dividend budget equations](../../../../../../discrete-dividend-budget-equation.md), optimality Euler equations and terminal conditions from part (i), together with these clearing equations, define equilibrium even when the market is incomplete. Summing the individual [budget constraints](../../../../../../budget-constraint.md) is consistent with total fruit consumption.

For the given [constant absolute risk aversion utility](../../../../../../constant-absolute-risk-aversion-utility.md), $U_j'(c)=e^{-\gamma_jc}$. Hence each interior optimum satisfies

$$
\boxed{S_t\beta_j^te^{-\gamma_jC_t^j}
=\mathbb E_t[\beta_j^{t+1}e^{-\gamma_jC_{t+1}^j}(S_{t+1}+d_{t+1})].}
$$

The same $S$ must satisfy all these equations, but their conditional expectation identities do not by themselves identify the different agents' pricing densities pointwise.

To illustrate explicit [exponential-utility risk sharing](../../../../../../exponential-utility-risk-sharing.md), first consider a complete or otherwise implementable interior allocation. With positive constant welfare weights $a_j$, a pointwise resource multiplier $\nu_t$ satisfies

$$
a_j\beta_j^te^{-\gamma_jC_t^j}=\nu_t.
$$

Write

$$
\Gamma=\left(\sum_j\gamma_j^{-1}\right)^{-1},\qquad
\log\bar\beta=\Gamma\sum_j\gamma_j^{-1}\log\beta_j,\qquad
\log A=\Gamma\sum_j\gamma_j^{-1}\log a_j.
$$

Solving the marginal equations and summing the consumptions gives

$$
\boxed{\nu_t=A\bar\beta^te^{-\Gamma d_t},\qquad
C_t^j=\frac\Gamma{\gamma_j}d_t
+\frac t{\gamma_j}(\log\beta_j-\log\bar\beta)
+\frac1{\gamma_j}(\log a_j-\log A).}
$$

The output risk is shared in proportion to risk tolerance $\gamma_j^{-1}$; differences in patience produce the time-dependent transfer term. The common normalized [state-price density](../../../../../../state-price-density.md) is $\zeta_t=\nu_t/\nu_0$. The weights, up to a common scale, are determined by the initial wealth budgets

$$
\mathbb E\sum_{t\geq0}\zeta_tC_t^j=\theta_0^j(S_0+d_0),\qquad\zeta_0=1,
$$

and, for a fundamental price,

$$
S_t=\frac1{\nu_t}\mathbb E_t\sum_{s>t}\nu_sd_s
=e^{\Gamma d_t}\mathbb E_t\sum_{s>t}\bar\beta^{s-t}e^{-\Gamma d_s}d_s.
$$

If [consumption](../../../../../../consumption.md) is required to be nonnegative and the interior formula produces a negative allocation, replace it by

$$
C_t^j=\max\left\{0,\frac{\log a_j+t\log\beta_j-\log\nu_t}{\gamma_j}\right\},\qquad\sum_jC_t^j=d_t.
$$

For $d_t>0$ this determines the resource multiplier uniquely. At zero total output all constrained consumptions are zero and the corresponding marginal inequalities apply.

A single traded tree need not span the contingent transfers in the general risk-sharing formula. A genuine equilibrium example within the literal one-tree market is obtained by taking all $\beta_j=\beta$ and initial shares $\theta_0^j=\Gamma/\gamma_j$. Then

$$
\boxed{\theta_t^j=\Gamma/\gamma_j,\qquad C_t^j=(\Gamma/\gamma_j)d_t,\qquad
\zeta_t=\beta^t e^{-\Gamma(d_t-d_0)}.}
$$

Every agent simply keeps the initial shares, all [budget constraints](../../../../../../budget-constraint.md) and clearing conditions hold, and their discounted marginal utilities coincide. The fundamental price above satisfies every Euler equation. For example, nonnegative bounded output ensures the required price and utility integrability and the terminal terms vanish; the supporting-line argument from part (i) then verifies individual optimality. For heterogeneous discount factors or arbitrary initial ownership, the displayed coupled Euler-budget-clearing system remains the correct one-tree formulation; using the unconstrained Pareto allocation as a traded equilibrium requires an additional financing check.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
