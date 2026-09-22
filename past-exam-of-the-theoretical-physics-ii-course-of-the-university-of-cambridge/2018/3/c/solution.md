<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the mode ordering with the $b^\dagger$ operator before the $c^\dagger$ operator, as in the given state. In the sector with one [fermion](../../../../fermion.md) in each subsystem, use the ordered basis

$$
(|B_1C_1\rangle,|B_1C_2\rangle,|B_2C_1\rangle,|B_2C_2\rangle).
$$

The [state vector](../../../../state-vector.md) is $v=(1/2,1/\sqrt2,0,1/2)^T$, whose squared norm is one. Thus the global [density matrix](../../../../density-matrix-split.md) is the rank-one projector

$$
\boxed{\rho_{BC}=vv^\dagger=
\begin{pmatrix}
\frac14&\frac1{2\sqrt2}&0&\frac14\\
\frac1{2\sqrt2}&\frac12&0&\frac1{2\sqrt2}\\
0&0&0&0\\
\frac14&\frac1{2\sqrt2}&0&\frac14
\end{pmatrix}}.
$$

It has [trace](../../../../matrix-trace.md) one and satisfies $\rho_{BC}^2=\rho_{BC}$, so the global state is pure.

Take the [partial trace](../../../../partial-trace.md) over $B$. The conditional vectors in $C$ are $v_1=(1/2,1/\sqrt2)^T$ for $B_1$ and $v_2=(0,1/2)^T$ for $B_2$. Therefore the [reduced density matrix](../../../../reduced-density-matrix.md) is

$$
\boxed{\rho_C=v_1v_1^\dagger+v_2v_2^\dagger
=\begin{pmatrix}\frac14&\frac1{2\sqrt2}\\\frac1{2\sqrt2}&\frac34\end{pmatrix}}.
$$

Its determinant is $1/16$, giving [eigenvalues](../../../../eigenvalue.md)

$$
\lambda_\pm=\frac{2\pm\sqrt3}{4}.
$$

Both are positive; in particular, $\operatorname{Tr}\rho_C^2=7/8<1$, so the reduced state is mixed despite global purity. The [entanglement entropy](../../../../entanglement-entropy.md) is obtained by diagonalizing this reduced [matrix](../../../../matrix.md) and evaluating

$$
\boxed{S_{\mathrm{ent}}=-\lambda_+\ln\lambda_+-\lambda_-\ln\lambda_-}.
$$

For a globally pure bipartite state this equals the entropy of either reduced subsystem. No numerical evaluation is needed.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
