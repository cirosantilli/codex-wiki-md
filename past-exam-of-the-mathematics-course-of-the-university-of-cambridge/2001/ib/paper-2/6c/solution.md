<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Right multiplication is linear because $(sX+tY)A=sXA+tYA$. In the supplied row-entry [basis](../../../../../basis.md), write $X=\begin{pmatrix}x_1&x_2\\x_3&x_4\end{pmatrix}$. Multiplying on the right gives coordinates $(ax_1+cx_2,bx_1+dx_2,ax_3+cx_4,bx_3+dx_4)^T$. Therefore

$$
\boxed{[\rho_A]=\begin{pmatrix}a&c&0&0\\b&d&0&0\\0&0&a&c\\0&0&b&d\end{pmatrix}=\operatorname{diag}(A^T,A^T).}
$$

The transpose is ordinary, with no complex conjugation. Block determinants and invariance of determinant under transpose prove

$$
\boxed{\chi_{\rho_A}(t)=\det(tI_2-A^T)^2=\chi_A(t)^2.}
$$

For every polynomial $p$, powers of right multiplication give $p(\rho_A)(X)=Xp(A)$. If $p(A)=0$ then $p(\rho_A)=0$; if $p(\rho_A)=0$, take $X=I$ to infer $p(A)=0$. They have identical annihilating polynomials, so their unique monic least-degree annihilator, the [minimal polynomial](../../../../../minimal-polynomial.md), is the same. Thus **$m_{\rho_A}=m_A$**, as in the [characteristic and minimal polynomials of right multiplication](../../../../../characteristic-and-minimal-polynomials-of-right-multiplication.md) result.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
