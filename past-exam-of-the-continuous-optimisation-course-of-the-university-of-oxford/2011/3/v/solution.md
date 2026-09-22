<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For fixed $y$, $s=c-A^Ty$ is fixed. The relaxed inequality and $\theta\geq0$ say precisely

$$
\theta\geq\sqrt{s^TQ^{-1}s}.
$$

The objective $b^Ty-\theta$ strictly decreases with $\theta$, so its best choice is always equality. Replacing any feasible relaxed point by that choice preserves feasibility and improves or leaves unchanged the objective. Conversely every point satisfying equality is feasible for the relaxed problem. Thus **the two dual formulations have the same optimal value and the same optimal $y,s$**, with equality at any optimizer.

This algebraic equivalence in fact does not require [Slater's condition](../../../../slater-s-condition.md). Under the stipulated condition, [strong duality](../../../../strong-duality.md) additionally identifies their attained optimum with the primal optimum. With $Q^{-1/2}s$ as a linear coordinate, the relaxed constraint is $\|Q^{-1/2}s\|_2\leq\theta$, so the relaxed formulation is a [second-order cone program](../../../../second-order-cone-programming.md).

## ↑ Ancestors (12)

1. [V](../v.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
