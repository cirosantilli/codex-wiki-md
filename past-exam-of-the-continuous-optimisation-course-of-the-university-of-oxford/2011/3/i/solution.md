<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take the usual symmetric meaning of positive definite $Q$. To include all data allowed by the source, first check feasibility. Put

$$
B=AQ^{-1}A^T,\qquad x_0=Q^{-1}A^TB^{-1}b,\qquad
\rho^2=b^TB^{-1}b.
$$

Full row rank makes $B$ positive definite. Every $x$ satisfying $Ax=b$ is uniquely $x_0+z$ with $Az=0$, and $z^TQx_0=0$. Thus

$$
x^TQx=\rho^2+z^TQz.
$$

If $\rho^2>1$, there is no feasible point. If $\rho^2=1$, the only feasible point is $x_0$, and **$x_0$ is optimal for every $c$**. If $\rho^2<1$, the [Slater condition](../../../../slater-s-condition.md) holds, and the following [KKT conditions](../../../../karush-kuhn-tucker-conditions.md) are necessary and sufficient:

$$
\boxed{Ax=b,\quad x^TQx\leq1,\quad \gamma\geq0,\quad
c-A^Ty+2\gamma Qx=0,\quad\gamma(x^TQx-1)=0.}
$$

Necessity follows from the [constraint qualification](../../../../constraint-qualification.md) proved in (ii). Sufficiency follows from [convexity](../../../../convex-function.md): the stationary [optimization Lagrangian](../../../../optimization-lagrangian.md) $c^Tx+y^T(b-Ax)+\gamma(x^TQx-1)$ is minimized at $x$, while its feasible values never exceed the objective, and [complementary slackness](../../../../complementary-slackness.md) makes its value at $x$ equal the objective.

The singleton case cannot be silently covered by ordinary KKT necessity. For example, let $Q=I$, $A=(1\ 0)$, $b=1$, $c=(0,1)^T$. The sole feasible point $(1,0)$ is optimal, but stationarity would require $(0,1)$ to lie in the span of $(1,0)$, which is impossible. The feasibility split above supplies genuinely necessary and sufficient conditions without assuming an unprinted regularity hypothesis.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
