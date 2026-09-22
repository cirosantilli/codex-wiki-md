<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [perfect Lie algebra](../../../../perfect-lie-algebra.md) $\mathfrak s$, every element is a sum of [Lie brackets](../../../../lie-bracket.md). The [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md) satisfies $\operatorname{ad}[x,y]=[\operatorname{ad}x,\operatorname{ad}y]$, and the [trace of a commutator](../../../../trace-of-a-commutator.md) is zero. Therefore

$$
\operatorname{tr}(\operatorname{ad}x)=0\qquad(x\in\mathfrak s).
$$

Some $\operatorname{ad}x$ must have a nonzero [eigenvalue](../../../../eigenvalue.md). Otherwise, over the [algebraically closed field](../../../../algebraically-closed-field.md) $k$, every $\operatorname{ad}x$ would be a [nilpotent linear map](../../../../nilpotent-linear-map.md), and the [Engel theorem](../../../../engel-s-theorem.md) would imply that $\mathfrak s$ is a [nilpotent Lie algebra](../../../../nilpotent-lie-algebra.md). This contradicts perfection: the [lower central series of a Lie algebra](../../../../lower-central-series-of-a-lie-algebra.md) $\gamma_1=\mathfrak s$, $\gamma_{r+1}=[\mathfrak s,\gamma_r]$ would equal $\mathfrak s\ne0$ at every step instead of terminating.

Choose such an $x$. Since $[x,x]=0$, zero is an [eigenvalue](../../../../eigenvalue.md) of $\operatorname{ad}x$. Its [trace](../../../../matrix-trace.md) is zero and its [dimension](../../../../dimension-vector-space.md) is three, so the remaining [eigenvalues](../../../../eigenvalue.md) are $\lambda,-\lambda$ with $\lambda\ne0$. These three [eigenvalues](../../../../eigenvalue.md) are distinct in [characteristic zero](../../../../characteristic-zero.md), hence $\operatorname{ad}x$ is [diagonalizable](../../../../diagonalizable-matrix.md). Put $h=2x/\lambda$, and choose nonzero [eigenvectors](../../../../eigenvector.md) $e,f$ with

$$
[h,e]=2e,\qquad[h,f]=-2f.
$$

The zero [eigenspace](../../../../eigenspace.md) is $kh$, so $h,e,f$ form a [basis](../../../../basis.md). Applying the [Jacobi identity](../../../../jacobi-identity.md) gives

$$
[h,[e,f]]=[[h,e],f]+[e,[h,f]]=2[e,f]-2[e,f]=0.
$$

Thus $[e,f]=ch$ for some $c\in k$. If $c=0$, all [Lie brackets](../../../../lie-bracket.md) of [basis vectors](../../../../basis-vector.md) lie in $\langle e,f\rangle$, contradicting $[\mathfrak s,\mathfrak s]=\mathfrak s$. Therefore $c\ne0$, and replacing $f$ by $f/c$ gives $[e,f]=h$.

We have constructed an [sl2 triple](../../../../sl2-triple.md) that is a [basis](../../../../basis.md). The [linear map](../../../../linear-map.md) to the [sl2 Lie algebra](../../../../sl2-lie-algebra.md) sending

$$
e\longmapsto\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad h\longmapsto\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad f\longmapsto\begin{pmatrix}0&0\\1&0\end{pmatrix}
$$

preserves all [Lie brackets](../../../../lie-bracket.md) of [basis vectors](../../../../basis-vector.md) and is bijective. Hence

$$
\boxed{\mathfrak s\cong\mathfrak{sl}_2(k).}
$$

This is the [classification of three-dimensional perfect Lie algebras](../../../../classification-of-three-dimensional-perfect-lie-algebras.md) without appealing to a classification of all [simple Lie algebras](../../../../simple-lie-algebra.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the lie algebras course of Part C of the mathematics course of the University of Oxford](../../../split.md)
5. [Lie algebras course of Part C of the mathematics course of the University of Oxford](../../../../lie-algebras-course-of-part-c-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
