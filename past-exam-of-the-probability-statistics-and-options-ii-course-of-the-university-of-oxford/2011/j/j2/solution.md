<h1 id="j/j2/solution">Solution</h1>

↑ **Parent:** [J2](../j2.md)

The general [time-independent Schrödinger equation](../../../../time-independent-schrodinger-equation.md) is $[-\hbar^2\nabla^2/(2m)+V]\psi=E\psi$. For a spherically symmetric wave function, $\nabla^2\psi=\psi''+2\psi'/r$; the Coulomb attraction between the proton and electron is $V=-q^2/(4\pi\epsilon_0r)$. These supply respectively the kinetic and potential terms in the displayed radial equation. Rearranging identifies

$$
\boxed{a=\frac{4\pi\epsilon_0\hbar^2}{mq^2}}
$$

as the [Bohr radius](../../../../bohr-radius.md).

Substitute $\psi=(A+Br)e^{-\lambda r}$ into the rearranged equation and put $\epsilon=2mE/\hbar^2$. Equating the coefficients of $r,1,r^{-1}$ after cancelling the exponential gives

$$
B(\lambda^2+\epsilon)=0,\qquad
A(\lambda^2+\epsilon)+B(2/a-4\lambda)=0,\qquad
B=(\lambda-1/a)A.
$$

A nonzero state has $A\neq0$. If $B=0$, these identities give $\lambda=1/a$ and $\epsilon=-1/a^2$. If $B\neq0$, they give $\lambda=1/(2a)$, $B=-A/(2a)$, and $\epsilon=-1/(4a^2)$. Thus the two independent eigenfunctions and their corresponding energies are

$$
\boxed{\begin{array}{c|c}
\psi\text{ up to normalization}&E\\\hline
e^{-r/a}&-\hbar^2/(2ma^2)\\
(1-r/(2a))e^{-r/(2a)}&-\hbar^2/(8ma^2)
\end{array}}
$$

They are eigenfunctions at different energies, rather than two independent solutions at one fixed energy.

For the higher-energy state, radial probabilities include the spherical [volume](../../../../volume.md) factor $4\pi r^2$. The normalization constant and $4\pi$ cancel in the ratio. Using the supplied integral at $b=a$ and at infinity,

$$
\Pr(r<a)=\frac{\int_0^ar^2(r-2a)^2e^{-r/a}\,dr}{\int_0^\infty r^2(r-2a)^2e^{-r/a}\,dr}
=\frac{8a^5-21a^5/e}{8a^5}.
$$

Hence

$$
\boxed{\Pr(r<a)=1-\frac{21}{8e}\approx0.0343.}
$$

This calculation fixes the denominator as $8e$ in the source's unparenthesized expression; interpreting it as a product with $e$ would give a negative [probability](../../../../probability.md).

## ↑ Ancestors (12)

1. [J2](../j2.md)
2. [J](../../j.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
