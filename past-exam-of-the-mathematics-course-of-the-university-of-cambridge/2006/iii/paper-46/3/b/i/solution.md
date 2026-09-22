<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $v_1=(1,1,1,0)^T$, direct multiplication by the [sample covariance matrix](../../../../../../../sample-covariance-matrix.md) gives

$$
\Sigma v_1=(2250,2250,2250,0)^T=2250v_1.
$$

It is therefore an [eigenvector](../../../../../../../eigenvector.md), with [eigenvalue](../../../../../../../eigenvalue.md) $2250$. Normalization gives $u_1=v_1/\sqrt3$, so the corresponding [sample principal component](../../../../../../../sample-principal-component.md) is

$$
\boxed{Y_1=\frac{(X_1-\bar X_1)+(X_2-\bar X_2)+(X_3-\bar X_3)}{\sqrt3},\qquad\widehat{\operatorname{Var}}(Y_1)=2250.}
$$

Its coefficients are proportional to the required vector. The remaining [eigenvalues](../../../../../../../eigenvalue.md) calculated in (ii) are smaller, confirming that this is the first [principal component](../../../../../../../principal-component.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
