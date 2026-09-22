<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $\epsilon_k=\hbar^2k^2/(2m)>0$ for $\mathbf k\ne0$ and $g=u\rho$, using $\rho=N/L^3$. Since the zero mode has zero [kinetic energy](../../../../kinetic-energy.md), the exact [kinetic energy](../../../../kinetic-energy.md) in this trial state is

$$
\boxed{\langle H_{\rm KE}\rangle
=\sum_{\mathbf k\ne0}\epsilon_k\sinh^2\theta_k.}
$$

Together with part (d), the [fixed-mean-number Bogoliubov variational energy](../../../../fixed-mean-number-bogoliubov-variational-energy.md) is

$$
\mathcal E[\theta]\simeq\frac{gN}{2}
+\sum_{\mathbf k\ne0}f_k(\theta_k),\qquad
f_k(\theta)=(\epsilon_k+g)\sinh^2\theta-g\sinh\theta\cosh\theta.
$$

For repulsive [contact interaction](../../../../contact-interaction-quantum-mechanics.md), $u>0$, each $\epsilon_k+g>g>0$. Using the double-angle [hyperbolic-function identities](../../../../hyperbolic-function-identity.md),

$$
f_k(\theta)=\frac{\epsilon_k+g}{2}(\cosh2\theta-1)
-\frac g2\sinh2\theta,
$$

so

$$
f_k'(\theta)=(\epsilon_k+g)\sinh2\theta-g\cosh2\theta.
$$

The [stationary point](../../../../stationary-point.md) therefore satisfies

$$
\boxed{\tanh2\theta_k=\frac{g}{\epsilon_k+g}
=\frac{u\rho}{u\rho+\hbar^2k^2/(2m)}.}
$$

This is a minimum, not just a vanishing [derivative](../../../../derivative.md). Define the positive [Bogoliubov quasiparticle dispersion](../../../../bogoliubov-quasiparticle-dispersion.md)

$$
E_k=\sqrt{(\epsilon_k+g)^2-g^2}
=\sqrt{\epsilon_k(\epsilon_k+2g)}.
$$

At the displayed solution $\theta_k^*$, $\cosh2\theta_k^*=(\epsilon_k+g)/E_k$ and $\sinh2\theta_k^*=g/E_k$. Hence

$$
f_k(\theta)=\frac{E_k}{2}\cosh[2(\theta-\theta_k^*)]
-\frac{\epsilon_k+g}{2},\qquad
f_k''(\theta_k^*)=2E_k>0.
$$

The [hyperbolic cosine](../../../../hyperbolic-cosine.md) has its unique minimum at zero, proving global minimization of each retained term. Treating equal-magnitude [wavevectors](../../../../wavevector.md) together simply multiplies the same function by their multiplicity. At a fixed [ultraviolet cutoff](../../../../ultraviolet-cutoff.md), the resulting [energy](../../../../energy-split.md) change from $\theta=0$ is

$$
\boxed{\mathcal E_{\min}-\mathcal E[0]
=\frac12\sum_{\mathbf k\ne0}(E_k-\epsilon_k-g)<0\quad(g>0).}
$$

Indeed $E_k<\epsilon_k+g$. More directly, for small positive $\theta$,

$$
f_k(\theta)=-g\theta+(\epsilon_k+g)\theta^2+O(\theta^3).
$$

The pair [vacuum expectation value](../../../../vacuum-expectation-value.md) lowers the [interaction energy](../../../../interaction-energy.md) at first order in $\theta$, whereas the nonzero [occupation number](../../../../occupation-number.md) and its [kinetic energy](../../../../kinetic-energy.md) cost start at second order. The [two-mode squeezed vacuum](../../../../two-mode-squeezed-vacuum.md) admixes opposite-[momentum](../../../../momentum-split.md) pairs into the condensate, introducing spatial correlations that reduce the chance of two [bosons](../../../../boson.md) coinciding. These correlations lower repulsive [contact interaction](../../../../contact-interaction-quantum-mechanics.md) enough to outweigh the added [kinetic energy](../../../../kinetic-energy.md). A small [quantum depletion of a Bose condensate](../../../../quantum-depletion-of-a-bose-condensate.md) can therefore lower the [energy](../../../../energy-split.md) below the uncorrelated condensate value.

Two qualifications delimit this result. First, the paper does not state the sign of $u$. More generally a finite stable minimum exists only when $\epsilon_k+g>|g|$ for every retained nonzero mode; repulsion ensures this. For example, with $g=-\epsilon_k$ in some mode, $f_k(\theta)=\epsilon_k\sinh(2\theta)/2$ tends to $-\infty$ as $\theta\to-\infty$, so an unconditional minimum claim for arbitrary $u$ is false. Also the formula minimizes the truncated [Bogoliubov theory](../../../../bogoliubov-theory.md) [energy](../../../../energy-split.md), not the exact quartic [Hamiltonian](../../../../hamiltonian.md) including its discarded terms, and it must remain in the regime of small [quantum depletion of a Bose condensate](../../../../quantum-depletion-of-a-bose-condensate.md).

Second, a three-dimensional unregulated [contact interaction](../../../../contact-interaction-quantum-mechanics.md) cannot give a finite absolute beyond-leading-order [ground-state energy](../../../../ground-state-energy.md) by this bare sum. For large $k$, $E_k-\epsilon_k-g=-g^2/(2\epsilon_k)+O(\epsilon_k^{-2})$, whose three-dimensional sum has an [ultraviolet divergence](../../../../ultraviolet-divergence.md). A finite [ultraviolet cutoff](../../../../ultraviolet-cutoff.md), or [renormalization of a three-dimensional dilute-gas contact coupling](../../../../renormalization-of-a-three-dimensional-dilute-gas-contact-coupling.md) matched to a physical [scattering length](../../../../scattering-length-from-a-partial-wave-s-matrix.md), is needed. This does not alter the modewise minimization or the finite-cutoff lowering mechanism just derived.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
