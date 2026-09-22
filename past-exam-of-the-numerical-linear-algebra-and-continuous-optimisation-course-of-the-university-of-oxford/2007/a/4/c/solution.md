<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One restarted step chooses $x_j=x_{j-1}+\alpha_jr_{j-1}$ to minimize the new residual norm. Since $r_{j-1}=A(x-x_{j-1})$,

$$
x-x_j=(I-\alpha_jA)(x-x_{j-1}),
$$

and induction gives

$$
\boxed{x-x_k=q_k(A)\cdots q_1(A)(x-x_0),\qquad q_j(t)=1-\alpha_jt.}
$$

These polynomials have degree at most one; a zero step gives the constant polynomial one.

In the specified example the first search space is spanned by $b=(1,1)^T$. Writing $x_1=\alpha b$, its squared residual norm is $(1-\alpha)^2+(1+\alpha)^2=2+2\alpha^2$, uniquely minimized at $\alpha=0$. Thus restarted [GMRES](../../../../../generalized-minimal-residual-method.md) gives $\boxed{x_1=x_2=(0,0)^T}$ and stagnates forever, repeatedly facing the same minimization problem.

Without restarting, the first iterate is still zero, but $K_2(A,b)=\operatorname{span}\{(1,1)^T,(1,-1)^T\}=\mathbb R^2$. The second minimization finds the exact solution $\boxed{x_2=(1,-1)^T}$. This [one-step restarted GMRES stagnation example](../../../../../one-step-restarted-gmres-stagnation-example.md) shows how discarding the accumulated search space can prevent convergence even for a nonsingular two-dimensional system.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
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
