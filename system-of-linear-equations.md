# System of linear equations

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/System_of_linear_equations)

A [system of linear equations](system-of-linear-equations.md) imposes several [linear equations](linear-equation.md) on the same unknowns. In the compact form $Ax=b$, the [matrix](matrix.md) $A$ contains their [coefficients](coefficient.md), the [vector](vector.md) $x$ contains the unknowns, and the [vector](vector.md) $b$ contains the required outputs. Over the [real numbers](real-number.md), the following examples exhibit the three possible outcomes: one solution, infinitely many solutions, or no solution.

For $x+y=3$ and $x-y=1$, adding the two [linear equations](linear-equation.md) gives $2x=4$, hence $x=2$ and $y=1$. Each [linear equation](linear-equation.md) describes a [line](straight-line.md) in the [plane](plane.md); the two [lines](straight-line.md) meet only at $(2,1)$. Substitution checks both requirements: $2+1=3$ and $2-1=1$. The two measurements together determine both unknowns.

Keeping only $x+y=3$ leaves a whole [line](straight-line.md) of solutions:

$$
(x,y)=(3-t,t)=(3,0)+t(-1,1),\qquad t\in\mathbb R.
$$

For instance, $t=0,1,3$ gives $(3,0),(2,1),(0,3)$. The direction $(-1,1)$ belongs to the [kernel](kernel-of-a-linear-map.md) of the [linear map](linear-map.md) $(x,y)\mapsto x+y$: its two contributions cancel. Moving in that direction changes the unknowns without changing their measured sum. The solution [line](straight-line.md) is an [affine space](affine-space.md), translated away from the origin.

For $x+y=3$ and $2x+2y=7$, the second [linear equation](linear-equation.md) instead demands $x+y=3.5$. The parallel [lines](straight-line.md) never meet. In the [augmented matrix](augmented-matrix.md), subtracting twice the first row from the second is an [elementary row operation](elementary-row-operation.md) that exposes the contradiction:

$$
\left[\begin{array}{cc|c}1&1&3\\2&2&7\end{array}\right]
\longrightarrow
\left[\begin{array}{cc|c}1&1&3\\0&0&1\end{array}\right].
$$

The last row says $0=1$. A zero row of [coefficients](coefficient.md) is harmless only when its appended entry is also zero.

<a id="image-three-linear-systems-a-unique-intersection-a-solution-line-and-incompatible-parallel-lines"></a>
![](linear-system-solution-sets.png)

**[Figure 40](#image-three-linear-systems-a-unique-intersection-a-solution-line-and-incompatible-parallel-lines). Three linear systems: a unique intersection, a solution line, and incompatible parallel lines**.

The column viewpoint unifies these pictures. If $a_j$ are the columns of $A$, then $Ax=\sum_j x_j a_j$: a [linear combination](linear-combination.md) of those columns. A [linear system](system-of-linear-equations.md) is consistent precisely when $b$ lies in the [column space](column-space.md), the [image of a linear map](image-of-a-linear-map.md) represented by $A$. Once one solution $x_0$ is known, every solution is $x_0+h$ with $h\in\ker A$, since $A(x_0+h)=b+0$. Conversely, subtracting any two solutions gives an element of the [kernel](kernel-of-a-linear-map.md). Thus the [kernel](kernel-of-a-linear-map.md) measures freedom, while the [image of a linear map](image-of-a-linear-map.md) decides existence. A consistent [linear system](system-of-linear-equations.md) has a unique solution exactly when its [kernel](kernel-of-a-linear-map.md) is $\{0\}$.[Strang, Lecture 1: The geometry of linear equations](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-1-the-geometry-of-linear-equations/)

Counting [linear equations](linear-equation.md) alone does not tell us how much information is present. If the second requirement were $2x+2y=6$, it would repeat $x+y=3$, so the two [linear equations](linear-equation.md) would still leave the same solution [line](straight-line.md). The [matrix rank](matrix-rank.md) counts independent requirements. For a consistent [linear system](system-of-linear-equations.md) with $n$ unknowns and [matrix rank](matrix-rank.md) $r$, the [rank-nullity theorem](rank-nullity-theorem.md) gives $n-r$ as the [dimension](dimension-vector-space.md) of the [kernel](kernel-of-a-linear-map.md). This is the number of independent directions in which a solution can move. In the single-measurement example, one measured combination leaves one direction of freedom; in the sum-and-difference example, neither unknown can change without changing an output.

**Table of contents**

- [Image criterion for a matrix factorization](image-criterion-for-a-matrix-factorization.md)
- [Augmented matrix](augmented-matrix.md)
- [Homogeneous linear system](homogeneous-linear-system.md)
- [Linear equation](linear-equation.md)
  - [Affine solution space of a linear equation](affine-solution-space-of-a-linear-equation.md)
- [Fredholm alternative for a matrix](fredholm-alternative-for-a-matrix.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Brouwer fixed-point theorem](brouwer-fixed-point-theorem.md)
- [Linear algebra](linear-algebra-split.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/6a/solution.md)
- [Spreadsheet circular reference](spreadsheet-circular-reference.md)
- [System of linear equations](system-of-linear-equations.md)
