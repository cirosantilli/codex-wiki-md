<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The objective is [strictly convex](../../../../../../strictly-convex-function.md), so the minimizer is unique. The [Slater condition](../../../../../../slater-s-condition.md) makes the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) necessary and sufficient. Absorb the box constraints into the [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) and attach a scalar multiplier $\nu$ to $a^Tx=b$. Stationarity over the box is equivalent to

$$
x^*=P_{[0,1]^n}(y-\nu a),
$$

while primal feasibility requires $a^Tx^*=b$. Coordinatewise, these conditions are

$$
\boxed{x_i^*=\min\{1,\max\{0,y_i-\nu a_i\}\}},
\qquad
\boxed{\sum_{i=1}^na_i
\min\{1,\max\{0,y_i-\nu a_i\}\}=b}.
$$

They are also sufficient because they minimize the [Lagrangian](../../../../../../lagrangian.md) over the box and satisfy the equality constraint. Thus the [projection onto a box-constrained hyperplane](../../../../../../projection-onto-a-box-constrained-hyperplane.md) reduces to solving the displayed one-dimensional continuous, nonincreasing equation for $\nu$. The multiplier need not be unique on a flat interval, but the projected vector is unique.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
