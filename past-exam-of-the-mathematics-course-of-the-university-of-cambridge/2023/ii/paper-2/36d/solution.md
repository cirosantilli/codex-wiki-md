<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

For any nonzero state, the [Rayleigh quotient](../../../../../rayleigh-quotient.md) is

$$
R[\psi]=\frac{\langle\psi|\widehat H|\psi\rangle}
{\langle\psi|\psi\rangle}.
$$

Expand $|\psi\rangle=\sum_nc_n|\psi_n\rangle$ in normalized energy eigenstates. Then

$$
R[\psi]=\frac{\sum_n|c_n|^2E_n}{\sum_n|c_n|^2}
\geq E_0.
$$

Because the ground state is unique, equality holds exactly when all coefficients except $c_0$ vanish. Thus the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) gives its minimum at the ray of $|\psi_0\rangle$.

For the proposed exact state, write $\widetilde\psi=e^{-\beta x^n}$. Its logarithmic derivatives give

$$
\frac{\widetilde\psi''}{\widetilde\psi}
=\beta^2n^2x^{2n-2}-\beta n(n-1)x^{n-2}.
$$

The stationary Schrödinger equation, after multiplication by $2m/\hbar^2$, is

$$
\left[-\frac{d^2}{dx^2}+x^6-3x^2+2\right]\widetilde\psi
=\varepsilon\widetilde\psi,
\qquad E=\frac{\hbar^2}{2m}\varepsilon.
$$

Matching the highest power requires $2n-2=6$, so $n=4$, and cancellation of $x^6$ requires $16\beta^2=1$. Normalizability selects $\beta=1/4$. Then $12\beta=3$ also cancels the quadratic term, leaving $\varepsilon=2$. Therefore

$$
\boxed{n=4,\qquad\beta=\frac14,\qquad E=\frac{\hbar^2}{m}.}
$$

This is the [exact ground state of a solvable sextic potential](../../../../../exact-ground-state-of-a-solvable-sextic-potential.md) candidate $e^{-x^4/4}$.

For the Gaussian trial state $\psi_\alpha=e^{-\alpha x^2/2}$, normalization cancels from the quotient. With respect to the probability density proportional to $e^{-\alpha x^2}$,

$$
\langle x^2\rangle=\frac1{2\alpha},
\qquad
\langle x^6\rangle=\frac{15}{8\alpha^3},
\qquad
\left\langle-\frac{d^2}{dx^2}\right\rangle=\frac\alpha2.
$$

Hence

$$
R[\psi_\alpha]
=\frac{\hbar^2}{2m}\varepsilon(\alpha),
\qquad
\varepsilon(\alpha)
=2+\frac\alpha2-\frac3{2\alpha}+\frac{15}{8\alpha^3}.
$$

The stationary equation is

$$
\varepsilon'(\alpha)=0
\quad\Longleftrightarrow\quad
4\alpha^4+12\alpha^2-45=0.
$$

Writing $z=\alpha^2$, the quadratic has exactly one positive root,

$$
z=\frac{-3+3\sqrt6}{2}
=\frac{-3+\sqrt{54}}2.
$$

Since the quotient tends to infinity as $\alpha\downarrow0$ or $\alpha\to\infty$, this is the unique global minimizer. Thus

$$
\boxed{p=-3,\qquad q=54,\qquad
\alpha_*=\sqrt{\frac{-3+\sqrt{54}}2}.}
$$

Using the stationary equation to replace $15/(8\alpha_*^3)$ by $\alpha_*/6+1/(2\alpha_*)$ gives the best estimate

$$
\boxed{
E_0^*=\frac{\hbar^2}{2m}
\left(2+\frac{2\alpha_*}{3}-\frac1{\alpha_*}\right).}
$$

This is the [Gaussian variational estimate for a solvable sextic potential](../../../../../gaussian-variational-estimate-for-a-solvable-sextic-potential.md).

The exact eigenfunction $e^{-x^4/4}$ is positive and has no nodes. The [nodeless theorem for a one-dimensional ground state](../../../../../nodeless-theorem-for-a-one-dimensional-ground-state.md) therefore identifies it as the true ground state, with dimensionless energy $2$. The variational value is consistent: since $\alpha_*^2>3/2$,

$$
\frac{2\alpha_*}{3}-\frac1{\alpha_*}>0,
$$

so $E_0^*>\hbar^2/m=E_0$, as every trial-state upper bound must satisfy.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
