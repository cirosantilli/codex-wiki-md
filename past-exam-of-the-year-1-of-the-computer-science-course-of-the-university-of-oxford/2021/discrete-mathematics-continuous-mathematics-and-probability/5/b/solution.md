<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Complete the square to write the objective as

$$
x^2-2x+y^2-4y=\|(x,y)-(1,2)\|^2-5.
$$

Let $z=(x,y)$ and $a=(1,2)$, so $\|a\|=\sqrt5$ while feasibility requires $\|z\|\geq\sqrt{20}=2\sqrt5$. The [reverse triangle inequality](../../../../../reverse-triangle-inequality.md) gives

$$
\|z-a\|\geq\|z\|-\|a\|\geq\sqrt5.
$$

The objective is therefore at least zero. Equality is attained by $z=2a=(2,4)$, which lies on the boundary. Equality requires the [vectors](../../../../../vector.md) to have the same direction and $\|z\|=2\sqrt5$, so this minimizer is unique. Hence

$$
\boxed{(x_*,y_*)=(2,4),\qquad f_*=0.}
$$

It also satisfies the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) with $\lambda=1/2$. The direct distance argument proves global optimality even though the exterior of a disk is not a [convex set](../../../../../convex-set-split.md); this is [nearest-point minimization outside a Euclidean ball](../../../../../nearest-point-minimization-outside-a-euclidean-ball.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
