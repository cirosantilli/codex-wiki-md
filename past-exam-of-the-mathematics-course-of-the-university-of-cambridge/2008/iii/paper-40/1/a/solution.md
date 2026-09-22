<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\kappa=(\mu-r)/\sigma$, assuming $\sigma>0$, and let

$$
\xi_t=\exp\bigl(-rt-\kappa W_t-\tfrac12\kappa^2t\bigr).
$$

This [state-price density](../../../../../../state-price-density.md) prices the [bank account](../../../../../../bank-account.md) and the risky asset. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(\xi_tw_t)+\xi_tc_t\,dt=\xi_t(\sigma\theta_t-\kappa w_t)\,dW_t.
$$

Nonnegative wealth and consumption make the deflated cumulative gains a nonnegative [local martingale](../../../../../../local-martingale.md), hence a [supermartingale](../../../../../../supermartingale.md). Every admissible consumption stream therefore satisfies the [state-price budget constraint](../../../../../../state-price-budget-constraint.md) $\mathbb E\int_0^\infty\xi_tc_t\,dt\leq w_0$.

Write $I=(U')^{-1}$ for the [inverse marginal utility](../../../../../../inverse-marginal-utility.md). The [Inada conditions](../../../../../../inada-conditions.md) make $I$ decreasing from infinity to zero. A positive [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $y$ for the budget gives the pointwise condition $e^{-\rho t}U'(c_t)=y\xi_t$. Thus, whenever a finite optimum exists and a multiplier exhausts the budget,

$$
\boxed{c_t^*=I(ye^{\rho t}\xi_t),\qquad\mathbb E\int_0^\infty\xi_tI(ye^{\rho t}\xi_t)\,dt=w_0.}
$$

The [concave supporting-tangent inequality](../../../../../../concave-supporting-tangent-inequality.md), integrated against the budget, proves optimality. These curvature and endpoint assumptions alone do not ensure that the infinite-horizon value is finite; part (b) gives the exact additional condition for power utility.

The optimal wealth is the conditional price of remaining consumption:

$$
w_t^*=\xi_t^{-1}\mathbb E\left[\left.\int_t^\infty\xi_sc_s^*\,ds\right|\mathcal F_t\right].
$$

It is nonnegative. Apply the [Martingale representation theorem](../../../../../../martingale-representation-theorem.md) to the integrable total discounted consumption claim:

$$
M_t=\mathbb E\left[\left.\int_0^\infty\xi_sc_s^*\,ds\right|\mathcal F_t\right]
=w_0+\int_0^t\phi_s\,dW_s.
$$

Comparing $M_t=\xi_tw_t^*+\int_0^t\xi_sc_s^*ds$ with the deflated wealth equation yields

$$
\boxed{\theta_t^*=\frac1\sigma\left(\frac{\phi_t}{\xi_t}+\kappa w_t^*\right).}
$$

This constructs the portfolio without assuming extra smoothness of the [value function](../../../../../../value-function.md). If the stationary value $V$ is twice differentiable with $V''<0$, optimization of its [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) instead gives $\theta^*(w)=-(\mu-r)V'(w)/(\sigma^2V''(w))$ and $c^*(w)=I(V'(w))$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
