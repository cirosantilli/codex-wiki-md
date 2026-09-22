<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\alpha=\Delta\tau/\hbar$ and $\beta=Ex_0\tau/\hbar$. The [Pauli matrix multiplication law](../../../../pauli-matrix-multiplication-law.md) gives the [pulse-and-precession spin one-half map](../../../../pulse-and-precession-spin-one-half-map.md)

$$
U_\Delta U_E=CI-i\mathbf v\cdot\boldsymbol\sigma,\quad C=\cos\alpha\cos\beta,\quad
\mathbf v=(\cos\alpha\sin\beta,-\sin\alpha\sin\beta,-\sin\alpha\cos\beta).
$$

Because $C^2+|\mathbf v|^2=1$, a suitable [angle](../../../../angle.md) and [unit vector](../../../../unit-vector.md) for the [rotation](../../../../rotation-mathematics.md) are

$$
\boxed{\theta=2\arccos(\cos\alpha\cos\beta),\qquad
\mathbf n=\frac{(\cos\alpha\sin\beta,-\sin\alpha\sin\beta,-\sin\alpha\cos\beta)}{\sqrt{1-\cos^2\alpha\cos^2\beta}}.}
$$

If the denominator vanishes, $U=\pm I$ and the axis is arbitrary. The [Bloch vector](../../../../bloch-vector.md) $\mathbf r=\langle\boldsymbol\sigma\rangle$ rotates through $\theta$ about $\mathbf n$ per period; after $N$ periods the angle is $N\theta$. The eigenphases equivalently give [quasienergies](../../../../quasienergy.md) $\pm\hbar\theta/(2\tau)$ modulo $2\pi\hbar/\tau$.

In the two-orbital subspace the position operator is $X=x_0\sigma_x$. The [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md) between pulses gives $P/m=(i/\hbar)[H_0,X]=(2\Delta x_0/\hbar)\sigma_y$, hence

$$
\langle X\rangle=x_0r_x,\qquad \langle P\rangle=\frac{2m\Delta x_0}{\hbar}r_y.
$$

Thus two components of the [Bloch vector](../../../../bloch-vector.md) directly describe the mean [position](../../../../position.md) and [momentum](../../../../momentum-split.md); its third gives the orbital population imbalance. The electric kick rotates about the position axis, leaving $\langle X\rangle$ unchanged at the kick, while free evolution mixes the position and momentum components. Starting in $|1s\rangle$, one complete period gives

$$
\mathbf r=(-\sin2\alpha\sin2\beta,-\cos2\alpha\sin2\beta,\cos2\beta),
$$

which exhibits the induced motion explicitly. These are projected two-orbital [observables](../../../../observable.md).

## ↑ Ancestors (14)

1. [D](../d.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
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
