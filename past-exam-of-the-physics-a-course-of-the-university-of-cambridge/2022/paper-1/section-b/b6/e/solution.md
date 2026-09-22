<h1 id="section-b/b6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The specified [energy](../../../../../../energy-split.md) requires $n_x+n_y=2$, so the relevant [energy eigenspace](../../../../../../energy-eigenspace.md) has the [orthonormal basis](../../../../../../orthonormal-basis.md)

$$
|2,0\rangle,\quad |1,1\rangle,\quad |0,2\rangle.
$$

Applying the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) gives

$$
\begin{aligned}
\hat Q|2,0\rangle&=i\sqrt2\hbar|1,1\rangle,\\
\hat Q|1,1\rangle&=-i\sqrt2\hbar|2,0\rangle+i\sqrt2\hbar|0,2\rangle,\\
\hat Q|0,2\rangle&=-i\sqrt2\hbar|1,1\rangle.
\end{aligned}
$$

Thus its [matrix](../../../../../../matrix.md) in this ordered [basis](../../../../../../basis.md) is

$$
Q=\hbar\begin{pmatrix}
0&-i\sqrt2&0\\
i\sqrt2&0&-i\sqrt2\\
0&i\sqrt2&0
\end{pmatrix}.
$$

Writing $q=\hbar\lambda$, the [characteristic polynomial](../../../../../../characteristic-polynomial.md) gives $\lambda(\lambda^2-4)=0$. The possible [angular momentum](../../../../../../angular-momentum.md) [eigenvalues](../../../../../../eigenvalue.md) are therefore

$$
\boxed{q=-2\hbar,\quad0,\quad+2\hbar.}
$$

For completeness, normalized simultaneous [energy](../../../../../../energy-split.md) and [angular momentum](../../../../../../angular-momentum.md) [eigenstates](../../../../../../eigenstate.md) are

$$
\begin{aligned}
|q=+2\hbar\rangle&=\tfrac12\bigl(|2,0\rangle+i\sqrt2|1,1\rangle-|0,2\rangle\bigr),\\
|q=0\rangle&=\tfrac1{\sqrt2}\bigl(|2,0\rangle+|0,2\rangle\bigr),\\
|q=-2\hbar\rangle&=\tfrac12\bigl(|2,0\rangle-i\sqrt2|1,1\rangle-|0,2\rangle\bigr).
\end{aligned}
$$

Each value occurs once in this [energy eigenspace](../../../../../../energy-eigenspace.md). Equivalently, [circular ladder operators of a two-dimensional oscillator](../../../../../../circular-ladder-operators-of-a-two-dimensional-oscillator.md) give $\hat H=\hbar\omega(\hat N_++\hat N_-+1)$ and $\hat L_z=\hbar(\hat N_+-\hat N_-)$. With $N_++N_-=2$, the difference can only be $2,0,-2$.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
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
