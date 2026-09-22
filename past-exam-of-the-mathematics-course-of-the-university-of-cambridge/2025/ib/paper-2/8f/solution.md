<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

A [Jordan block](../../../../../jordan-block.md) is $J_m(\alpha)=\alpha I+N$, where $N$ has ones on the superdiagonal and zeros elsewhere. Since $N^2=0$ for $m=2$, Taylor expansion gives

$$
p(J_2(\alpha))=p(\alpha)I+p'(\alpha)N
=\begin{pmatrix}p(\alpha)&p'(\alpha)\\0&p(\alpha)\end{pmatrix}.
$$

The [Jordan normal form](../../../../../jordan-normal-form.md) is the block-diagonal [matrix](../../../../../matrix.md), unique up to block order, to which $A$ is similar and whose blocks are Jordan blocks.

A block of size at least two for [eigenvalue](../../../../../eigenvalue.md) $\lambda$ contributes a [generalized eigenvector](../../../../../generalized-eigenvector.md) in $\ker(A-\lambda I)^2\setminus\ker(A-\lambda I)$. Thus the displayed equality for every $\lambda$ is equivalent to every block having size one, which is diagonalizability.

The transpose of each Jordan block is similar to it by reversing its [basis](../../../../../basis.md). Hence $A^T$ has the same Jordan form as $A$.

Write $A=PJP^{-1}$. Let $R$ be block diagonal with the reversal [matrix](../../../../../matrix.md) on each Jordan block. Both $R$ and $RJ$ are symmetric and $R$ is invertible. Therefore

$$
A=(PRP^T)\{P^{-T}(RJ)P^{-1}\}=CD,
$$

where $C,D$ are symmetric and $C$ is nonsingular.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
