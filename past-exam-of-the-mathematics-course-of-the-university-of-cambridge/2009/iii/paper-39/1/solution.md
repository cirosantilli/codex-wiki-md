<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $p=1-R$, $b=\mu-r\mathbf1$, $A=\sigma\sigma^T$ and $q=R+\varepsilon$. First assume the [covariance matrix](../../../../../covariance-matrix.md) $A$ is invertible and initial [portfolio wealth](../../../../../portfolio-wealth.md) is positive. Introduce the accumulated fee process

$$
y_t=aw_t\exp\left(-\frac{\varepsilon}{2}\int_0^t\pi_s^TA\pi_sds\right).
$$

The [Itô formula](../../../../../ito-s-lemma.md) and the [self-financing portfolio](../../../../../self-financing-portfolio.md) equation give

$$
\frac{dy_t}{y_t}=\left(r+b^T\pi_t-\frac{\varepsilon}{2}\pi_t^TA\pi_t\right)dt+\pi_t^T\sigma\,dW_t.
$$

This converts the path-dependent payment into a terminal-utility problem with state $y$. The [volatility-penalized terminal fee](../../../../../volatility-penalized-terminal-fee.md) changes its [drift](../../../../../drift-coefficient.md) as well as its [spot volatility](../../../../../spot-volatility.md).

Let $J(t,y)$ be the manager's [value function](../../../../../value-function.md). Its [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md), with terminal condition $J(T,y)=y^p/p$, is

$$
0=J_t+ryJ_y+\sup_\pi\left\{yJ_yb^T\pi+\frac12\left(y^2J_{yy}-\varepsilon yJ_y\right)\pi^TA\pi\right\}.
$$

The [homogeneity](../../../../../homogeneity.md) of [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) suggests $J(t,y)=f(t)y^p/p$. Since $yJ_y=f(t)y^p$ and $y^2J_{yy}=-Rf(t)y^p$, the portfolio-dependent expression is

$$
f(t)y^p\left(b^T\pi-\frac q2\pi^TA\pi\right).
$$

Its coefficient is positive even when $p<0$. [Completing the square](../../../../../completing-the-square.md) gives

$$
b^T\pi-\frac q2\pi^TA\pi
=\frac{b^TA^{-1}b}{2q}-\frac q2(\pi-\pi^*)^TA(\pi-\pi^*),
\qquad
\boxed{\pi^*=\frac{A^{-1}(\mu-r\mathbf1)}{R+\varepsilon}}.
$$

Thus the [stock](../../../../../stock.md) fractions are constant. Substitution into the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) yields

$$
f(t)=\exp\left[p\left(r+\frac{b^TA^{-1}b}{2q}\right)(T-t)\right],
\qquad
J(0,aw_0)=\frac{(aw_0)^p}{p}\exp\left[p\left(r+\frac{b^TA^{-1}b}{2q}\right)T\right].
$$

In particular, multiplying the fee by $a$ does not affect the optimal [investment portfolio](../../../../../investment-portfolio.md).

To prove global optimality rather than merely solve a formal [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md), write $v_t=\sigma^T\pi_t$, $v^*=\sigma^T\pi^*$ and let $y^*$ be the fee under the proposed constant policy. Then $b^T\pi=qv^*\cdot v$. Define a probability $Q$ by

$$
\frac{dQ}{dP}=\exp\left(pv^*\cdot W_T-\frac12p^2|v^*|^2T\right).
$$

This density is a true [martingale](../../../../../martingale-split.md) because $v^*$ is constant. By the [Girsanov theorem](../../../../../girsanov-theorem.md), $W_t^Q=W_t-pv^*t$ is a [Brownian motion](../../../../../brownian-motion-split.md) under $Q$. The [geometric Brownian motion](../../../../../geometric-brownian-motion.md) formula for the fee ratio gives

$$
\log\frac{y_T}{y_T^*}
=\int_0^T(v_s-v^*)\cdot dW_s^Q-\frac{1+\varepsilon}{2}\int_0^T|v_s-v^*|^2ds.
$$

For admissible, locally square-integrable exposures with finite accumulated [quadratic variation](../../../../../quadratic-variation.md), set

$$
Z_T=\exp\left((1+\varepsilon)\int_0^T(v_s-v^*)\cdot dW_s^Q-\frac{(1+\varepsilon)^2}{2}\int_0^T|v_s-v^*|^2ds\right).
$$

This [stochastic exponential](../../../../../doleans-dade-exponential.md) is a positive [local martingale](../../../../../local-martingale.md), so $E_QZ_T\leq1$. Moreover,

$$
\left(\frac{y_T}{y_T^*}\right)^p=Z_T^{p/(1+\varepsilon)},
\qquad
E_P[y_T^p]=E_P[(y_T^*)^p]E_Q[Z_T^{p/(1+\varepsilon)}].
$$

For $p>0$, the exponent $p/(1+\varepsilon)$ lies between zero and one. The [Jensen inequality](../../../../../jensen-s-inequality.md) for this [concave function](../../../../../concave-function.md) gives $E_Q[Z_T^{p/(1+\varepsilon)}]\leq1$. For $p<0$, the power is [convex](../../../../../convex-function.md) and decreasing, so the [Jensen inequality](../../../../../jensen-s-inequality.md) gives $E_Q[Z_T^{p/(1+\varepsilon)}]\geq(E_QZ_T)^{p/(1+\varepsilon)}\geq1$; an infinite moment only makes this inequality stronger. Dividing by $p$, with its corresponding sign, proves $E[U(y_T)]\leq E[U(y_T^*)]$ in both cases. Equality is achieved by the constant policy.

For an ordinary terminal-wealth agent with relative risk aversion $q$, the same [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) calculation, with no fee penalty, maximizes $b^T\pi-q\pi^TA\pi/2$. It therefore gives exactly the same optimal [investment portfolio](../../../../../investment-portfolio.md). For $q\ne1$, the preceding [stochastic exponential](../../../../../doleans-dade-exponential.md) and [Jensen inequality](../../../../../jensen-s-inequality.md) verification applies with penalty zero and exponent $1-q$, proving global optimality for this agent too. **The [spot volatility](../../../../../spot-volatility.md) penalty adds $\varepsilon$ to effective relative risk aversion.** If $q=1$, the printed expression for $U_0$ has a zero denominator; its appropriate limit, after subtracting an irrelevant constant, is $U_0(x)=\log x$, which still gives $\pi^*=A^{-1}b$. In this logarithmic case, the terminal log-wealth difference from the candidate equals $\log Z_T$ for a positive [stochastic exponential](../../../../../doleans-dade-exponential.md) $Z$, so $E[\log Z_T]\leq\log E[Z_T]\leq0$ proves its optimality.

If $A$ is singular, the same conclusion holds in the absence of [arbitrage](../../../../../arbitrage.md), provided $b$ lies in the [image of a linear map](../../../../../image-of-a-linear-map.md) $x\mapsto Ax$: replace $A^{-1}$ by the [Moore-Penrose inverse](../../../../../moore-penrose-inverse.md), and add any vector in the [kernel](../../../../../kernel-of-a-linear-map.md) of $A$ to $\pi^*$. These additions change neither returns nor [Brownian portfolio exposures](../../../../../brownian-portfolio-exposures.md). If $b$ has a nonzero component in that [kernel](../../../../../kernel-of-a-linear-map.md), a zero-volatility position has a nonzero excess return. Scaling its profitable sign gives [arbitrage](../../../../../arbitrage.md), so a finite attained optimum as claimed requires this degeneracy to be excluded.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
