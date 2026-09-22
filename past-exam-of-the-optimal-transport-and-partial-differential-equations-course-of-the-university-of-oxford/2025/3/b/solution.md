<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a candidate curve $\rho$, define the [velocity field](../../../../velocity-field.md) by the [convolution](../../../../convolution.md)

$$
b_\rho(t,x)=K*\rho_t(x)=-\int J\nabla W(x-z)\,d\rho_t(z).
$$

It is well defined with a finite first [absolute moment](../../../../absolute-moment.md), because $|K(x-z)|\leq L(|x|+|z|)$. Equality of mixed [partial derivatives](../../../../partial-derivative.md) gives

$$
\operatorname{div}K=\partial_xW_y-\partial_yW_x=0,\qquad\operatorname{div}b_\rho=0.
$$

The [Hessian matrix](../../../../hessian-matrix.md) bound justifies moving a spatial derivative through this [convolution](../../../../convolution.md). For smooth densities, the [transport equation](../../../../transport-equation-split.md) consequently becomes the [continuity equation](../../../../continuity-equation.md)

$$
\boxed{\partial_t\rho+\operatorname{div}(b_\rho\rho)=0.}
$$

This form defines the equation for singular [probability measures](../../../../probability-measure.md) as well. With initial [probability measure](../../../../probability-measure.md) $\rho_0$, a [weak solution](../../../../weak-solution.md) is a curve in $C([0,\infty),\mathcal P_1)$ such that every $\varphi\in C_c^1([0,\infty)\times\mathbb R^2)$ satisfies

$$
\boxed{\int_0^\infty\!\int\left[\partial_t\varphi(t,x)+b_\rho(t,x)\cdot\nabla\varphi(t,x)\right]d\rho_t(x)\,dt+\int\varphi(0,x)\,d\rho_0(x)=0.}
$$

Using smooth [test functions](../../../../test-function.md) gives the same definition by approximation on compact sets. Continuity in the [Wasserstein distance](../../../../wasserstein-distance.md) bounds first [absolute moments](../../../../absolute-moment.md) on compact time intervals, so the displayed integrals exist.

For the [empirical measure](../../../../empirical-measure.md), the [chain rule](../../../../chain-rule.md) and the particle equations give

$$
\begin{aligned}
\frac d{dt}\int\varphi(t,x)\,d\mu_t^N(x)&=\frac1N\sum_i\left[\partial_t\varphi(t,X^i)+\nabla\varphi(t,X^i)\cdot\dot X^i\right]\\
&=\int\left[\partial_t\varphi+b_{\mu^N}\cdot\nabla\varphi\right]d\mu_t^N.
\end{aligned}
$$

Integrating in time, with zero terminal contribution because $\varphi$ has compact [support](../../../../support.md), gives precisely the weak identity and the correct initial [empirical measure](../../../../empirical-measure.md). Thus **$\mu^N$ is a global weak solution**. The self-interaction term vanishes since $K(0)=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
