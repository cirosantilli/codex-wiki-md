<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the [eigenvalue equation](../../../../../eigenvalue-equation.md) along the assumed smooth normalized eigenbranch:

$$
A'x+Ax'=\lambda'x+\lambda x'.
$$

Since $A$ is real symmetric, $x^TA=\lambda x^T$. Multiplying the differentiated equation by $x^T$ and using $x^Tx=1$ cancels the terms containing $x'$:

$$
x^TA'x+\lambda x^Tx'=\lambda'+\lambda x^Tx'.
$$

Thus the finite-dimensional [Hellmann–Feynman theorem](../../../../../hellmann-feynman-theorem.md) gives

$$
\boxed{\left.\frac{d\lambda}{d\epsilon}\right|_{\epsilon=0}=x(0)^T\left.\frac{dA}{d\epsilon}\right|_{\epsilon=0}x(0).}
$$

Equivalently, differentiating the normalization gives $2x^Tx'=0$ and eliminates those terms from the [derivative](../../../../../derivative.md) of $\lambda=x^TAx$. The proof needs the smooth eigenbranch assumed in the question; the smallest [eigenvalue](../../../../../eigenvalue.md) need not be differentiable at an arbitrary crossing without that assumption.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
