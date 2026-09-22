<h1 id="13b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Legendre's equation is

$$
-\frac d{dx}\left((1-x^2)y'\right)=\lambda y.
$$

With $\langle f,g\rangle=\int_{-1}^1f\bar g\,dx$, integration by parts has no endpoint term because $1-x^2=0$ there, so the operator is self-adjoint. Sturm–Liouville [eigenvalues](../../../../../../eigenvalue.md) are real, can be ordered increasingly, and their eigenfunctions are orthogonal and complete under standard regularity assumptions.

Substitution of $y=\sum a_nx^n$ gives

$$
\frac{a_{n+2}}{a_n}=\frac{n(n+1)-\lambda}{(n+1)(n+2)}.
$$

The [series](../../../../../../series-mathematics.md) terminates at degree $\ell$ when $\lambda=\ell(\ell+1)$. Normalizing at one gives

$$
\boxed{P_1(x)=x,\qquad P_3(x)=\frac12(5x^3-3x).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13B](../../13b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
