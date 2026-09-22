<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose $y$ in the [capped simplex](../../../../../../capped-simplex.md) has a coordinate strictly between zero and one. Since $\sum_i y_i=k$ is an integer, it cannot have exactly one such coordinate: the other coordinates would contribute an integer sum. Hence there are distinct $i,j$ with $0<y_i,y_j<1$.

Choose $0<\varepsilon<\min\{y_i,1-y_i,y_j,1-y_j\}$ and set $y^{\pm}=y\pm\varepsilon(e_i-e_j)$, where $e_i,e_j$ are [standard basis](../../../../../../standard-basis.md) vectors. Both perturbed [vectors](../../../../../../vector.md) satisfy the coordinate bounds and have the same coordinate sum. They are distinct and $y=(y^++y^-)/2$, so $y$ is not an [extreme point](../../../../../../extreme-point.md).

Conversely, every zero-one [vector](../../../../../../vector.md) in this [convex polytope](../../../../../../convex-polytope.md) is an [extreme point](../../../../../../extreme-point.md). If it were a nontrivial [convex combination](../../../../../../convex-combination.md) of two feasible [vectors](../../../../../../vector.md), each coordinate equal to zero would force both corresponding coordinates to be zero, and each coordinate equal to one would force both to be one. Thus the two [vectors](../../../../../../vector.md) would equal the original one. The [extreme points](../../../../../../extreme-point.md) are therefore exactly the indicators of $k$-element subsets.

## ↑ Ancestors (11)

1. [A](../a.md)
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
