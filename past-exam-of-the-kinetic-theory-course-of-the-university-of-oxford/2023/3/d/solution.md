<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $m=k_\phi$, $B_{\mathbf k}=\mathbf k\cdot\partial_{\mathbf J}f_0$, and let the detuning from the rotating perturbation be

$$
\Delta_{\mathbf k}(\mathbf J)=\mathbf k\cdot\boldsymbol\Omega(\mathbf J)-m\Omega_{\mathrm p}.
$$

Substitute $\delta\Phi_{\mathbf k}=\Psi_{\mathbf k}e^{-im\Omega_{\mathrm p}t}$ into the [linear response in action-angle variables](../../../../linear-response-in-action-angle-variables.md), then set $\tau=t-t'$:

$$
\delta f_{\mathbf k}=iB_{\mathbf k}\Psi_{\mathbf k}e^{-im\Omega_{\mathrm p}t}\int_0^te^{-i\Delta_{\mathbf k}\tau}\,d\tau
=B_{\mathbf k}\Psi_{\mathbf k}e^{-im\Omega_{\mathrm p}t}\frac{1-e^{-i\Delta_{\mathbf k}t}}{\Delta_{\mathbf k}}.
$$

At exact [resonance](../../../../resonance.md) the last quotient is interpreted by its continuous limit $it$. Inserting this response in [c](../c.md) gives

$$
\mathcal T(t)=i(2\pi)^3\sum_{\mathbf k}m\int B_{\mathbf k}|\Psi_{\mathbf k}|^2\frac{1-e^{-i\Delta_{\mathbf k}t}}{\Delta_{\mathbf k}}\,d^3J.
$$

Pair $\mathbf k$ with $-\mathbf k$. Because $B_{-\mathbf k}=-B_{\mathbf k}$, $\Delta_{-\mathbf k}=-\Delta_{\mathbf k}$, and $|\Psi_{-\mathbf k}|^2=|\Psi_{\mathbf k}|^2$, the imaginary cosine terms cancel. The finite-time [torque](../../../../torque.md) is

$$
\boxed{\mathcal T(t)=-(2\pi)^3\sum_{\mathbf k}m\int B_{\mathbf k}|\Psi_{\mathbf k}|^2\frac{\sin(\Delta_{\mathbf k}t)}{\Delta_{\mathbf k}}\,d^3J.}
$$

This is a leading, second-order response in the perturbation amplitude.

For the long-time limit, assume a continuum of occupied [action variables](../../../../action-variable.md), sufficiently smooth integrable weights, convergent harmonic sums, and regular [resonance](../../../../resonance.md) surfaces $\nabla_{\mathbf J}\Delta_{\mathbf k}\ne0$ wherever a contributing surface intersects the distribution. Assume also that the perturbation is weak enough to neglect nonlinear trapping and secular changes in $f_0$, and that the prescribed [stellar bar](../../../../stellar-bar.md) pattern and its coefficients stay fixed. Then [phase mixing](../../../../phase-mixing.md) removes nonresonant transients in the integrated response. The relevant [long-time resonance kernel](../../../../long-time-resonance-kernel.md) is the [distributional convergence](../../../../weak-convergence-of-distributions.md)

$$
\frac{\sin(tx)}x\longrightarrow\pi\delta(x)\qquad(t\to+\infty).
$$

It is not a pointwise limit: at $x=0$ the kernel equals $t$. To justify its use under the [integral](../../../../integral-split.md) over [action variables](../../../../action-variable.md), resolve the integral into detuning surfaces; the [coarea formula](../../../../coarea-formula.md) gives

$$
\int W(\mathbf J)\delta(\Delta_{\mathbf k}(\mathbf J))\,d^3J
=\int_{\Delta_{\mathbf k}=0}\frac{W(\mathbf J)}{|\nabla_{\mathbf J}\Delta_{\mathbf k}|}\,dS.
$$

Smoothness and decay of this surface weight reduce the limit to the one-dimensional [long-time resonance kernel](../../../../long-time-resonance-kernel.md). Equivalently, a causal convergence factor $e^{-\eta\tau}$ gives $\operatorname{Re}\int_0^\infty e^{-\eta\tau-i\Delta\tau}\,d\tau=\eta/(\eta^2+\Delta^2)\to\pi\delta(\Delta)$ as $\eta\downarrow0$.

Therefore the [resonant torque from a rotating perturbation](../../../../resonant-torque-from-a-rotating-perturbation.md) is

$$
\boxed{\mathcal T=-\pi(2\pi)^3\sum_{\mathbf k}k_\phi\int|\Psi_{\mathbf k}|^2\,
\mathbf k\cdot\frac{\partial f_0}{\partial\mathbf J}\,
\delta\bigl(\mathbf k\cdot\boldsymbol\Omega-k_\phi\Omega_{\mathrm p}\bigr)\,d^3J.}
$$

Only orbital [resonances](../../../../resonance.md) contribute to this steady integrated [torque](../../../../torque.md). The limit is a formal weak-perturbation limit, or an intermediate-time approximation after [phase mixing](../../../../phase-mixing.md) but before substantial secular redistribution. It does not prove an unchanged halo can absorb [angular momentum](../../../../angular-momentum.md) at this rate forever. A discrete set of orbital [frequencies](../../../../frequency.md), singular [resonance](../../../../resonance.md) surfaces, or strong trapping can invalidate the stated steady limit.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
