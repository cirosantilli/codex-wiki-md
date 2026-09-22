<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Separate the defining [matrix exponential](../../../../../matrix-exponential.md) into even and odd powers and use $\tau_j^2=I_2$:

$$
e^{i\alpha_j\tau_j}=I_2\sum_{m=0}^\infty\frac{(-1)^m\alpha_j^{2m}}{(2m)!}
+i\tau_j\sum_{m=0}^\infty\frac{(-1)^m\alpha_j^{2m+1}}{(2m+1)!}
=I_2\cos\alpha_j+i\tau_j\sin\alpha_j.
$$

Therefore

$$
\boxed{A_1=\begin{pmatrix}\cos\alpha_1&i\sin\alpha_1\\i\sin\alpha_1&\cos\alpha_1\end{pmatrix},\qquad
A_2=\begin{pmatrix}\cos\alpha_2&\sin\alpha_2\\-\sin\alpha_2&\cos\alpha_2\end{pmatrix},}
$$



$$
\boxed{A_3=\begin{pmatrix}e^{i\alpha_3}&0\\0&e^{-i\alpha_3}\end{pmatrix}.}
$$

Since each $\tau_j$ is [Hermitian](../../../../../hermitian-operator.md), $A_j^\dagger=\cos\alpha_j I_2-i\sin\alpha_j\tau_j=A_j^{-1}$; each is a [unitary matrix](../../../../../unitary-matrix.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
