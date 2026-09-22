<h1 id="41d/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $E_2=(e_1,e_2)$ and

$$
S_k=\operatorname{range}(H^{k+1}E_2).
$$

Because $Q_kR_k$ is the QR factorization of $H^{k+1}$, $S_k$ is the span of the first two columns $q_1^{(k)},q_2^{(k)}$ of $Q_k$.

The first row of the tridiagonal [eigenvalue](../../../../../../../eigenvalue.md) equation is

$$
h_{11}b_j+h_{12}c_j=\lambda_jb_j.
$$

In the generic case $\lambda_{n-1}\ne\lambda_n$, the two dominant coefficient [vectors](../../../../../../../vector.md) are independent, since

$$
\det\begin{pmatrix}b_{n-1}&c_{n-1}\\b_n&c_n\end{pmatrix}
=\frac{b_{n-1}b_n}{h_{12}}(\lambda_n-\lambda_{n-1})\ne0.
$$

Here $h_{12}\ne0$, since otherwise the displayed [eigenvalue](../../../../../../../eigenvalue.md) equation and the nonzero $b_j$ would force all [eigenvalues](../../../../../../../eigenvalue.md) to equal $h_{11}$. The strict [spectral gap](../../../../../../../spectral-gap.md) below the dominant pair now implies

$$
S_k\longrightarrow W=\operatorname{span}\{w_{n-1},w_n\}.
$$

This is two-dimensional [subspace iteration](../../../../../../../subspace-iteration.md). If the [dominant eigenvalue](../../../../../../../dominant-eigenvalue.md) is repeated, $H$ acts as a [scalar](../../../../../../../scalar.md) on $W$; the same QR argument either captures all of $W$ or separates its missing direction from the strictly smaller eigenspaces, and the conclusion below is unchanged.

Since $q_2^{(k)}\in S_k$ and $q_3^{(k)}\perp S_k$,

$$
\operatorname{dist}(q_2^{(k)},W)\to0,
\qquad
\lVert P_Wq_3^{(k)}\rVert\to0.
$$

The space $W$ is invariant under $H$, so

$$
 h_{3,2}^{(k+1)}
 =(q_3^{(k)})^THq_2^{(k)}\longrightarrow0.
$$

Shifting the index does not affect the [limit](../../../../../../../limit-of-a-function.md), and therefore

$$
\boxed{h_{3,2}^{(k)}\to0.}
$$

**Thus the unshifted QR algorithm asymptotically deflates a $2\times2$ block associated with the equal-modulus dominant pair.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [41D](../../../41d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
