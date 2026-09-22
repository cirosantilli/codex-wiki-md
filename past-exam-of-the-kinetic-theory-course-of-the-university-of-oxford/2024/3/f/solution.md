<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With $C_{\mathbf k}$ and $a$ from [e](../e.md), inversion gives

$$
\delta\Phi_{\mathbf k}^{\mathrm{tot}}(t)=\frac1{2\pi}\int_{\operatorname{Im}\omega=\eta>0}d\omega\,e^{-i\omega t}\frac{iC_{\mathbf k}}{(\omega-a)\epsilon_{\mathbf k}(\omega)}.
$$

For $t>0$, deform the contour downwards. Closing below is clockwise, so the [residue theorem](../../../../residue-theorem.md) multiplies the sum of enclosed residues by $-i$. The forcing pole has residue $iC_{\mathbf k}e^{-iat}/\epsilon_{\mathbf k}(a+i0^+)$ and therefore contributes

$$
\frac{C_{\mathbf k}e^{-iat}}{\epsilon_{\mathbf k}(a+i0^+)}.
$$

A simple collective root $\omega_j$ of the continued [gravitational dielectric function](../../../../gravitational-dielectric-function.md) contributes

$$
\frac{C_{\mathbf k}e^{-i\omega_jt}}{(\omega_j-a)\epsilon_{\mathbf k}'(\omega_j)}.
$$

These are the [Landau mode](../../../../landau-mode.md) transients excited by introducing the mass abruptly. For a strictly damped background they decay, together with any remaining phase-mixing contour contribution under the usual regularity and decay assumptions. Thus

$$
\boxed{\delta\Phi_{\mathbf k}^{\mathrm{tot}}(t)\sim\frac{\delta\Phi_{\mathbf k}^{\mathrm{ext}}(t)}{\epsilon_{\mathbf k}(\mathbf k\cdot\mathbf v_p+i0^+)},\qquad t\to\infty.}
$$

The causal boundary value is what the paper abbreviates by $\epsilon_{\mathbf k}(\mathbf k\cdot\mathbf v_p)$. Physically, the moving mass polarizes the stellar population and carries a [gravitational wake](../../../../gravitational-wake.md). Each spatial harmonic is changed in amplitude and phase by $1/\epsilon_{\mathbf k}$ at the forcing [frequency](../../../../frequency.md). [Self-gravity](../../../../self-gravity.md) can amplify the wake. The induced part alone is $(1/\epsilon_{\mathbf k}-1)\delta\Phi_{\mathbf k}^{\mathrm{ext}}$; the wake's back-reaction on the perturber produces [dynamical friction](../../../../dynamical-friction.md).

The waiting time is controlled by the **slowest excited collective damping**, not just an orbital or crossing time. If $\omega_j=\omega_{rj}-i\Gamma_j$ with $\Gamma_j>0$, then a modal amplitude is suppressed by $e^{-\Gamma_jt}$, and one needs $t\Gamma_j\gg1$ for every appreciably excited mode, together with decay of the phase-mixing remainder. Large transient prefactors can require additional time. Near marginal stability, a relevant $\Gamma_j$ tends to zero and the required waiting time diverges; the stationary wake approximation is then not uniform in the stability parameter.[Sections 2.1–2.2: forcing-pole and Landau-mode contributions, and the nonuniform late-time limit](../../../../the-linear-response-of-stellar-systems-does-not-diverge-at-marginal-stability-by-chris-hamilton-and-tobias-heinemann.md)

**Qualification of stability.** If stable means only non-growing, a persistent neutral mode invalidates the asserted asymptote. A concrete example is a homogeneous [waterbag distribution](../../../../waterbag-distribution.md) with parallel marginal $F(u)=\rho\mathbf1_{|u|<V}/(2V)$. Its [gravitational dielectric function](../../../../gravitational-dielectric-function.md) is

$$
\epsilon_k(\omega)=1-\frac{4\pi G\rho}{k^2V^2-\omega^2}.
$$

For $k^2V^2>4\pi G\rho$, the roots $\omega=\pm\sqrt{k^2V^2-4\pi G\rho}$ are real, so the switch-on transients persist although that harmonic has no growing mode. Taking the smallest box [wavenumber](../../../../wavenumber.md) to satisfy the same inequality makes the whole waterbag model free of growing harmonics. The claimed late-time formula therefore requires damping of all excited modes and $\epsilon_k(a)\ne0$; exact forcing at an undamped root instead produces a secular response.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
