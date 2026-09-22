<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume the regime is observed and $\sigma_i=\sigma(i)>0$. With $\mu_i=\mu(i)$, the wealth dynamics are

$$
\boxed{dw_t=[rw_t+(\mu_{\xi_t}-r)\theta_t-c_t]dt+\sigma_{\xi_t}\theta_t\,dW_t.}
$$

Let $V_i(w)$ be the [value function](../../../../../value-function.md) conditional on the [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md) being in state $i$. Its generator adds $\sum_jq_{ij}V_j(w)$ to the diffusion generator. The [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
0=\sup_{c>0,\theta}\left\{U(c)+(rw+(\mu_i-r)\theta-c)V_i'
+\tfrac12\sigma_i^2\theta^2V_i''\right\}+\sum_jq_{ij}V_j-\rho V_i.
$$

For $V_i'>0$, $V_i''<0$, the maximizing controls are $c=I(V_i')$ and $\theta=-(\mu_i-r)V_i'/(\sigma_i^2V_i'')$. Put $\kappa_i=(\mu_i-r)/\sigma_i$. The optimized equation is

$$
0=\widehat U(V_i')+rwV_i'-\frac{\kappa_i^2(V_i')^2}{2V_i''}+\sum_jq_{ij}V_j-\rho V_i.
$$

Here $\widehat U$ is the [utility conjugate](../../../../../utility-conjugate.md).

Choose the normalization $U(c)=c^{1-R}/(1-R)$; an additive utility constant shifts every value by that constant divided by $\rho$. Homogeneity gives $V_i(w)=A_iw^{1-R}/(1-R)$ with $A_i>0$. The [regime-switching Merton equations](../../../../../regime-switching-merton-equations.md) reduce the differential system to one nonlinear algebraic equation per regime:

$$
\boxed{\left[\rho-(1-R)\left(r+\frac{\kappa_i^2}{2R}\right)\right]A_i
-\sum_jq_{ij}A_j-R A_i^{1-1/R}=0.}
$$

The candidate feedback controls are

$$
\boxed{c_i^*(w)=A_i^{-1/R}w,\qquad\theta_i^*(w)=\frac{\mu_i-r}{R\sigma_i^2}w.}
$$

Changing the regime changes consumption's wealth coefficient, while the risky fraction uses the current regime's risk premium and volatility.

Numerically solve these finite-dimensional equations by a damped [Newton method](../../../../../newton-s-method-in-optimization.md), using $A_i=e^{x_i}$ to enforce positivity. For $d_i=\rho-(1-R)(r+\kappa_i^2/(2R))$, the Jacobian in the $A$ variables is

$$
\frac{\partial F_i}{\partial A_j}=d_i\mathbf1_{\{i=j\}}-q_{ij}-(R-1)A_i^{-1/R}\mathbf1_{\{i=j\}}.
$$

Multiply its $j$th column by $A_j$ in the logarithmic variables. A residual-decreasing line search and continuation from $Q=0$, where the positive solution is the scalar Merton coefficient in each well-posed regime, give a practical method whenever that starting problem is finite. More generally use a positive initialization for the coupled system, and check residuals, positivity and conditioning rather than accepting an arbitrary algebraic root.

Verification requires constructing admissible feedback controls, proving the resulting wealth stays nonnegative, and establishing the stochastic-integral and transversality bounds needed at infinite horizon. Apply the [Itô formula for semimartingales with jumps](../../../../../ito-formula-for-semimartingales-with-jumps.md) to $e^{-\rho t}V_{\xi_t}(w_t)$, stopping before wealth leaves a compact interval. The [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) makes accumulated utility plus discounted candidate value a [local supermartingale](../../../../../local-supermartingale.md) for every admissible policy and a [local martingale](../../../../../local-martingale.md) under the feedback. Justify removal of localization and let the terminal discounted value vanish under the candidate. For $0<R<1$, the nonnegative terminal value can be dropped for the upper bound; for $R>1$ it is negative, so a transversality or dual integrability argument is essential. This establishes the global value bound and attainment, rather than just stationarity of the algebraic equations. The boundary is $V_i(0)=0$ for $R<1$ and the limiting value $-\infty$ for $R>1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
