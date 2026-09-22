<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in $\mathbb C^N$, the domain of the [matrix](../../../../../../matrix.md) $A$; the printed $\mathbb C^n$ in the introduction is a dimension typo. For a fixed nonempty [support of a vector](../../../../../../support-of-a-vector.md) $S$, write $u$ for the coordinates of $x$ in $S$. Then

$$
\|Ax\|_2^2-\|x\|_2^2=u^*(A_S^*A_S-I_{|S|})u.
$$

The [Gram matrix](../../../../../../gram-matrix.md) $A_S^*A_S$ is a [Hermitian matrix](../../../../../../hermitian-operator.md), so its difference from the [identity matrix](../../../../../../identity-matrix.md) is also a [Hermitian matrix](../../../../../../hermitian-operator.md). By the [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md), its [matrix 2-norm](../../../../../../matrix-2-norm.md) is the largest absolute [eigenvalue](../../../../../../eigenvalue.md), equivalently

$$
\sup_{u\ne0}\frac{|u^*(A_S^*A_S-I_{|S|})u|}{\|u\|_2^2}=\|A_S^*A_S-I_{|S|}\|_{2\to2}.
$$

Indeed, an expansion in an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) bounds every [Rayleigh quotient](../../../../../../rayleigh-quotient.md) by the largest absolute [eigenvalue](../../../../../../eigenvalue.md), and an appropriate [eigenvector](../../../../../../eigenvector.md) attains that bound. The [restricted isometry constant](../../../../../../restricted-isometry-constant.md) must bound this quantity for every $S$ of size at most $s$, and the maximum of these quantities suffices for all [sparse vectors](../../../../../../sparse-vector.md) of order $s$. There are finitely many sets, so the maximum exists. The empty set contributes zero. **Therefore**

$$
\boxed{\delta_s(A)=\max_{|S|\le s}\|A_S^*A_S-I_{|S|}\|_{2\to2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
