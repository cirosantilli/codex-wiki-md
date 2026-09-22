<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Reducing the augmented matrix gives

$$
\operatorname{rref}(A\mid b)=\begin{pmatrix}1&0&1&0\\0&1&2&1/2\\0&0&0&0\end{pmatrix}.
$$

There is no contradictory row. Hence the system is **consistent**, with [affine solution space](../../../../../affine-solution-space.md)

$$
\boxed{(x,y,z)=(0,1/2,0)+t(-1,-2,1),\qquad t\in\mathbb R.}
$$

The three [planes](../../../../../plane.md) intersect in this common line. Their normals span a two-dimensional [row space](../../../../../row-space.md), leaving a one-dimensional common direction, the [null space](../../../../../kernel-of-a-linear-map-split.md). More explicitly, five times the first equation minus eleven times the second plus twice the third is the zero equation, including the right-hand side; the third plane therefore contains the intersection of the first two.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
