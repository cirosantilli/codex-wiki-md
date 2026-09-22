<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

The reservation bid price for a claim $Y$ is the fixed cash payment $p_i(Y)$ which leaves the agent indifferent: $E[U_i(X_i+Y-p_i(Y))]=E[U_i(X_i)]$. For Gaussian wealth $W$, [exponential utility](../../../../../constant-absolute-risk-aversion-utility.md) is $-\exp[-\gamma_iE(W)+\gamma_i^2\operatorname{Var}(W)/2]$, so its [certainty equivalent](../../../../../certainty-equivalent.md) is $E(W)-\gamma_i\operatorname{Var}(W)/2$. For $Y=\lambda X_0$, subtracting the original [certainty equivalent](../../../../../certainty-equivalent.md) gives

$$
\boxed{p_i(\lambda)=-\tfrac12\gamma_i(\lambda^2v_{00}+2\lambda v_{0i}),\qquad\lim_{\lambda\to0}\frac{p_i(\lambda)}\lambda=-\gamma_i v_{0i}.}
$$

The marginal price is positive when the claim hedges the agent's endowment, negative when it adds positively correlated risk, and zero for an uncorrelated zero-mean infinitesimal position.

Assume $v_{00}>0$, so the claim is nontrivial. Buying $\theta$ units at per-unit price $p$ changes the [certainty equivalent](../../../../../certainty-equivalent.md) by $-(p+\gamma_iv_{0i})\theta-\gamma_iv_{00}\theta^2/2$. This strictly concave quadratic is maximized at $\theta_i=-(p+\gamma_iv_{0i})/(\gamma_iv_{00})$. Market clearing $\sum_i\theta_i=0$ gives

$$
\boxed{p=-\Gamma\sum_i v_{0i},\qquad\Gamma^{-1}=\sum_i\gamma_i^{-1},\qquad\theta_i=\frac{\Gamma v_{0\bullet}-\gamma_iv_{0i}}{\gamma_iv_{00}}.}
$$

At the optimum the certainty-equivalent gain is

$$
\boxed{\Delta_i=\frac{(\gamma_i v_{0i}-\Gamma v_{0\bullet})^2}{2\gamma_i v_{00}}.}
$$

The maximal expected utility equals the original negative utility multiplied by $e^{-\gamma_i\Delta_i}$, hence is improved. Paying a fixed amount $\Delta_i$ removes exactly that gain, proving it is the fixed-payment value of market access. If $v_{00}=0$, the Gaussian claim vanishes almost surely, all its [covariances](../../../../../covariance.md) vanish, and the appropriate price and access value are zero; the printed formulas with a [variance](../../../../../variance-split.md) denominator require the nontrivial-claim assumption.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
