<h1 id="b/6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Since $p$ is even, differentiating $c_i^p$ gives

$$
\boxed{\nabla_x\Phi(x,\mu)=\nabla f(x)+\frac1\mu\sum_i c_i(x)^{p-1}\nabla c_i(x).}
$$

At a stationary point define $y_i=-c_i(x)^{p-1}/\mu$. Then $\nabla f(x)-Dc(x)^Ty=0$, precisely the stationarity equation for the [optimization Lagrangian](../../../../../optimization-lagrangian.md). Bounded multipliers give

$$
\boxed{|c_i(x)|=(\mu|y_i|)^{1/(p-1)}\longrightarrow0.}
$$

Thus along any subsequence of stationary points with $x_\mu\to x_*$, a further subsequence of bounded multipliers converges to $y_*$, and continuity yields $c(x_*)=0$ and $\nabla f(x_*)-Dc(x_*)^Ty_*=0$. These are the equality-constrained first-order conditions. Bounded multipliers alone do not establish convergence of the primal points; the precise conclusion concerns their finite cluster points. This is the [power penalty multiplier limit](../../../../../power-penalty-multiplier-limit.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
