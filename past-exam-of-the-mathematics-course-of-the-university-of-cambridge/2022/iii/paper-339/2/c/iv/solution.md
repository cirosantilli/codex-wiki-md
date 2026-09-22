<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $C=\{x:Ax\geq b\}$, primal [projected gradient descent](../../../../../../../projected-gradient-descent.md) is

$$
\boxed{x_{k+1}=P_C[(I-\eta Q)x_k],
\qquad 0<\eta\leq\lambda_{\max}(Q)^{-1}.}
$$

Projection onto $C$ is itself a constrained quadratic program. The dual method only projects componentwise onto $\mathbb R_+^m$ and uses the fixed matrix $AQ^{-1}A^T$, so its iterations can be substantially cheaper, especially when $Q^{-1}$ can be prefactored and the number of constraints is moderate.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
