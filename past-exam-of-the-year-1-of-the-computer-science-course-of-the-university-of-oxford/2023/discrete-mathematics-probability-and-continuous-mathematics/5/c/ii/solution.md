<h1 id="5/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Convexity](../../../../../../convex-function.md) of the components of a [vector field](../../../../../../vector-field.md) is not the decisive criterion for a root-finding problem. Neither method becomes globally reliable merely because each component is [convex](../../../../../../convex-function.md).

Prefer the [Newton root-finding iteration](../../../../../../newton-root-finding-iteration.md) when the [Jacobian matrix](../../../../../../jacobian-matrix.md) is available accurately and at reasonable cost. Solve $J(\mathbf x_k)\mathbf s_k=-\mathbf f(\mathbf x_k)$ rather than explicitly forming an [inverse matrix](../../../../../../matrix-inverse-split.md). Near a root with a nonsingular [Jacobian matrix](../../../../../../jacobian-matrix.md) and a locally Lipschitz [Jacobian matrix](../../../../../../jacobian-matrix.md), the usual exact iteration has [quadratic convergence](../../../../../../quadratic-convergence.md).

Prefer [Broyden's method](../../../../../../broyden-s-method.md) when evaluating or differentiating the [vector field](../../../../../../vector-field.md) makes a fresh [Jacobian matrix](../../../../../../jacobian-matrix.md) expensive. It learns an approximate [Jacobian matrix](../../../../../../jacobian-matrix.md) through secant updates using function differences. Under appropriate local regularity and initialization assumptions it has [superlinear convergence](../../../../../../superlinear-convergence.md), generally slower asymptotically than the [quadratic convergence](../../../../../../quadratic-convergence.md) of exact Newton steps, but often with cheaper iterations.[pp. 577–579, cost of Jacobian evaluation and construction of updating methods.](../../../../../../a-class-of-methods-for-solving-nonlinear-simultaneous-equations-by-charles-george-broyden.md)

Dimension matters through storage and solves. A full dense Newton factorization costs order $d^3$ arithmetic operations; a dense Broyden approximation uses order $d^2$ storage, and maintained inverse or factorization updates can cost order $d^2$. A naive fresh dense solve can still cost order $d^3$. Sparsity can favour Newton, while very large $d$ can make either dense formulation unsuitable. Neither local rate guarantees convergence from an arbitrary starting point.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
