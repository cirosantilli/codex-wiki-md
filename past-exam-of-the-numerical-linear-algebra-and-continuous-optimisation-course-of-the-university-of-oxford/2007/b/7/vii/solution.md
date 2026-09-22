<h1 id="b/7/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Two reasons to prefer more advanced methods for smooth, high-accuracy optimization are:

- **Slow progress on ill-conditioned problems.** On an elongated quadratic level set, successive negative gradients can zigzag across the narrow valley. Convergence can be only linear with a factor close to one, and line search cannot remove the underlying poor scaling.
- **Failure to retain curvature information.** Each new step again uses only the current gradient. [Newton's method](../../../../../newton-s-method-in-optimization.md) and [quasi-Newton methods](../../../../../quasi-newton-method.md) exploit curvature to obtain substantially faster local convergence under suitable hypotheses, often compensating for their more expensive steps.

The question's blanket wording is too strong: the [steepest descent method](../../../../../gradient-descent-split.md) and related gradient algorithms are used in practice, especially when problem size, cheap gradients or simplicity make curvature-based alternatives costly. The objections describe limitations, not universal nonuse.

## ↑ Ancestors (13)

1. [Vii](../vii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
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
