<h1 id="b/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At an unconstrained local minimizer of a twice continuously differentiable [objective function](../../../../../objective-function.md), the [first-order optimality condition](../../../../../first-order-optimality-condition.md) is $\boxed{\nabla f(x_*)=0}$. The second-order necessary condition is $d^T\nabla^2f(x_*)d\geq0$ for every direction $d$, so the [Hessian matrix](../../../../../hessian-matrix.md) is positive semidefinite.

For the Euclidean norm, the unit [steepest descent direction](../../../../../steepest-descent-direction.md) is $-g/\|g\|_2$ when $g=\nabla f(x)\ne0$; the algorithm usually uses the unnormalized direction $p=-g$. It is a [descent direction](../../../../../descent-direction.md) because $\boxed{g^Tp=-\|g\|_2^2<0}$.

Two limitations of unpreconditioned [steepest descent method](../../../../../gradient-descent-split.md) in high-accuracy smooth optimization are its slow zigzagging on ill-conditioned valleys and its sensitivity to scaling of the coordinates. It uses no curvature information to correct those directions, so it can require many function and gradient evaluations compared with a suitable Newton or quasi-Newton method. These are reasons to prefer curvature-aware methods in that setting, rather than a claim that gradient-based methods are never useful.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
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
