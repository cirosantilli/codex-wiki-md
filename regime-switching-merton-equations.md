# Regime-switching Merton equations

↑ **Parent:** [Merton consumption-investment problem](merton-consumption-investment-problem.md)

For an observed finite-state [continuous-time Markov chain](continuous-time-markov-chain.md) with rate matrix $Q$, constant bank rate $r$, and state-dependent stock drifts $\mu_i$ and positive volatilities $\sigma_i$, [constant relative risk aversion utility](constant-relative-risk-aversion-utility.md) gives $V_i(w)=A_iw^{1-R}/(1-R)$. Set $\kappa_i=(\mu_i-r)/\sigma_i$ and $d_i=\rho-(1-R)(r+\kappa_i^2/(2R))$. The [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) reduces to the displayed nonlinear algebraic system with $A_i>0$. Its feedback controls are $c_i=A_i^{-1/R}w$ and $\theta_i=(\mu_i-r)w/(R\sigma_i^2)$.

A damped [Newton method](newton-s-method-in-optimization.md) in the logarithmic variables $A_i=e^{x_i}$ preserves positivity. Solving these equations produces a candidate value; admissibility, stochastic-integral bounds and the [investment value transversality condition](investment-value-transversality-condition.md) still need verification.

## ↑ Ancestors (10)

1. [Merton consumption-investment problem](merton-consumption-investment-problem.md)
2. [Investment-consumption problem](investment-consumption-problem.md)
3. [Expected utility maximization](expected-utility-maximization.md)
4. [Expected utility hypothesis](expected-utility-hypothesis.md)
5. [Utility function](utility-function-split.md)
6. [Mathematical finance](mathematical-finance-split.md)
7. [Mathematical optimization](mathematical-optimization-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-40/4/solution.md)
