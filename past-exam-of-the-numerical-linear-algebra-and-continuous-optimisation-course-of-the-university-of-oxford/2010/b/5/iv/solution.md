<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The linearized constraints may be inconsistent, for example when $-c(x_k)$ is not in the [image of a linear map](../../../../../image-of-a-linear-map.md) defined by $A(x_k)$. Even if feasible, the quadratic objective may have negative curvature along its feasible tangent space, making it unbounded below and leaving no local minimizer.

Fletcher's [Sℓ1QP](../../../../../sl1qp.md) replaces the hard linearized constraints by an [L1 exact penalty](../../../../../l1-exact-penalty.md) and bounds the step inside a [trust region](../../../../../trust-region.md). One usual form is

$$
\boxed{\min_{\|s\|_\infty\leq\Delta_k}\ g_k^Ts+\frac12s^TH_ks+\rho_k\|c_k+A_ks\|_1,\qquad\rho_k>0.}
$$

The zero step is always admissible. The trust region is compact, so a minimum exists even when the model [Hessian matrix](../../../../../hessian-matrix.md) is indefinite; the constraint penalty measures infeasibility rather than making the subproblem impossible to solve. Adjusting its weight promotes feasibility, while the radius keeps the local model within a controlled neighbourhood. Introducing nonnegative positive- and negative-part slack variables converts the absolute values to an equivalent smooth [quadratic program](../../../../../quadratic-program.md) with box constraints.[§3.3, equations (3.25)–(3.26): Fletcher's Sℓ1-QP model and its elastic quadratic-program formulation](../../../../../sequential-quadratic-programming-methods-by-philip-e-gill-and-elizabeth-wong.md)

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
