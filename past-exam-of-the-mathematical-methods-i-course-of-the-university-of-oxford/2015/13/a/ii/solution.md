<h1 id="13/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Repeated substitution in the [affine iteration](../../../../../affine-iteration.md) gives

$$
x_k=M^{k-1}x_1+(I+M+\cdots+M^{k-2})c.
$$

Therefore the required [matrix polynomials](../../../../../matrix-polynomial.md) are

$$
\boxed{f(M)=M^{k-1},\qquad g(M)=\sum_{j=0}^{k-2}M^j.}
$$

These formulas do not require an inverse. If $I-M$ is an [invertible matrix](../../../../../invertible-matrix.md), multiplying the finite geometric sum by $I-M$ gives $g(M)=(I-M^{k-1})(I-M)^{-1}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [13](../../../13.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
