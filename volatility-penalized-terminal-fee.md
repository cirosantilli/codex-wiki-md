# Volatility-penalized terminal fee

↑ **Parent:** [Constant relative risk aversion utility](constant-relative-risk-aversion-utility.md)

A fee proportional to terminal [portfolio wealth](portfolio-wealth.md) but reduced by accumulated portfolio [quadratic variation](quadratic-variation.md) changes the optimal risk exposure of a manager with [constant relative risk aversion utility](constant-relative-risk-aversion-utility.md). Write $A=\sigma\sigma^T$, $b=\mu-r\mathbf1$ and assume $A$ is invertible. The fee process has drift $r+b^T\pi-\varepsilon\pi^TA\pi/2$ and volatility $\sigma^T\pi$. Its [Hamilton-Jacobi-Bellman equation](hamilton-jacobi-bellman-equation.md) therefore maximizes $b^T\pi-(R+\varepsilon)\pi^TA\pi/2$, giving $\pi^*=A^{-1}b/(R+\varepsilon)$. The fee increases effective relative risk aversion from $R$ to $R+\varepsilon$, independently of its positive scale $a$.

There is also a direct global bound. Put $p=1-R$, $v^*=\sigma^T\pi^*$, and tilt probability by $\exp(pv^*\cdot W_T-p^2|v^*|^2T/2)$. Under this probability let $Z$ be the [stochastic exponential](doleans-dade-exponential.md) of $(1+\varepsilon)\int(\sigma^T\pi-v^*)\cdot dW^*$. The terminal fee ratio satisfies $(y_T/y_T^*)^p=Z_T^{p/(1+\varepsilon)}$. A nonnegative [local martingale](local-martingale.md) has expectation at most one. The [Jensen inequality](jensen-s-inequality.md), applied to a concave positive power when $p>0$ and a convex negative power when $p<0$, proves that the constant exposure maximizes expected [CRRA utility](constant-relative-risk-aversion-utility.md). Effective risk aversion one uses logarithmic utility.

## ↑ Ancestors (7)

1. [Constant relative risk aversion utility](constant-relative-risk-aversion-utility.md)
2. [Utility function](utility-function-split.md)
3. [Mathematical finance](mathematical-finance-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39/1/solution.md)
