# Square-root coordinates for primal congestion control

↑ **Parent:** [Global convergence of primal congestion control](global-convergence-of-primal-congestion-control.md)

For positive rates in [congestion control](congestion-control.md), put $x_r=\kappa_rz_r^2/4$ and $V(z)=U(x(z))$, where $U$ is the [primal congestion potential](primal-congestion-potential.md). The equation $\dot x_r=\kappa_rx_r\partial_rU$ becomes $\dot z_r=\partial_rV$. Positive logarithmic utility weights make $\sum_rw_r\log(\kappa_rz_r^2/4)$ strictly concave on the positive orthant. Each integrated nonnegative nondecreasing resource price is a convex nondecreasing function of its load; composing it with the convex quadratic load in $z$ preserves convexity. Hence $V$ is a [strictly concave function](strictly-concave-function.md), even for prices that are merely continuous. For two solutions, $\frac12\frac d{dt}\|z-\widetilde z\|^2=(z-\widetilde z)\cdot[\nabla V(z)-\nabla V(\widetilde z)]\leq0$. This proves uniqueness of the flow without assuming local Lipschitz continuity of the price functions.

## ↑ Ancestors (10)

1. [Global convergence of primal congestion control](global-convergence-of-primal-congestion-control.md)
2. [Primal congestion potential](primal-congestion-potential.md)
3. [Congestion control](congestion-control.md)
4. [Stochastic network](stochastic-network.md)
5. [Queueing theory](queueing-theory-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73/4/solution.md)
