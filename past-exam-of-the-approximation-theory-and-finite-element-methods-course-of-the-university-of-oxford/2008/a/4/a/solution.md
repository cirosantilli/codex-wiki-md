<h1 id="a/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [equioscillation theorem](../../../../../equioscillation-theorem.md) says that a best degree-at-most-$n$ [polynomial](../../../../../polynomial-split.md) approximation to a continuous real [function](../../../../../function-split.md) on $[a,b]$ has $n+2$ ordered extreme-error points with alternating signs and equal absolute error. Conversely such alternation proves optimality. If the error is zero, the target is already a [polynomial](../../../../../polynomial-split.md) of the required degree.

For the [single-point exchange in polynomial minimax approximation](../../../../../single-point-exchange-in-polynomial-minimax-approximation.md), start with $n+2$ ordered reference points $t_j$ and solve the linear system

$$
u(t_j)-p(t_j)=(-1)^jE,\qquad j=0,\ldots,n+1
$$

for the $n+1$ [polynomial](../../../../../polynomial-split.md) coefficients and $E$. Locate a point of largest absolute error on the interval. If its magnitude is no larger than $|E|$ within the desired tolerance, alternation certifies the approximation.

Otherwise insert that point and delete one old reference point so that the ordered signs still alternate. If the new point lies between two reference points, delete the neighboring point with the same error sign. If it lies outside the reference range, either replace the adjacent same-sign endpoint or, for opposite sign, insert it and drop the far endpoint. Solve again and repeat. This is the one-point [Remez algorithm](../../../../../remez-algorithm.md); a global extreme-error search is required for its stopping certificate, rather than merely checking the old reference points.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
