<h1 id="b/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At the current point $x$, a [trust-region method](../../../../../trust-region-method.md) approximately minimizes a local quadratic model

$$
m(s)=f(x)+g(x)^Ts+\frac12s^TBs\qquad\text{subject to }\|s\|_2\leq\Delta,
$$

where $B$ is a symmetric Hessian approximation and $\Delta>0$ is the trust-region radius. For a step with positive predicted decrease, compare the true and predicted reductions through

$$
\boxed{\rho=\frac{f(x)-f(x+s)}{m(0)-m(s)}.}
$$

Choose fixed thresholds $0<\eta_1<\eta_2<1$. If $\rho<\eta_1$, the step is unsuccessful: reject it and reduce the radius. If $\eta_1\leq\rho<\eta_2$, accept the successful step and normally retain the radius. If $\rho\geq\eta_2$, the step is very successful: accept it and permit an increase in radius, especially when the step reaches its boundary. The ratio tests whether the local model is accurate enough to justify moving. An approximate subproblem solver should deliver at least the model decrease achieved at the [Cauchy point](../../../../../cauchy-point.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
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
