<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [orthonormal](../../../../../orthonormal-set.md) columns give $A^TA=I_n$. Thus $P=AA^T$ is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the [column space](../../../../../column-space.md) of $A$, and

$$
Ax-b=A(x-A^Tb)-(I_m-P)b.
$$

The two terms are [orthogonal](../../../../../orthogonal-vectors.md), so the [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|Ax-b\|_2^2=\|x-A^Tb\|_2^2+\|(I_m-AA^T)b\|_2^2.
$$

Only the first term depends on $x$. Consequently the [linear least-squares problem](../../../../../linear-least-squares-problem.md) has the unique answer

$$
\boxed{x_*=A^Tb},\qquad \min_x\|Ax-b\|_2=\|(I_m-AA^T)b\|_2.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
