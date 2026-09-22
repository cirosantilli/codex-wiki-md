<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Regard the real [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md) as acting on $\mathbb C^n$. Its [Hermitian adjoint](../../../../../adjoint-operator.md) is $A^*=A^T=-A$. Parts (i) and (iii) show that its [eigenvalues](../../../../../eigenvalue.md) are purely imaginary and its complex [minimal polynomial](../../../../../minimal-polynomial.md) has no repeated roots.

Since $A$ has real entries, nonreal [eigenvalues](../../../../../eigenvalue.md) occur in conjugate pairs. A nonzero pair has the form $i\alpha,-i\alpha$, with $\alpha>0$, and contributes the real [quadratic polynomial](../../../../../quadratic-polynomial.md)

$$
(x-i\alpha)(x+i\alpha)=x^2+\alpha^2.
$$

Zero, if present, contributes one factor $x$. Hence the real [minimal polynomial](../../../../../minimal-polynomial.md) is

$$
\boxed{m_A(x)=x^{\varepsilon}\prod_{j=1}^r(x^2+\alpha_j^2),\qquad
\varepsilon\in\{0,1\},\quad\alpha_j>0\text{ distinct}.}
$$

The product annihilates $A$ after [complexification of a real vector space](../../../../../complexification-of-a-real-vector-space.md), so it also annihilates the original real [linear map](../../../../../linear-map.md); no factor can be removed because each displayed complex root is an [eigenvalue](../../../../../eigenvalue.md). This proves both the asserted form and its minimality. The case $A=0$ has $\varepsilon=1$ and an empty product.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
