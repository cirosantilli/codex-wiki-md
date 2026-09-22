<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The required [linear program](../../../../../../linear-programming.md) is

$$
\boxed{f_k(x)=\max_{y\in\mathbb R^n}\left\{x^Ty:y_i\geq0,\ y_i\leq1\ (1\leq i\leq n),\ \sum_i y_i=k\right\}.}
$$

There are $2n$ inequality constraints and one equality constraint, all independent of $x$.

The feasible set is the [capped simplex](../../../../../../capped-simplex.md), a nonempty [compact set](../../../../../../compact-space.md). A [linear function](../../../../../../linear-function.md) attains its maximum at an [extreme point](../../../../../../extreme-point.md); the previous part identifies these as the indicators of $k$-element subsets. At such a [vector](../../../../../../vector.md), the objective is the sum of the selected coordinates. Maximizing selects the $k$ largest coordinates, including when some are negative or tied. Equivalently, $f_k$ is the [support function](../../../../../../support-function.md) called the [sum of the largest components](../../../../../../sum-of-the-largest-components.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
