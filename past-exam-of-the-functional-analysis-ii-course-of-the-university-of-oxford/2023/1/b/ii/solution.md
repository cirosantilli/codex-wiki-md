<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [orthogonal complement](../../../../../orthogonal-complement.md) $x^\perp$ is infinite-dimensional: otherwise $X=\operatorname{span}\{x\}\oplus x^\perp$ would be finite-dimensional. Inductively choose an [orthonormal sequence](../../../../../orthonormal-sequence.md) $(e_n)$ in $x^\perp$, each new vector being orthogonal to the preceding finite [linear span](../../../../../linear-span.md). The [Bessel inequality](../../../../../bessel-s-inequality.md) gives $\sum_n|\langle e_n,z\rangle|^2\leq\|z\|^2$ for every $z\in X$, so $\langle e_n,z\rangle\to0$. Thus $(e_n)$ is a [weakly null orthonormal sequence](../../../../../weakly-null-orthonormal-sequence.md).

Set

$$
\boxed{x_n=x+\sqrt{1-\|x\|^2}\,e_n.}
$$

By [orthogonality](../../../../../orthogonal-vectors.md), $\|x_n\|^2=\|x\|^2+(1-\|x\|^2)=1$, while $\langle x_n-x,z\rangle\to0$ for every $z$. Hence $x_n\rightharpoonup x$. When $\|x\|=1$, this formula simply gives the constant sequence $x_n=x$. In particular, the [weak closure of the unit sphere](../../../../../weak-closure-of-the-unit-sphere.md) contains the whole [closed unit ball](../../../../../closed-unit-ball.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
