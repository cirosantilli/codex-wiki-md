# User-network decomposition of concave utility maximization

↑ **Parent:** [Congestion control](congestion-control.md)

Maximize a sum of increasing strictly concave utilities $U_r(x_r)$ subject to $Ax\leq C$, $x\geq0$. Suppose capacities are positive, every route is nonempty, and $U_r'(0)=\infty$. At its unique positive optimizer $x^*$, the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) give nonnegative [resource congestion prices](resource-congestion-price.md) $p^*$ and [route congestion prices](route-congestion-price.md) $y_r^*=U_r'(x_r^*)$. Choosing $\nu_r^*=x_r^*e^{y_r^*}$ makes each user maximize $U_r(\nu_r e^{-y_r^*})-y_r^*\nu_r e^{-y_r^*}$ at $\nu_r^*$. It also makes $x^*$ maximize the [entropy maximization for loss-network occupancy](entropy-maximization-for-loss-network-occupancy.md) objective, since its gradient is $\log(\nu_r^*/x_r^*)=(A^Tp^*)_r$. Thus user and network optima implement the same system optimum.

## ↑ Ancestors (8)

1. [Congestion control](congestion-control.md)
2. [Stochastic network](stochastic-network.md)
3. [Queueing theory](queueing-theory-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/4/b/solution.md)
