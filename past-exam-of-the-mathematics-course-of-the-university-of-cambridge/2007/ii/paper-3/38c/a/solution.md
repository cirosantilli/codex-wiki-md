<h1 id="38c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\theta_k=k\pi/(M+1)$, extend the proposed [vector](../../../../../../vector.md) by $v_0=v_{M+1}=0$. The sine addition identity gives $v_{i-1}+v_{i+1}=2\cos\theta_k\,v_i$. Thus row-by-row multiplication yields

$$
\boxed{Av^{(k)}=(a+2b\cos\theta_k)v^{(k)},\qquad
\lambda_k=a+2b\cos\frac{k\pi}{M+1}.}
$$

These [vectors](../../../../../../vector.md) do not depend on $a,b$. To prove they form a basis even when [eigenvalues](../../../../../../eigenvalue.md) of $A$ coincide, apply the calculation first to the [symmetric matrix](../../../../../../symmetric-matrix.md) with $a=0,b=1$, whose [eigenvalues](../../../../../../eigenvalue.md) $2\cos\theta_k$ are distinct. Its $M$ nonzero [eigenvectors](../../../../../../eigenvector.md) are orthogonal and form a basis. Their squared lengths are $(M+1)/2$, so multiplying each by $\sqrt{2/(M+1)}$ gives a common [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) for every [matrix](../../../../../../matrix.md) in the family.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
