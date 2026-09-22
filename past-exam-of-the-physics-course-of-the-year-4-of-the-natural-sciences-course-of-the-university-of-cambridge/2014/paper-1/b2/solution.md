<h1 id="b2/solution">Solution</h1>

↑ **Parent:** [B2](../b2.md)

Perturbation theory expands known [eigenvalues](../../../../eigenvalue.md) and [eigenfunctions](../../../../eigenfunction.md) about a solvable Hamiltonian. Small corrections require appropriate energy-gap and matrix-element scales; degeneracies must first be diagonalized within their subspace. The [variational method](../../../../variational-method.md) instead minimizes a normalized trial state's [energy](../../../../energy-split.md) expectation. It gives an upper bound on the ground [energy](../../../../energy-split.md) without requiring a small perturbation; excited-state bounds need orthogonality constraints or an appropriate symmetry subspace.

Normalize the unperturbed oscillator states:

$$
|\psi_0|^2=\frac\alpha{\sqrt\pi}e^{-\alpha^2x^2},\qquad
|\psi_1|^2=\frac{2\alpha^3}{\sqrt\pi}x^2e^{-\alpha^2x^2}.
$$

For the [Gaussian perturbation of a quantum harmonic oscillator](../../../../gaussian-perturbation-of-a-quantum-harmonic-oscillator.md), the first-order shifts are its expectation values:

$$
\boxed{\Delta E_0=\frac{V_0\alpha}{\sqrt{\alpha^2+\beta^2}},\qquad
\Delta E_1=\frac{V_0\alpha^3}{(\alpha^2+\beta^2)^{3/2}}.}
$$

For $\beta\gg\alpha$, they scale as $V_0\alpha/\beta$ and $V_0(\alpha/\beta)^3$ respectively: a narrow central perturbation couples weakly to the odd state's central [node](../../../../node-dynamical-systems.md). For $\beta\ll\alpha$, both approach $V_0$ because the perturbation is nearly constant over the wavefunctions. The leading corrections are $V_0[1-\beta^2/(2\alpha^2)]$ and $V_0[1-3\beta^2/(2\alpha^2)]$.

For an improved variational estimate, replace the fixed width $\alpha$ by an adjustable positive width $s$ in each even/odd Gaussian. Their [energy](../../../../energy-split.md) functionals are

$$
E_{\rm even}(s)=\frac{\hbar^2s^2}{4m}+\frac{m\omega^2}{4s^2}
+\frac{V_0s}{\sqrt{s^2+\beta^2}},
$$



$$
E_{\rm odd}(s)=\frac{3\hbar^2s^2}{4m}+\frac{3m\omega^2}{4s^2}
+\frac{V_0s^3}{(s^2+\beta^2)^{3/2}}.
$$

Minimize each separately. At $s=\alpha$ they recover the unperturbed [energy](../../../../energy-split.md) plus the first-order shift, so optimization cannot raise those trial estimates. For this even one-dimensional potential the lowest odd state is the first [excited state](../../../../excited-state.md), making its odd-sector minimum an upper bound on $E_1$. Enlarging each parity-preserving trial basis can improve the estimates further.

## ↑ Ancestors (12)

1. [B2](../b2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
