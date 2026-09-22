<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [iv](../iv.md)

We prove by [mathematical induction](../../../../../mathematical-induction.md) on $n=\dim V$ that every [linear map](../../../../../linear-map.md) on an $n$-dimensional [complex vector space](../../../../../complex-vector-space.md) admits both triangular forms. For $n=0$ or $1$ this is immediate. When $n>1$, the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) supplies an [eigenvector](../../../../../eigenvector.md) $v$; its [span](../../../../../linear-span.md) $U=\langle v\rangle$ is an [invariant subspace](../../../../../invariant-subspace.md).

By parts (ii) and (iii), $U^0$ has [dimension](../../../../../dimension-vector-space.md) $n-1$ and is an [invariant subspace](../../../../../invariant-subspace.md) of the [dual map](../../../../../transpose-of-a-linear-map.md) $T'$. Apply the induction hypothesis to $T'|_{U^0}$ to choose a [basis](../../../../../basis.md) $\varphi_1,\ldots,\varphi_{n-1}$ with an [upper triangular matrix](../../../../../upper-triangular-matrix.md). Extend it by a [linear functional](../../../../../linear-functional.md) $\varphi_n$ satisfying $\varphi_n(v)=1$. Such a functional exists by [basis extension](../../../../../basis-extension.md), and cannot belong to $U^0$. In this [basis](../../../../../basis.md) of $V'$, the [matrix](../../../../../matrix.md) of $T'$ has the form

$$
C=\begin{pmatrix}B&b\\0&\lambda\end{pmatrix},
$$

where $B$ is an [upper triangular matrix](../../../../../upper-triangular-matrix.md); here the last diagonal entry follows by evaluating $T'\varphi_n$ at $v$, where $Tv=\lambda v$.

There is a [basis](../../../../../basis.md) $e_1,\ldots,e_n$ of $V$ with $\varphi_i(e_j)=\delta_{ij}$, since the [dual basis](../../../../../dual-basis.md) construction gives a finite-dimensional [bidual evaluation map](../../../../../bidual-evaluation-map.md) isomorphism. In particular $e_n=v$. The [matrix transpose](../../../../../transpose.md) relationship for a [dual map](../../../../../transpose-of-a-linear-map.md) gives

$$
[T]_{(e_1,\ldots,e_n)}=C^T,
$$

a [lower triangular matrix](../../../../../lower-triangular-matrix.md). Reversing this [basis](../../../../../basis.md) turns a [lower triangular matrix](../../../../../lower-triangular-matrix.md) into an [upper triangular matrix](../../../../../upper-triangular-matrix.md). If $R$ is the [permutation matrix](../../../../../permutation-matrix.md) reversing the order, we have proved

$$
\boxed{[T]_{(e_1,\ldots,e_n)}=C^T\text{ lower triangular},\qquad
[T]_{(e_n,\ldots,e_1)}=RC^TR\text{ upper triangular}}.
$$

This completes the induction by [triangularization using dual spaces](../../../../../triangularization-using-dual-spaces.md).

## ↑ Ancestors (13)

1. [iv](../iv.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
