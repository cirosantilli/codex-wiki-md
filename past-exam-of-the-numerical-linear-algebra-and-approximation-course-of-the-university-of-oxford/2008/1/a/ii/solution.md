<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Householder matrix](../../../../../householder-transformation.md) has the form

$$
\boxed{H=I-2\frac{vv^T}{v^Tv},\qquad v\ne0.}
$$

It reflects in the hyperplane perpendicular to $v$. Put $P=vv^T/(v^Tv)$, an [orthogonal projector](../../../../../orthogonal-projection.md) satisfying $P^T=P$ and $P^2=P$. Then $H^TH=(I-2P)^2=I-4P+4P^2=I$, proving that every [Householder matrix](../../../../../householder-transformation.md) is orthogonal.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and approximation course of the University of Oxford](../../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
