<h1 id="34b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Projecting $H|\Psi\rangle=E|\Psi\rangle$ onto $\langle\psi_n|$ and using orthonormality gives

$$
E_0c_n+\sum_{m=0}^2\langle\psi_n|V|\psi_m\rangle c_m=Ec_n.
$$

Thus, with $d=E_0+\alpha$,

$$
\begin{pmatrix}
d&-A&-A\\
-A&d&-A\\
-A&-A&d
\end{pmatrix}
\begin{pmatrix}c_0\\c_1\\c_2\end{pmatrix}
=E\begin{pmatrix}c_0\\c_1\\c_2\end{pmatrix}.
$$

The symmetric vector $(1,1,1)$ has eigenvalue

$$
E_s=d-2A=E_0+\alpha-2A.
$$

Let $\omega=e^{2\pi i/3}$, so $1+\omega+\omega^2=0$. For either vector

$$
(1,\omega,\omega^2),
\qquad
(1,\omega^2,\omega),
$$

the other two components in each row sum to minus the component in that row. Both therefore have eigenvalue

$$
E_d=d+A=E_0+\alpha+A.
$$

The spectrum is consequently

$$
\boxed{E_0+\alpha-2A,\quad E_0+\alpha+A,\quad E_0+\alpha+A},
$$

with normalized eigenvectors obtained by multiplying the three displayed vectors by $1/\sqrt3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34B](../../34b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
