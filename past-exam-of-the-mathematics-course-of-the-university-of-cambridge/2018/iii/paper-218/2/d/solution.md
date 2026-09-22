<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First use the dual convention for [support vectors](../../../../../../support-vector.md), and interpret the stipulated uniqueness as applying to each training fit. If $\alpha_j=0$, the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) in the preceding part give $\xi_j=0$ and $y_jf(x_j)\geq1$. Delete the $j$th primal variable and its zero dual coefficient. All remaining primal constraints, stationarity equations and complementary-slackness equations still hold with the same $w,b$. These conditions certify a global minimizer of the reduced [convex optimization](../../../../../../convex-optimization-split.md) problem, since the objective is convex and the [Slater condition](../../../../../../slater-s-condition.md) holds by choosing positive large slacks. Uniqueness therefore gives exactly the same fitted score and [support-vector-machine decision boundary](../../../../../../support-vector-machine-decision-boundary.md). The omitted point is correctly classified.

For the geometric convention, a non-support point has strict margin $y_jf(x_j)>1$. One can obtain the same conclusion using just uniqueness of the full fit: if the reduced problem had another optimizer, the convex segment from the original optimizer toward it would also consist of reduced optimizers. A sufficiently short segment retains strict margin at $j$, hence has zero omitted hinge loss and would give another full optimizer, a contradiction.

Only a [support vector](../../../../../../support-vector.md) can therefore cause a held-out error. Each contributes at most one, proving the [support-vector leave-one-out error bound](../../../../../../support-vector-leave-one-out-error-bound.md)

$$
\boxed{\operatorname{err}_{CV}\leq\frac{s}{n}.}
$$

Keeping $C$ fixed is necessary for this deletion argument: holding an average-loss penalty parameter fixed while changing the sample size changes the optimization problem's effective $C$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
