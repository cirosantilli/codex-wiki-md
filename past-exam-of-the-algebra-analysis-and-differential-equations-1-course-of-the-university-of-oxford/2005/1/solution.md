<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $m_T$ be the [minimal polynomial](../../../minimal-polynomial.md). If $Tv=\lambda v$ with $v\ne0$, then $0=m_T(T)v=m_T(\lambda)v$, so $m_T(\lambda)=0$. Conversely, if $m_T(\lambda)=0$, write $m_T(X)=(X-\lambda)q(X)$. If $T-\lambda I$ were invertible, the identity $(T-\lambda I)q(T)=0$ would imply $q(T)=0$, contradicting minimality of the degree. Thus $T-\lambda I$ has a nonzero [kernel of a linear map](../../../kernel-of-a-linear-map-split.md), and $\lambda$ is an [eigenvalue](../../../eigenvalue.md). This proves the [eigenvalue criterion using the minimal polynomial](../../../eigenvalue-criterion-using-the-minimal-polynomial.md) for roots in the field under consideration.

For the given matrix, direct expansion gives

$$
\boxed{\chi_T(X)=\det(XI-A)=X^3+3X^2+3X+1=(X+1)^3.}
$$

Put $N=A+I$. Direct multiplication gives

$$
N^2=\begin{pmatrix}1&2&1\\-1&-2&-1\\1&2&1\end{pmatrix}\ne0,\qquad N^3=0.
$$

By the [Cayley-Hamilton theorem](../../../cayley-hamilton-theorem-split.md), $m_T$ divides $(X+1)^3$; the nonzero square rules out every smaller power. Therefore $\boxed{m_T(X)=(X+1)^3}$. Its sole [eigenvalue](../../../eigenvalue.md) is $-1$, but the size of the nilpotent part makes the minimum polynomial cubic rather than linear.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2005](../../2005-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
