<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [constant relative risk aversion utility](../../../../../../constant-relative-risk-aversion-utility.md), $I(z)=z^{-1/R}$. Define the [Merton consumption constant](../../../../../../merton-consumption-constant.md)

$$
\gamma_M=\frac{\rho-(1-R)(r+\kappa^2/(2R))}{R}.
$$

The Gaussian exponential moment gives

$$
\mathbb E[\xi_t(ye^{\rho t}\xi_t)^{-1/R}]=y^{-1/R}e^{-\gamma_Mt}.
$$

When $\gamma_M>0$, the budget is $w_0=y^{-1/R}/\gamma_M$. Conditional pricing then gives $c_t^*=\gamma_Mw_t^*$, and the [Merton consumption-investment problem](../../../../../../merton-consumption-investment-problem.md) has

$$
\boxed{V(w)=\frac{\gamma_M^{-R}w^{1-R}}{1-R},\qquad c_t^*=\gamma_Mw_t^*,\qquad\theta_t^*=\frac{\mu-r}{R\sigma^2}w_t^*.}
$$

The resulting wealth is a [geometric Brownian motion](../../../../../../geometric-brownian-motion.md), so positive initial wealth remains positive. Substitution in the [Hamilton-Jacobi-Bellman equation](../../../../../../hamilton-jacobi-bellman-equation.md) verifies the first-order conditions and the value; the budget argument in part (a) supplies global optimality.

**The problem has a finite value precisely when $\gamma_M>0$.** For $0<R<1$ and $\gamma_M\leq0$, the supremum is $+\infty$. Indeed, use the displayed risky fraction and consumption $c_t=kw_t$, $k>0$. Its expected utility is

$$
\frac{w^{1-R}k^{1-R}}{1-R}\int_0^\infty e^{-[R\gamma_M+(1-R)k]t}\,dt.
$$

For $\gamma_M<0$, sufficiently small $k$ already gives infinite utility. For $\gamma_M=0$, the finite values tend to infinity as $k\downarrow0$.

For $R>1$ and $\gamma_M\leq0$, every admissible stream has utility $-\infty$. To see this, put $q=(R-1)/R$ and apply [Holder inequality](../../../../../../holder-inequality.md) on $[0,T]\times\Omega$:

$$
\int_0^T e^{-\gamma_Mt}\,dt
=\mathbb E\int_0^T(e^{-\rho t}c_t^{1-R})^{1/R}(\xi_tc_t)^{(R-1)/R}\,dt
\leq\left(\mathbb E\int_0^T e^{-\rho t}c_t^{1-R}dt\right)^{1/R}w_0^{(R-1)/R}.
$$

The left side diverges as $T\to\infty$, forcing the positive utility-cost integral to diverge. Thus there is no finite-value optimization problem in either ill-posed case.

## ↑ Ancestors (11)

1. [B](../b.md)
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
