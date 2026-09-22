<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $W=\operatorname{span}\{\mathbf v,\mathbf w\}=\operatorname{col}V$. Since the two columns are [linearly independent](../../../../../../linear-independence.md), the leading $2\times2$ block $R_1$ in

$$
R=SV=\begin{pmatrix}R_1\\0\end{pmatrix}
$$

is invertible. Hence $S(W)=\operatorname{span}\{\mathbf e^{(1)},\mathbf e^{(2)}\}$. The hypothesis that $W$ is an [invariant subspace](../../../../../../invariant-subspace.md) of $A$ implies that this coordinate plane is invariant under $\widehat A=SAS^{-1}$. Consequently the first two columns of $\widehat A$ have no entries below row two, and

$$
\widehat A=
\begin{pmatrix}
B&C\\
0&D
\end{pmatrix},
$$

where $B$ is the top-left $2\times2$ block and $D$ is the bottom-right $(n-2)\times(n-2)$ block. [Eigenvalue deflation by an invariant subspace](../../../../../../eigenvalue-deflation-by-an-invariant-subspace.md) now gives

$$
\det(zI-A)=\det(zI-\widehat A)
=\det(zI_2-B)\det(zI_{n-2}-D),
$$

so

$$
\boxed{\operatorname{spec}(A)=\operatorname{spec}(B)\mathbin\cup\operatorname{spec}(D),}
$$

again counting [algebraic multiplicities](../../../../../../algebraic-multiplicity.md).

For the required orthogonal reduction, take a thin [QR decomposition](../../../../../../qr-decomposition.md) $V=Q_1R_1$, extend the two orthonormal columns of $Q_1$ to an orthogonal matrix $Q$, and set $S=Q^T$. Then

$$
SV=Q^TV=\begin{pmatrix}R_1\\0\end{pmatrix}.
$$

Equivalently, apply one [Householder transformation](../../../../../../householder-transformation.md) to annihilate entries $2,\ldots,n$ of $\mathbf v$, followed by a second Householder transformation acting only on coordinates $2,\ldots,n$ to annihilate entries $3,\ldots,n$ of the transformed $\mathbf w$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
