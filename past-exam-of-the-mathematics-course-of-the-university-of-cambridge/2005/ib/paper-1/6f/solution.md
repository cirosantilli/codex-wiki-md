<h1 id="6f/solution">Solution</h1>

↑ **Parent:** [6F](../6f.md)

For the [Cholesky decomposition](../../../../../cholesky-decomposition.md) $A=LL^T$, choose $L$ lower triangular with positive diagonal whenever $A$ is [positive-definite](../../../../../positive-definite-bilinear-form.md). Successive entries are

$$
l_{11}=\sqrt2,\quad l_{21}=-2\sqrt2,\quad l_{31}=\sqrt2,\quad
l_{22}=\sqrt{\lambda+2}.
$$

The $(3,2)$ equation gives $l_{31}l_{21}+l_{32}l_{22}=2+3\lambda$, so $l_{32}=3\sqrt{\lambda+2}$. Finally,

$$
l_{33}^2=23+9\lambda-l_{31}^2-l_{32}^2=3.
$$

Thus for $\lambda>-2$,

$$
\boxed{L=\begin{pmatrix}
\sqrt2&0&0\\
-2\sqrt2&\sqrt{\lambda+2}&0\\
\sqrt2&3\sqrt{\lambda+2}&\sqrt3
\end{pmatrix}}.
$$

It is nonsingular, and for every nonzero vector $v$, $v^TAv=|L^Tv|^2>0$.

Necessity also follows from the leading principal determinants $2$, $2(\lambda+2)$ and $6(\lambda+2)$, or directly from the second elimination pivot. Hence

$$
\boxed{A\text{ is positive definite exactly when }\lambda>-2}.
$$

At $\lambda=-2$ the displayed limiting factor still satisfies $A=LL^T$, but has rank two and zero second diagonal entry: $A$ is [positive semidefinite](../../../../../positive-semidefinite-matrix.md), not [positive-definite](../../../../../positive-definite-bilinear-form.md). For $\lambda<-2$, taking $v=(2,1,0)^T$ gives $v^TAv=\lambda+2<0$, so no real factor $LL^T$ exists.

## ↑ Ancestors (10)

1. [6F](../6f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
