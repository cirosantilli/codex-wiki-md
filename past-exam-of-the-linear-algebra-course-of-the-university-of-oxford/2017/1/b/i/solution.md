<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The displayed [matrix](../../../../../matrix.md) is the transpose convention for a [companion matrix](../../../../../companion-matrix.md). Expanding $\det(xI-A)$ along its last row gives

$$
\det(xI-A)=x^n+\alpha_{n-1}x^{n-1}+\cdots+\alpha_1x+\alpha_0=f(x).
$$

Indeed, the last entry contributes $(x+\alpha_{n-1})x^{n-1}$ and the entry in column $j<n$ contributes $\alpha_{j-1}x^{j-1}$; the cofactor signs cancel those from the superdiagonal entries $-1$. Consequently

$$
\boxed{\chi_T(x)=(-1)^nf(x).}
$$

The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem-split.md) gives $f(A)=0$, so $m_T$ divides $f$. To exclude a smaller [minimal polynomial](../../../../../minimal-polynomial.md), let $e_1,\ldots,e_n$ be the [standard basis](../../../../../standard-basis.md). The first $n-1$ rows of $A$ show

$$
e_1^{\mathsf T}A^j=e_{j+1}^{\mathsf T}\qquad(0\leq j<n).
$$

If $\sum_{j=0}^{n-1}c_jA^j=0$, multiplying on the left by $e_1^{\mathsf T}$ gives $\sum_jc_je_{j+1}^{\mathsf T}=0$, so every coefficient is zero. No nonzero [polynomial](../../../../../polynomial-split.md) of degree below $n$ vanishes at $A$. Since $f$ and $m_T$ are [monic polynomials](../../../../../monic-polynomial.md),

$$
\boxed{m_T=f.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
