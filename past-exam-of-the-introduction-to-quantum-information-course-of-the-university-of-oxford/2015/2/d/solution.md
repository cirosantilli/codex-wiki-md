<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a [Hermitian matrix](../../../../hermitian-operator.md) $A$, the [spectral theorem](../../../../spectral-theorem.md) gives $A=U\operatorname{diag}(\lambda_1,\ldots,\lambda_d)U^\dagger$, with real [eigenvalues](../../../../eigenvalue.md) and a [unitary matrix](../../../../unitary-matrix.md) $U$. Hence

$$
A^\dagger A=A^2=U\operatorname{diag}(\lambda_1^2,\ldots,\lambda_d^2)U^\dagger,
\qquad
\sqrt{A^\dagger A}=U\operatorname{diag}(|\lambda_1|,\ldots,|\lambda_d|)U^\dagger.
$$

The square root here is the unique [positive square root of an operator](../../../../positive-square-root-of-an-operator.md). Taking the [trace](../../../../matrix-trace.md), which is unchanged by [unitary similarity](../../../../unitary-similarity.md), proves

$$
\boxed{\|A\|_{\rm tr}=\sum_{j=1}^d|\lambda_j|.}
$$

For a [density matrix](../../../../density-matrix-split.md), all [eigenvalues](../../../../eigenvalue.md) are nonnegative and sum to one. Its [trace norm](../../../../trace-norm.md) is therefore

$$
\boxed{\|\rho\|_{\rm tr}=\operatorname{Tr}\rho=1.}
$$

The absolute values cannot be omitted for a general [Hermitian matrix](../../../../hermitian-operator.md), since positive and negative [eigenvalues](../../../../eigenvalue.md) can cancel in its [trace](../../../../matrix-trace.md) but never in its [trace norm](../../../../trace-norm.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
