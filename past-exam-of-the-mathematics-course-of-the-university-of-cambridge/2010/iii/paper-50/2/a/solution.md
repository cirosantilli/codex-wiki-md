<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hermitian operators](../../../../../../hermitian-operator.md) form a [real vector space](../../../../../../real-vector-space.md) of dimension $N^2$. To see that the same basis spans all complex operators, decompose an arbitrary $A$ as $A=B+iC$, where $B=(A+A^\dagger)/2$ and $C=(A-A^\dagger)/(2i)$ are Hermitian. Expand $B,C$ in the real [orthonormal basis](../../../../../../orthonormal-basis.md) and combine their coefficients. The resulting complex expansion is unique because $\operatorname{Tr}(\sigma_m\sigma_k)=\delta_{mk}$. Taking the [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) with $\sigma_m$ gives

$$
\boxed{A=\sum_{k=1}^{N^2}a_k\sigma_k,\qquad a_k=\operatorname{Tr}(\sigma_kA)}.
$$

If $A$ is Hermitian, then $a_k^*=\operatorname{Tr}((\sigma_kA)^\dagger)=\operatorname{Tr}(A\sigma_k)=a_k$ by cyclicity. Hence $\boxed{\vec a\in\mathbb R^{N^2}\text{ for Hermitian }A}$. The basis is a real basis of [Hermitian operators](../../../../../../hermitian-operator.md) and its complexification is a complex basis of all operators.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
