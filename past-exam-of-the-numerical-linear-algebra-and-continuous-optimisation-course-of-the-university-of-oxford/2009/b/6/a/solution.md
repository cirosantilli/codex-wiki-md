<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [contingent tangent cone](../../../../../contingent-tangent-cone.md) consists of feasible first-order velocities:

$$
\boxed{T_\Omega(x)=\{d:\exists t_n\downarrow0,\ x_n\in\Omega,\ (x_n-x)/t_n\to d\}.}
$$

If $x_*$ is a local minimizer, then $\boxed{\nabla f(x_*)^Td\geq0\text{ for every }d\in T_\Omega(x_*)}$. Indeed, $x_n\to x_*$ along the defining sequence, so eventually $f(x_n)-f(x_*)\geq0$. Differentiability gives

$$
\frac{f(x_n)-f(x_*)}{t_n}=\nabla f(x_*)^T\frac{x_n-x_*}{t_n}+o(1)\longrightarrow\nabla f(x_*)^Td.
$$

This proves the inequality. Using feasible limiting velocities avoids assuming that every tangent direction is realized by a straight segment staying in the feasible set.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
