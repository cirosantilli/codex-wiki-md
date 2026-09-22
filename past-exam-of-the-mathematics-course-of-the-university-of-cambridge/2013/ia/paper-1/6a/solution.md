<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

For a [linear map](../../../../../linear-map.md) $\alpha:\mathbb R^m\to\mathbb R^n$, its [kernel](../../../../../kernel-of-a-linear-map.md) and [image of a linear map](../../../../../image-of-a-linear-map.md) are

$$
\ker\alpha=\{v:\alpha(v)=0\},\qquad\operatorname{im}\alpha=\{\alpha(v):v\in\mathbb R^m\}.
$$

The kernel is a subspace of the domain and the image a subspace of the codomain. Given the stated bases, define the [matrix of a linear map](../../../../../matrix-representation-of-a-linear-map.md) by

$$
\alpha(e_j)=\sum_{i=1}^n A_{ij}f_i.
$$

Its $j$th column is the coordinate vector of $\alpha(e_j)$; if $v=\sum_jv_je_j$, the output coordinates are $(\alpha v)_i=\sum_jA_{ij}v_j$.

For the [change of basis](../../../../../change-of-basis.md), write $e'_j=\sum_k P_{kj}e_k$ and $f'_i=\sum_\ell Q_{\ell i}f_\ell$. The matrices $P,Q$ are invertible. Input coordinates change by $v_{\rm old}=Pv_{\rm new}$ and output coordinates by $w_{\rm old}=Qw_{\rm new}$, so

$$
\boxed{A'=Q^{-1}AP,\qquad A'_{ij}=\sum_{\ell=1}^n\sum_{k=1}^m(Q^{-1})_{i\ell}A_{\ell k}P_{kj}.}
$$

The domain and codomain basis changes need not be the same matrix.

For $\beta$, the two input vectors form a basis of $\mathbb R^2$, so its image is the span of $v=(1,2,3)^T$ and $w=(6,4,2)^T$. The vector $n=(1,-2,1)^T$ is [orthogonal](../../../../../orthogonal-vectors.md) to both, since $n\cdot v=n\cdot w=0$. Every possible output therefore satisfies $n\cdot\beta x=0$, whereas the target itself is $n$ and $n\cdot n=6$. Hence **there is no $x$ with the required output**. This uses an [image obstruction by an annihilating functional](../../../../../image-obstruction-by-an-annihilating-functional.md), rather than an inconsistent guessed input.

For $\gamma$, use the input basis $v_1=(1,2,0)^T$, $v_2=(0,1,1)^T$, $v_3=(0,1,0)^T$. Its determinant is $-1$, so it is genuinely a basis. Write $x=sv_1+tv_2+wv_3$. Then

$$
\gamma x=(s-2t,\ 3s+t+w)^T=0
\quad\Longleftrightarrow\quad s=2t,\quad w=-7t.
$$

Substitution back into physical coordinates gives

$$
\boxed{\ker\gamma=\{t(2,-2,1)^T:t\in\mathbb R\}.}
$$

For a direct check, its standard matrix is $\begin{pmatrix}1&0&-2\\1&1&0\end{pmatrix}$, which annihilates exactly that line.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
