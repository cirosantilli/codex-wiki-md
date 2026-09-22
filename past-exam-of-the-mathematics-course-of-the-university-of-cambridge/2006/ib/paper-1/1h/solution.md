<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

The [minimal polynomial](../../../../../minimal-polynomial.md) $m_A$ is the [monic polynomial](../../../../../monic-polynomial.md) of smallest degree satisfying $m_A(A)=0$. An annihilating [polynomial](../../../../../polynomial-split.md) exists, for example because $I,A,\ldots,A^{n^2}$ are linearly dependent in the $n^2$-dimensional space of [matrices](../../../../../matrix.md). A nonzero constant cannot annihilate $A$, so the minimal degree is positive.

If $p$ and $q$ are two such [monic polynomials](../../../../../monic-polynomial.md) of minimal degree $d$, then $(p-q)(A)=0$ and $\deg(p-q)<d$ unless $p=q$. Minimality therefore forces $p=q$. [Polynomial](../../../../../polynomial-split.md) division also shows that $m_A$ divides every annihilating [polynomial](../../../../../polynomial-split.md): the remainder after division would otherwise be an annihilator of smaller degree. This proves uniqueness rather than merely choosing one of several minimal-degree [polynomials](../../../../../polynomial-split.md).

If $A$ is real, coefficientwise [complex conjugation](../../../../../complex-conjugation.md) of $m_A(A)=0$ gives $\overline{m_A}(A)=0$. The conjugated [polynomial](../../../../../polynomial-split.md) is monic of the same degree, hence uniqueness gives $\overline{m_A}=m_A$. **The [minimal polynomial](../../../../../minimal-polynomial.md) of a real [matrix](../../../../../matrix.md) has real coefficients.**

For $n\ge3$, use the [block diagonal matrix](../../../../../block-diagonal-matrix.md)

$$
\boxed{A=\begin{pmatrix}1&1\\0&1\end{pmatrix}\oplus(-1)\oplus I_{n-3}.}
$$

The two-dimensional [Jordan block](../../../../../jordan-block.md) is annihilated by $(t-1)^2$ but not by $t-1$, while the scalar block requires the factor $t+1$. A [polynomial](../../../../../polynomial-split.md) annihilates the [direct sum](../../../../../direct-sum.md) exactly when it annihilates every block. Thus its [minimal polynomial](../../../../../minimal-polynomial.md) is the [least common multiple](../../../../../least-common-multiple.md) $(t-1)^2(t+1)$. For $n=3$ the final identity block is omitted.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
