<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Over the [complex numbers](../../../../../complex-number.md), the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) makes every [irreducible polynomial](../../../../../irreducible-polynomial.md) factor $f_j(x)$ equal to $x-\lambda_j$. Part (b)(iv) gives

$$
m_T(x)=\prod_{j=1}^r(x-\lambda_j)
$$

with distinct [eigenvalues](../../../../../eigenvalue.md). The [primary decomposition theorem for linear maps](../../../../../primary-decomposition-theorem-for-linear-maps.md) consequently expresses $V$ as the [direct sum](../../../../../direct-sum.md) of the actual [eigenspaces](../../../../../eigenspace.md) $E_{\lambda_j}=\ker(T-\lambda_jI)$, with no higher [generalized eigenspaces](../../../../../generalized-eigenspace.md) needed. Part (ii) makes these summands mutually [orthogonal](../../../../../orthogonal-vectors.md).

Apply the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to a [basis](../../../../../basis.md) within each [eigenspace](../../../../../eigenspace.md). Its [linear combinations](../../../../../linear-combination.md) stay within that [eigenspace](../../../../../eigenspace.md), so all resulting [vectors](../../../../../vector.md) are still [eigenvectors](../../../../../eigenvector.md). Their union is [orthonormal](../../../../../orthonormal-set.md) by part (ii) and spans $V$ by the [primary decomposition theorem for linear maps](../../../../../primary-decomposition-theorem-for-linear-maps.md). Thus

$$
\boxed{V=\bigoplus_{j=1}^{r} E_{\lambda_j},\qquad
[T]_{\mathcal B}=\operatorname{diag}(\lambda_1I_{\dim E_{\lambda_1}},\ldots,\lambda_rI_{\dim E_{\lambda_r}})}
$$

for an [orthonormal basis](../../../../../orthonormal-basis.md) $\mathcal B$ of [eigenvectors](../../../../../eigenvector.md). This proves the finite-dimensional complex [spectral theorem for normal operators](../../../../../spectral-theorem-for-normal-operators.md) by the requested decomposition argument.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [c](../../c.md)
3. [3](../../../3.md)
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
