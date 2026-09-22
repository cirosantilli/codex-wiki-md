<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A local minimizer of a [differentiable function](../../../../../differentiable-function.md) on $\mathbb R^N$ necessarily satisfies $\boxed{\nabla f(x_*)=0}$. A sufficient condition for a strict local minimum is $\boxed{\nabla f(x_*)=0,\quad\nabla^2f(x_*)\text{ positive definite}}$. Indeed, the second-order [Taylor expansion](../../../../../taylor-expansion.md) has a strictly positive quadratic term that dominates its $o(\|x-x_*\|^2)$ remainder near $x_*$.

For [Newton's method](../../../../../newton-s-method-in-optimization.md), solve $H_ns_n=-g_n$ with $H_n=\nabla^2f(x_n)$, $g_n=\nabla f(x_n)$, and set $x_{n+1}=x_n+s_n$. A positive-definite Hessian makes this a [descent direction](../../../../../descent-direction.md); general Hessians may need modification or a separate [line search](../../../../../line-search.md) for a globally useful method.

The sequence is q-quadratically convergent if there is $C<\infty$ such that $\|x_{n+1}-x_*\|\leq C\|x_n-x_*\|^2$ eventually. Sufficient local hypotheses are $\nabla f(x_*)=0$, a nonsingular $H_*=\nabla^2f(x_*)$, a [Lipschitz continuous](../../../../../lipschitz-continuity.md) Hessian near $x_*$, and $x_0$ sufficiently close. For convergence to a local minimum take $H_*$ positive definite. Near $x_*$, inverse Hessians are uniformly bounded, and integration along the error segment gives

$$
x_{n+1}-x_*=H_n^{-1}\int_0^1[H_n-\nabla^2f(x_*+t(x_n-x_*))](x_n-x_*)\,dt.
$$

A Hessian Lipschitz constant $L_H$ yields $\|x_{n+1}-x_*\|\leq\tfrac12L_H\|H_n^{-1}\|\|x_n-x_*\|^2$. Choosing a sufficiently small invariant neighborhood proves [quadratic convergence](../../../../../quadratic-convergence.md). Continuous second derivatives alone do not guarantee this quadratic rate; the Lipschitz hypothesis supplies the needed remainder bound.

## ↑ Ancestors (13)

1. [A](../a.md)
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
