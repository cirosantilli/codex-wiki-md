<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

The stationary [Schrödinger equation](../../../../schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\Delta\psi+V\psi=E\psi.
$$

The [Laplacian](../../../../laplacian.md) represents the kinetic-[energy](../../../../energy-split.md) operator. For a [spherically symmetric function](../../../../spherically-symmetric-function.md), $\Delta\psi=\psi''+2\psi'/r$. The attractive [Coulomb potential](../../../../coulomb-potential-energy.md) of the nucleus is $V=-q^2/(4\pi\epsilon_0r)$; $E$ is the [energy](../../../../energy-split.md) [eigenvalue](../../../../eigenvalue.md). Multiplication by $-2m/\hbar^2$ produces the displayed radial equation with [Bohr radius](../../../../bohr-radius.md)

$$
\boxed{a=\frac{4\pi\epsilon_0\hbar^2}{mq^2}.}
$$

For a normalizable bound state, write $\kappa^2=-2mE/\hbar^2$ and take $\lambda>0$. Substitution of $\psi=(A+Br)e^{-\lambda r}$ in

$$
\psi''+\frac2r\psi'+\left(\frac2{ar}-\kappa^2\right)\psi=0
$$

gives, after division by the exponential, the coefficients

$$
\begin{array}{c|c}
r&(\lambda^2-\kappa^2)B\\
1&(\lambda^2-\kappa^2)A-4\lambda B+2B/a\\
1/r&2B-2\lambda A+2A/a.
\end{array}
$$

If $B=0$ and $A\neq0$, these force $\lambda=1/a$ and $\kappa=\lambda$. If $B\neq0$, the first coefficient gives $\kappa^2=\lambda^2$, the second gives $\lambda=1/(2a)$, and the third gives $B=-A/(2a)$. Up to nonzero scalar factors, the two radial bound states and their energies are consequently

$$
\boxed{\begin{aligned}
\psi_1(r)&=e^{-r/a},& E_1&=-\frac{\hbar^2}{2ma^2},\\
\psi_2(r)&=(r-2a)e^{-r/(2a)},&E_2&=-\frac{\hbar^2}{8ma^2}.
\end{aligned}}
$$

They are linearly independent as functions and correspond to different [energy](../../../../energy-split.md) [eigenvalues](../../../../eigenvalue.md). Strictly, they are not two solutions of one fixed-[energy](../../../../energy-split.md) differential equation: each is a solution at its own [energy](../../../../energy-split.md).

For the higher-[energy](../../../../energy-split.md) state, the spherical [Born rule](../../../../born-rule.md) includes the radial factor $4\pi r^2$. Its normalization constant and the angular factor cancel in the ratio

$$
P(r<a)=\frac{\int_0^a r^2(r-2a)^2e^{-r/a}\,dr}
{\int_0^\infty r^2(r-2a)^2e^{-r/a}\,dr}.
$$

The given [integral](../../../../integral-split.md) formula makes the denominator $8a^5$ and the numerator $8a^5-21a^5/e$. Thus

$$
\boxed{P(r<a)=1-\frac{21}{8e}.}
$$

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
