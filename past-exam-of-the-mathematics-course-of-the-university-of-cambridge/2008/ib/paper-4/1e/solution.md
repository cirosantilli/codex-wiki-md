<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

A [Jordan normal form](../../../../../jordan-normal-form.md) of a complex $n\times n$ [matrix](../../../../../matrix.md) $A$ is a [similarity transformation](../../../../../similarity-transformation.md) $P^{-1}AP=J$ in which $J$ is a direct sum of [Jordan blocks](../../../../../jordan-block.md)

$$
J_r(\lambda)=\begin{pmatrix}\lambda&1&&0\\&\lambda&\ddots&\\&&\ddots&1\\0&&&\lambda\end{pmatrix}.
$$

For each [eigenvalue](../../../../../eigenvalue.md), the multiset of block sizes is uniquely determined by $A$; only the order of the blocks is arbitrary. The change-of-basis [matrix](../../../../../matrix.md) $P$ is generally not unique.

For the given [matrix](../../../../../matrix.md), expansion of the [characteristic polynomial](../../../../../characteristic-polynomial.md) gives

$$
\det(tI-A)=(t-1)^2(t-2),\qquad A-I=\begin{pmatrix}-8&3&-5\\7&-2&5\\17&-6&11\end{pmatrix}.
$$

The upper-left $2\times2$ minor of $A-I$ is $-5$, so its [rank](../../../../../rank-one-quadratic-form.md) is $2$ and the [eigenspace](../../../../../eigenspace.md) for $1$ has dimension $1$. Thus the two occurrences of the [eigenvalue](../../../../../eigenvalue.md) $1$ belong to a single size-$2$ [Jordan block](../../../../../jordan-block.md). More explicitly, the [Jordan chain](../../../../../jordan-chain.md) and the remaining [eigenvector](../../../../../eigenvector.md) can be chosen as

$$
v_1=(1,1,-1)^T,\quad v_2=(1,3,0)^T,\quad v_3=(0,5,3)^T,\qquad (A-I)v_1=0,\quad(A-I)v_2=v_1,\quad Av_3=2v_3.
$$

Consequently, with $P=(v_1\ v_2\ v_3)$, for which $\det P=1$, the answer is

$$
\boxed{P^{-1}AP=\begin{pmatrix}1&1&0\\0&1&0\\0&0&2\end{pmatrix}.}
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
