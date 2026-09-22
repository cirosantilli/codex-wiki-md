<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A confined [ground state](../../../../ground-state.md) requires $k>0$; take $\alpha>0$ so the trial [wavefunction](../../../../wave-function-split.md) is normalizable. Its normalized form is

$$
f_\alpha(x)=\left(\frac\alpha\pi\right)^{1/4}e^{-\alpha x^2/2}.
$$

The [Gaussian moment recurrence](../../../../gaussian-moment-recurrence.md) gives $\langle x^2\rangle=1/(2\alpha)$ and $\langle x^4\rangle=3/(4\alpha^2)$. Also, [integration by parts](../../../../integration-by-parts.md) gives $\langle p^2\rangle=\hbar^2\int|f_\alpha'|^2dx=\hbar^2\alpha/2$. The [Rayleigh quotient](../../../../rayleigh-quotient.md) for the [quartic oscillator](../../../../quartic-oscillator.md) is consequently

$$
\mathcal E(\alpha)=\frac{\hbar^2\alpha}{4m}+\frac{3k}{4\alpha^2}.
$$

Differentiation yields $\mathcal E'(\alpha)=\hbar^2/(4m)-3k/(2\alpha^3)$, so the unique minimum is at $\alpha_*=(6mk/\hbar^2)^{1/3}$. Since the quotient diverges at both endpoints $0$ and $\infty$, this is the global minimum in the trial family. The [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md) gives

$$
\boxed{E_0\leq\mathcal E(\alpha_*)
=\frac{3\hbar^2}{8m}\left(\frac{6mk}{\hbar^2}\right)^{1/3}.}
$$

For the first excited [energy eigenstate](../../../../energy-eigenstate.md), choose the odd trial family

$$
\boxed{g_\beta(x)=\left(\frac{4\beta^3}{\pi}\right)^{1/4}x e^{-\beta x^2/2},\qquad\beta>0.}
$$

The even confining potential has an even, nodeless [ground state](../../../../ground-state.md), by the [nodeless theorem for a one-dimensional ground state](../../../../nodeless-theorem-for-a-one-dimensional-ground-state.md). By the [Sturm oscillation theorem](../../../../sturm-oscillation-theorem.md), its first excited state is odd with one node. The proposed family has the same [parity operator](../../../../parity-operator.md) eigenvalue and one node, and is orthogonal to the exact ground state, not merely to its Gaussian trial approximation. Minimization in the odd [linear subspace](../../../../vector-subspace.md) therefore bounds the first excited energy from above. For completeness, its [Rayleigh quotient](../../../../rayleigh-quotient.md) is $3\hbar^2\beta/(4m)+15k/(4\beta^2)$, minimized at $\beta^3=10mk/\hbar^2$, giving $E_1\leq(9\hbar^2/8m)(10mk/\hbar^2)^{1/3}$. These are [Gaussian variational bounds for a quartic oscillator](../../../../gaussian-variational-bounds-for-a-quartic-oscillator.md).

If $k=0$, there is no normalizable [free particle](../../../../free-particle.md) ground state on the whole line, though the spectral infimum is zero. If $k<0$, the [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is not bounded below, so a ground-energy bound of the requested kind does not exist.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
