<h1 id="5/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Gradient descent](../../../../../../gradient-descent-split.md) uses only the current [gradient](../../../../../../gradient.md) and a suitable [step size](../../../../../../step-size.md); its additional storage is order $d$. It is attractive for very large $d$ or when low per-iteration cost matters most. For a smooth [strongly convex function](../../../../../../strongly-convex-function.md), standard step choices give [linear convergence](../../../../../../linear-convergence.md), with a rate sensitive to the [condition number](../../../../../../condition-number.md). Mere [convexity](../../../../../../convex-function.md) gives a global-minimum interpretation but does not alone imply a linear rate; for nonconvex objectives the usual guarantee concerns stationary points.

[BFGS](../../../../../../bfgs-method.md) uses successive [gradients](../../../../../../gradient.md) to update an approximation to inverse curvature, incorporating information that can correct poor scaling. Full [BFGS](../../../../../../bfgs-method.md) uses order $d^2$ storage and update work. With suitable [line searches](../../../../../../line-search.md) and local smoothness and positive-curvature assumptions near a nondegenerate [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md), it has [superlinear convergence](../../../../../../superlinear-convergence.md). This often favours it in moderate dimensions when gradients are not extremely cheap relative to the extra work.

Neither [gradient descent](../../../../../../gradient-descent-split.md) nor [BFGS](../../../../../../bfgs-method.md) requires an explicitly evaluated [Hessian matrix](../../../../../../hessian-matrix.md). Thus an expensive [Hessian matrix](../../../../../../hessian-matrix.md) is compatible with both, rather than a reason to reject [BFGS](../../../../../../bfgs-method.md). If an accurate [Hessian matrix](../../../../../../hessian-matrix.md) and its factorization are exceptionally cheap, [Newton's method in optimization](../../../../../../newton-s-method-in-optimization.md) becomes an additional reasonable option. [Convexity](../../../../../../convex-function.md) helps identify a stationary point as a global [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md); without it, both methods need suitable descent and curvature safeguards. The [BFGS](../../../../../../bfgs-method.md) update learns curvature from the [Quasi-Newton secant equation](../../../../../../quasi-newton-secant-equation.md).[Quasi-Newton condition and the BFGS member of the low-rank updating family.](../../../../../../quasi-newton-methods-by-neos-guide.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
