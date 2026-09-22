<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For distinct [eigenvalues](../../../../../../eigenvalue.md), the formula holds for $n=0,1$. If the lower-left entry of $L^n$ is $b_n=(\lambda_1^n-\lambda_2^n)/(\lambda_1-\lambda_2)$, multiplication by $L$ gives $b_{n+1}=\lambda_1b_n+\lambda_2^n=(\lambda_1^{n+1}-\lambda_2^{n+1})/(\lambda_1-\lambda_2)$. This proves by [mathematical induction](../../../../../../mathematical-induction.md) that

$$
L^n=\begin{pmatrix}\lambda_1^n&0\\(\lambda_1^n-\lambda_2^n)/(\lambda_1-\lambda_2)&\lambda_2^n\end{pmatrix}.
$$

Summing the absolutely convergent [matrix exponential](../../../../../../matrix-exponential.md) series gives

$$
\boxed{A(t)=e^{Lt}=\begin{pmatrix}e^{\lambda_1t}&0\\\dfrac{e^{\lambda_1t}-e^{\lambda_2t}}{\lambda_1-\lambda_2}&e^{\lambda_2t}\end{pmatrix}.}
$$

For the repeated [eigenvalue](../../../../../../eigenvalue.md) $\lambda_1=\lambda_2=\lambda$, the continuous limit is $A(t)=e^{\lambda t}\begin{pmatrix}1&0\\t&1\end{pmatrix}$. This is also the exponential of a two-dimensional [Jordan block](../../../../../../jordan-block.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
