<h1 id="section-c/c11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Between delta barriers, $V=0$ and the [Schrödinger equation](../../../../../../schrodinger-equation.md) gives $\psi''+k^2\psi=0$, with $k^2=2mE/\hbar^2$ for positive [energy](../../../../../../energy-split.md). Write the state and derivative as a two-component vector $\mathbf v=(\psi,\psi')^T$. Free propagation across one interval of length $a$ is

$$
\mathbf v(a^-)=P\mathbf v(0^+),\qquad
P=\begin{pmatrix}\cos ka&\sin ka/k\\-k\sin ka&\cos ka\end{pmatrix}.
$$

The wavefunction is continuous at a delta barrier, while its derivative jumps by $g\psi$, with $g=2m\alpha/\hbar^2$. Thus the barrier matrix is

$$
D=\begin{pmatrix}1&0\\g&1\end{pmatrix},\qquad
\mathbf v(a^+)=M\mathbf v(0^+),\quad M=DP.
$$

[Bloch's theorem](../../../../../../bloch-s-theorem-split.md) requires $\mathbf v(a^+)=e^{i\phi a}\mathbf v(0^+)$. Both $D$ and $P$ have determinant one, so the two eigenvalues of $M$ are $e^{i\phi a}$ and $e^{-i\phi a}$. Taking its trace gives

$$
2\cos(\phi a)=\operatorname{tr}M=2\cos ka+\frac gk\sin ka.
$$

Therefore the [Floquet discriminant of the delta-comb Kronig-Penney model](../../../../../../floquet-discriminant-of-the-delta-comb-kronig-penney-model.md) yields

$$
\boxed{\cos(\phi a)=\cos(ka)+\frac{m\alpha}{\hbar^2k}\sin(ka).}
$$

This trace argument is the one-cell transfer method for the [Kronig-Penney model](../../../../../../kronig-penney-model.md). The loop imposes the additional discrete values of $\phi$ derived in part (b). Real $\phi$ requires the right-hand side to lie in $[-1,1]$, giving allowed [energy bands](../../../../../../energy-band.md); values outside this range are [band gaps](../../../../../../band-gap.md). The strength $\alpha$ has units of [energy](../../../../../../energy-split.md) times length, because a [Dirac delta distribution](../../../../../../dirac-delta-function.md) has units of inverse length.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
