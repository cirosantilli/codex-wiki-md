<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $J(x)=DR(x)$, with one residual gradient per row. The [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{\nabla f(x)=\sum_jR^{(j)}(x)\nabla R^{(j)}(x)=J(x)^TR(x).}
$$

Differentiating each product gives

$$
\boxed{\nabla^2f(x)=J(x)^TJ(x)+\sum_jR^{(j)}(x)\nabla^2R^{(j)}(x).}
$$

The approximation $B_n=J(x_n)^TJ(x_n)$ defines the [Gauss-Newton method](../../../../../gauss-newton-algorithm.md). It is symmetric, and full column rank gives $v^TB_nv=\|J(x_n)v\|_2^2>0$ for $v\ne0$, so the step is well-defined.

If $x_n\to x_*$, $R(x_*)=0$ and $J(x_*)$ has full column rank, then $\nabla f(x_*)=0$ and $H_*=\nabla^2f(x_*)=J(x_*)^TJ(x_*)$ is positive definite. Continuity of $J$ gives $B_n\to H_*$. Therefore

$$
\frac{\|(B_n-H_*)s_n\|}{\|s_n\|}\leq\|B_n-H_*\|\to0.
$$

The [Dennis-Moré condition](../../../../../dennis-more-condition.md) applies, proving $\boxed{x_n\to x_*\text{ q-superlinearly}}$, or finite termination. The zero-residual hypothesis is what makes the discarded second-derivative term vanish at the limit.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
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
