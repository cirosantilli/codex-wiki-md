<h1 id="41c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [gradient descent](../../../../../../gradient-descent.md) iteration is

$$
\boxed{x^{(k+1)}=(I-\alpha A)x^{(k)}+\alpha b}.
$$

For the error $e^{(k)}=x^{(k)}-A^{-1}b$,

$$
e^{(k+1)}=(I-\alpha A)e^{(k)}.
$$

Part (a) shows that convergence for every initial vector is equivalent to  
$|1-\alpha\lambda_i|<1$ for every eigenvalue of $A$. Since all eigenvalues are positive,

$$
\boxed{0<\alpha<\frac2{\lambda_{\max}(A)}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [41C](../../41c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
