<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Apply the [chain rule](../../../../chain-rule.md) to $f_0=f_0(E)$ with $E=H_0(\mathbf J)$:

$$
\mathbf k\cdot\partial_{\mathbf J}f_0=f_0'(E)\mathbf k\cdot\boldsymbol\Omega.
$$

On the [resonance](../../../../resonance.md) selected by the [Dirac delta function](../../../../dirac-delta-function.md), $\mathbf k\cdot\boldsymbol\Omega=k_\phi\Omega_{\mathrm p}$. Thus

$$
\boxed{\mathcal T=\pi(2\pi)^3\Omega_{\mathrm p}\sum_{\mathbf k}k_\phi^2\int|\Psi_{\mathbf k}|^2\bigl[-f_0'(E)\bigr]
\delta\bigl(\mathbf k\cdot\boldsymbol\Omega-k_\phi\Omega_{\mathrm p}\bigr)\,d^3J\geq0.}
$$

Every weight is nonnegative, and $-f_0'(E)>0$. Strict positivity additionally requires a populated nonaxisymmetric [resonance](../../../../resonance.md) with nonzero coupling on a set of positive surface measure. **The unconditional statement is nonnegativity, rather than positive definiteness.** As a concrete counterexample to strict positivity of this formula, retain one nonzero conjugate harmonic pair with $k_\phi\ne0$ and choose its smooth coefficient $\Psi_{\mathbf k}$ supported in an open region $|\Delta_{\mathbf k}|>d>0$. The perturbation is nonzero but has zero resonant coupling, so $\mathcal T=0$ even when $f_0'(E)<0$. The even simpler zero-perturbation case also gives zero. Whether a particular physical [stellar bar](../../../../stellar-bar.md) has nonzero resonant overlap is additional information.

For a coupled [stellar bar](../../../../stellar-bar.md) and halo, the halo gains positive [angular momentum](../../../../angular-momentum.md) and exerts the opposite [torque](../../../../torque.md) on the [stellar bar](../../../../stellar-bar.md). If the halo [mass](../../../../mass.md) is $M_h$ and the rigid [stellar bar](../../../../stellar-bar.md) has constant positive [moment of inertia](../../../../moment-of-inertia.md) $I_b$, then

$$
\boxed{I_b\frac{d\Omega_{\mathrm p}}{dt}=-M_h\mathcal T\leq0.}
$$

This [bar-halo angular-momentum transfer](../../../../bar-halo-angular-momentum-transfer.md) is a form of [dynamical friction](../../../../dynamical-friction.md): a resonantly coupled [stellar bar](../../../../stellar-bar.md) tends to slow down while the [dark matter halo](../../../../dark-matter-halo.md) spins up. Actual long-term evolution changes both the [stellar bar](../../../../stellar-bar.md) pattern and the halo [distribution function](../../../../cumulative-distribution-function.md), so the fixed-pattern response must then be updated. If the [stellar bar](../../../../stellar-bar.md) changes its [moment of inertia](../../../../moment-of-inertia.md), the general relation is $d(I_b\Omega_{\mathrm p})/dt=-M_h\mathcal T$; positive [moment of inertia](../../../../moment-of-inertia.md) alone would not fix the sign of $d\Omega_{\mathrm p}/dt$ without that rigidity assumption.

## ↑ Ancestors (12)

1. [E](../e.md)
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
