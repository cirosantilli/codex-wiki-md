# Global convergence of primal congestion control

↑ **Parent:** [Primal congestion potential](primal-congestion-potential.md)

Assume finitely many nonempty routes, positive weights and adjustment rates, and continuous nonnegative nondecreasing resource prices. Each route must meet a resource whose price is positive somewhere. Then the [primal congestion potential](primal-congestion-potential.md) has compact superlevel sets inside the positive orthant and a unique maximum. Along [gradient flow with diagonal mobility](gradient-flow-with-diagonal-mobility.md), $\dot U=\sum_r\kappa_rx_r(\partial_rU)^2$. The substitution $x_r=\kappa_rz_r^2/4$ makes the dynamics ordinary [gradient flow](gradient-flow.md) ascent for $V(z)=U((\kappa_rz_r^2/4)_r)$. This $V$ is [strictly concave](strictly-concave-function.md): the logarithmic terms are strictly concave, and each integrated price is convex and nondecreasing, composed with a convex quadratic load. Thus its continuous gradient is monotone decreasing, which proves uniqueness of trajectories even without differentiability of the prices. Compact trapping and the dissipation identity force every limit point to be the unique maximizer. If every price on some route vanishes identically, its rate instead grows linearly and there is no equilibrium.

**Table of contents**

- [Square-root coordinates for primal congestion control](square-root-coordinates-for-primal-congestion-control.md)

## ↑ Ancestors (9)

1. [Primal congestion potential](primal-congestion-potential.md)
2. [Congestion control](congestion-control.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30/4/solution.md)
