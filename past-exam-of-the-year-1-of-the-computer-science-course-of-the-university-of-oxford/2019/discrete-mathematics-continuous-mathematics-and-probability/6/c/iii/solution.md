<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**At $d=1000$, [gradient descent](../../../../../../gradient-descent-split.md) and full [BFGS](../../../../../../bfgs-method.md) are practical candidates; a dense [Newton method](../../../../../../newton-s-method-in-optimization.md) can also be feasible, but its extra work and indefinite curvature need attention.** The number of examples $n$, data sparsity and conditioning still matter.

For dense $A$, a [gradient](../../../../../../gradient.md) evaluation costs $O(nd)$ arithmetic, with $O(d)$ working storage beyond the data and accumulation buffers. [Gradient descent](../../../../../../gradient-descent-split.md) is inexpensive per iteration and, with an appropriate [line search](../../../../../../line-search.md), follows a [descent direction](../../../../../../descent-direction.md), but poor conditioning can make it slow.

Forming the [Hessian matrix](../../../../../../hessian-matrix.md) explicitly costs $O(nd^2)$ arithmetic, and a dense [Newton method](../../../../../../newton-s-method-in-optimization.md) solve costs $O(d^3)$. A $1000$-square double-precision [matrix](../../../../../../matrix.md) uses about $8$ MB, so storage alone is manageable, but repeated factorization may be expensive. Because the [Hessian matrix](../../../../../../hessian-matrix.md) can be indefinite or singular, an unmodified [Newton step](../../../../../../newton-step.md) need not decrease the loss; a modified Hessian, damping or a [trust region](../../../../../../trust-region.md) is appropriate.

Full [BFGS](../../../../../../bfgs-method.md) uses [gradients](../../../../../../gradient.md) and an $O(d^2)$ curvature approximation, avoiding explicit second [derivatives](../../../../../../derivative.md). Its rank-two updates and direction calculation cost $O(d^2)$ per step and require roughly the same [matrix](../../../../../../matrix.md) storage. A positive-definite initial approximation with safeguarded curvature updates and a suitable [line search](../../../../../../line-search.md) preserves [descent directions](../../../../../../descent-direction.md). For this scale it is often a good compromise, without guaranteeing a global minimum.[Secant condition, positive-definite updating, and quadratic per-step operation/storage costs](../../../../../../quasi-newton-methods-by-neos-guide.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
