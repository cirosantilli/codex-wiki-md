<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [quasi-Newton method](../../../../../quasi-newton-method.md) replaces the Hessian in the Newton system by an efficiently updated approximation $B_n$:

$$
\boxed{B_ns_n=-\nabla f(x_n),\qquad x_{n+1}=x_n+s_n.}
$$

The matrices must be nonsingular for the step to exist. Symmetry reflects the true Hessian, and positive definiteness makes every nonzero step a [descent direction](../../../../../descent-direction.md), since $\nabla f(x_n)^Ts_n=-s_n^TB_ns_n<0$. Secant updates often enforce the [Quasi-Newton secant equation](../../../../../quasi-newton-secant-equation.md) $B_{n+1}s_n=\nabla f(x_{n+1})-\nabla f(x_n)$.

Q-[superlinear convergence](../../../../../superlinear-convergence.md) means $\|x_{n+1}-x_*\|/\|x_n-x_*\|\to0$, unless the sequence terminates exactly. A sufficient [Dennis-Moré condition](../../../../../dennis-more-condition.md) is

$$
\boxed{\frac{\|(B_n-H_*)s_n\|}{\|s_n\|}\to0,\qquad H_*=\nabla^2f(x_*),}
$$

assuming $x_n\to x_*$, $\nabla f(x_*)=0$, continuous Hessian near $x_*$ and nonsingular $H_*$. Only accuracy on the actual step direction is required; full matrix convergence $B_n\to H_*$ is sufficient but stronger.

To prove the assertion, continuity of the Hessian along the short segment from $x_n$ to $x_{n+1}$ gives

$$
\nabla f(x_{n+1})=\nabla f(x_n)+H_*s_n+o(\|s_n\|)=-(B_n-H_*)s_n+o(\|s_n\|)=o(\|s_n\|).
$$

Nonsingularity of $H_*$ and $\nabla f(x_*+e)=H_*e+o(\|e\|)$ give a constant $C$ with $\|e\|\leq C\|\nabla f(x_*+e)\|$ near zero. Writing $e_n=x_n-x_*$, we obtain

$$
\|e_{n+1}\|\leq\varepsilon_n\|s_n\|\leq\varepsilon_n(\|e_n\|+\|e_{n+1}\|),\qquad\varepsilon_n\to0.
$$

Thus $\|e_{n+1}\|/\|e_n\|\leq\varepsilon_n/(1-\varepsilon_n)\to0$. This proves sufficiency. It is a local rate result for an already convergent sequence, not a claim that arbitrary unmodified quasi-Newton iterations converge from every starting point.

## ↑ Ancestors (13)

1. [B](../b.md)
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
