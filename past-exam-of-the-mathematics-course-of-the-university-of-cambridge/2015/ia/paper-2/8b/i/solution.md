<h1 id="8b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [independence of eigenvectors for distinct eigenvalues](../../../../../../independence-of-eigenvectors-for-distinct-eigenvalues.md) ensures that such [eigenvectors](../../../../../../eigenvector.md) form a [linearly independent](../../../../../../linear-independence.md) set. For completeness, apply $\prod_{j\ne k}(M-\lambda_j I)$ to a proposed relation $\sum_i c_i\mathbf e_i=0$. It leaves $c_k\prod_{j\ne k}(\lambda_k-\lambda_j)\mathbf e_k=0$, so every $c_k=0$. Thus the three [eigenvectors](../../../../../../eigenvector.md) form a [basis](../../../../../../basis.md) over the relevant field and $\mathbf x=\sum_i a_i(t)\mathbf e_i$. Substitution into the [linear system of ordinary differential equations](../../../../../../linear-system-of-differential-equations.md) gives $\sum_i(\dot a_i-\lambda_i a_i)\mathbf e_i=0$; [linear independence](../../../../../../linear-independence.md) implies $\dot a_i=\lambda_i a_i$. Hence

$$
\boxed{\mathbf x(t)=\sum_{i=1}^3 A_i e^{\lambda_i t}\mathbf e_i.}
$$

A real matrix may have a complex conjugate pair of [eigenvalues](../../../../../../eigenvalue.md). In that case the calculation is over $\mathbb C$ and conjugate coefficients yield real solutions; equivalently use real and imaginary parts of the complex modes. No unstated assumption that all three [eigenvalues](../../../../../../eigenvalue.md) are real is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
