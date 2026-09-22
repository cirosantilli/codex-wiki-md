<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [outer product](../../../../../outer-product.md) has entries $\boxed{(xy^T)_{ij}=x_iy_j}$. Every column is a multiple of $x$, and at least one column is nonzero because $y\ne0$. Its column space is therefore exactly $\operatorname{span}\{x\}$, giving $\boxed{\operatorname{rank}(xy^T)=1}$.

A [Householder matrix](../../../../../householder-transformation.md) is $H=I-2vv^T/(v^Tv)$, $v\ne0$. With $P=vv^T/(v^Tv)$ one has $P^T=P$ and $P^2=P$, so $H^TH=(I-2P)^2=I$. Thus it is an [orthogonal matrix](../../../../../orthogonal-matrix.md) and is its own inverse.

To express an arbitrary orthogonal $Q$ as a product of these reflections, argue by induction on its dimension. Its first column $q$ is a unit vector. If $q\ne e_1$, take $v=q-e_1$. Then $v^Tq=1-q_1$ and $v^Tv=2(1-q_1)$, so the corresponding reflection satisfies $Hq=q-v=e_1$. If $q=e_1$, no reflection is required. The resulting orthogonal matrix has first column $e_1$; orthogonality of its columns then makes its first row $e_1^T$ as well. It is consequently $\operatorname{diag}(1,Q')$ with $Q'$ orthogonal. Apply the induction hypothesis to $Q'$ and embed its reflections in the full space. In dimension one the only possibilities are $1$, the empty product, and $-1$, itself a reflection. Reversing the performed transformations proves the [Householder factorization of an orthogonal matrix](../../../../../householder-factorization-of-an-orthogonal-matrix.md), with at most the dimension many reflections.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
