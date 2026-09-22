<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A basis of [Hermitian matrices](../../../../../../hermitian-operator.md) is a real basis for the Hermitian subspace, but it also supplies a complex basis for all matrices. Indeed every operator has the decomposition

$$
A=B+iC,\qquad B=\frac{A+A^\dagger}{2},\qquad
C=\frac{A-A^\dagger}{2i},
$$

with $B,C$ Hermitian. Expand each in the given real basis, then combine their coefficients to expand $A$. Orthogonality for the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) determines those complex coefficients uniquely:

$$
\operatorname{Tr}(\sigma_jA)=\sum_k a_k\operatorname{Tr}(\sigma_j\sigma_k)=a_j.
$$

Consequently

$$
\boxed{A=\sum_{k=1}^{N^2}\operatorname{Tr}(\sigma_kA)\sigma_k.}
$$

If $A$ is Hermitian, cyclicity of the [trace](../../../../../../matrix-trace.md) gives

$$
a_j^*=\operatorname{Tr}[(\sigma_jA)^\dagger]
=\operatorname{Tr}(A\sigma_j)=\operatorname{Tr}(\sigma_jA)=a_j.
$$

Thus its coordinate vector is real. The product $\sigma_jA$ need not itself be Hermitian; [trace](../../../../../../matrix-trace.md) cyclicity is what justifies the conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
