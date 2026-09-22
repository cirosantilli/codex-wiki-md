<h1 id="1b/solution">Solution</h1>

↑ **Parent:** [1B](../1b.md)

Use the standard complex [inner product](../../../../../inner-product.md) $\langle u,v\rangle=u^*v$, conjugate-linear in its first argument. A [unitary matrix](../../../../../unitary-matrix.md) satisfies $U^*U=I$, and a [Hermitian matrix](../../../../../hermitian-operator.md) satisfies $H^*=H$, where $*$ is conjugate transpose.

If $Hv=\lambda v$ with $v\ne0$, then

$$
\lambda\langle v,v\rangle=\langle v,Hv\rangle=\langle Hv,v\rangle=\overline\lambda\langle v,v\rangle.
$$

Positivity of $\langle v,v\rangle$ proves $\boxed{\lambda\in\mathbb R}$. If $Uv=\lambda v$, preservation of the [norm](../../../../../norm.md) gives $\|v\|^2=\|Uv\|^2=|\lambda|^2\|v\|^2$, so $\boxed{|\lambda|=1}$.

For [eigenvectors](../../../../../eigenvector.md) $Hv=\lambda v$ and $Hw=\mu w$, the [Hermitian matrix](../../../../../hermitian-operator.md) identity gives $\langle v,Hw\rangle=\langle Hv,w\rangle$. The already established reality of the [eigenvalues](../../../../../eigenvalue.md) therefore implies $(\mu-\lambda)\langle v,w\rangle=0$. Thus **distinct [eigenvalues](../../../../../eigenvalue.md) have orthogonal [eigenvectors](../../../../../eigenvector.md)**.

## ↑ Ancestors (10)

1. [1B](../1b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
