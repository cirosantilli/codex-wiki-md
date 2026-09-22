<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
\Omega=\begin{pmatrix}0&I_n\\-I_n&0\end{pmatrix}.
$$

The identity belongs to $G$. If $A,B\in G$, then

$$
(AB)^T\Omega(AB)=B^T(A^T\Omega A)B=B^T\Omega B=\Omega.
$$

Taking determinants in $A^T\Omega A=\Omega$ shows that $A$ is invertible, and multiplying that identity by $A^{-T}$ and $A^{-1}$ gives $(A^{-1})^T\Omega A^{-1}=\Omega$. Thus $G$ is a group.

Let $\operatorname{Skew}_{2n}(\mathbb R)$ denote the vector space of skew-symmetric $2n\times2n$ matrices and define

$$
F:M_{2n}(\mathbb R)\longrightarrow\operatorname{Skew}_{2n}(\mathbb R),
\qquad F(A)=A^T\Omega A.
$$

Then $G=F^{-1}(\Omega)$. At $A\in G$,

$$
DF_A(H)=H^T\Omega A+A^T\Omega H.
$$

Given any skew-symmetric matrix $S$, set $H=AB$ with $B=-\frac12\Omega S$. Since $A^T\Omega A=\Omega$, a direct calculation gives

$$
DF_A(AB)=B^T\Omega+\Omega B=S.
$$

The derivative is therefore surjective at every point of $F^{-1}(\Omega)$. The [regular level set theorem](../../../../../../regular-level-set-theorem.md) proves that the [symplectic group](../../../../../../symplectic-group.md) is an embedded submanifold of $M_{2n}(\mathbb R)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
