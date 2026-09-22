<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Using $\chi_M(t)=\det(tI-M)$, expansion or triangular reordering gives

$$
\boxed{\chi_M(t)=(t-1)^2(t-2)^2.}
$$

The [eigenspace](../../../../../eigenspace.md) for $1$ is spanned by $e_1$, so its algebraic multiplicity two requires a size-two [Jordan block](../../../../../jordan-block.md). A convenient [Jordan chain](../../../../../jordan-chain.md) is

$$
v_1=e_1,\qquad v_2=e_2+e_3,\qquad (M-I)v_2=v_1.
$$

For [eigenvalue](../../../../../eigenvalue.md) $2$, the [eigenspace](../../../../../eigenspace.md) has [basis](../../../../../basis.md) $w_1=e_1+e_3$, $w_2=e_4$, hence both corresponding blocks have size one. Therefore a [Jordan normal form](../../../../../jordan-normal-form.md) and the [minimal polynomial](../../../../../minimal-polynomial.md) are

$$
\boxed{J=\begin{pmatrix}1&1&0&0\\0&1&0&0\\0&0&2&0\\0&0&0&2\end{pmatrix},
\qquad m_M(t)=(t-1)^2(t-2).}
$$

The ordered [basis](../../../../../basis.md) $(v_1,v_2,w_1,w_2)$ supplies the [change-of-basis matrix](../../../../../change-of-basis-matrix.md)

$$
\boxed{P=\begin{pmatrix}1&0&1&0\\0&1&0&0\\0&1&1&0\\0&0&0&1\end{pmatrix}.}
$$

Its [determinant](../../../../../determinant.md) is one, and the chain equations give $MP=PJ$, proving $P^{-1}MP=J$. The square at $t=1$ in the [minimal polynomial](../../../../../minimal-polynomial.md) is essential: $M$ is not [diagonalizable](../../../../../diagonalizable-matrix.md).

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
