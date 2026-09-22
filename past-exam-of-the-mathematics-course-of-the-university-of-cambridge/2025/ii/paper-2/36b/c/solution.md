<h1 id="36b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the basis $(|\psi_1\rangle,|\psi_2\rangle)$,

$$
H=\begin{pmatrix}E_1&h\\h&E_2\end{pmatrix}.
$$

Writing $\Delta=E_2-E_1>0$, its exact eigenvalues are

$$
\boxed{
E_\pm=\frac{E_1+E_2}{2}
\pm\sqrt{\frac{\Delta^2}{4}+h^2}.}
$$

For the normalized trial state,

$$
\begin{aligned}
E(\beta)
&=E_1\sin^2\beta+E_2\cos^2\beta
+2h\sin\beta\cos\beta\\
&=\frac{E_1+E_2}{2}
+\frac\Delta2\cos2\beta+h\sin2\beta.
\end{aligned}
$$

The minimum of $A\cos2\beta+h\sin2\beta$ is $-\sqrt{A^2+h^2}$ with $A=\Delta/2$. Therefore

$$
\boxed{
\min_\beta E(\beta)
=\frac{E_1+E_2}{2}
-\sqrt{\frac{\Delta^2}{4}+h^2}=E_-.}
$$

The variational estimate is exact because the trial family ranges over all real normalized states in the two-dimensional Hilbert space, and the real symmetric Hamiltonian has a real ground eigenvector.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36B](../../36b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
