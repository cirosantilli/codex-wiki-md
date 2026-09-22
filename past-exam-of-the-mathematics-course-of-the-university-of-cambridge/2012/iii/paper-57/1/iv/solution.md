<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Now impose the stipulated negligible shear and work where $\Pi\ne0$. The [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md), [momentum constraint](../../../../../../momentum-constraint.md) and local expansion evolution give

$$
H^2=\frac{8\pi G}{3}(\tfrac12\Pi^2+V),\qquad \partial_iH=-4\pi G\Pi\partial_i\phi,\qquad \dot H=-4\pi GN\Pi^2.
$$

Time differentiation of the first equation, followed by $\dot\phi=N\Pi$, gives $\dot\Pi=-N(3H\Pi+V_{,\phi})$. Spatial differentiation of the same equation and use of the [momentum constraint](../../../../../../momentum-constraint.md) gives

$$
\Pi\partial_i\Pi+V_{,\phi}\partial_i\phi=-3H\Pi\partial_i\phi,\qquad
\partial_i\Pi=-(3H+V_{,\phi}/\Pi)\partial_i\phi.
$$

These are the temporal and spatial identities needed for the [nonlinear curvature covector](../../../../../../nonlinear-curvature-covector.md). Differentiate its definition, keeping the spatially varying [lapse function](../../../../../../lapse-function.md):

$$
\dot\zeta_i=-\partial_i(NH)+\left[-4\pi GN\Pi+\frac{NH(3H\Pi+V_{,\phi})}{\Pi^2}\right]\partial_i\phi+\frac H\Pi\partial_i(N\Pi).
$$

The terms proportional to $\partial_iN$ cancel. The terms $-N\partial_iH$ and $-4\pi GN\Pi\partial_i\phi$ cancel by the [momentum constraint](../../../../../../momentum-constraint.md), and the remaining two terms cancel by the spatial momentum identity. Therefore

$$
\boxed{\dot\zeta_i\simeq0}
$$

to the retained gradient order. No homogeneous-lapse assumption was needed.

For linear [adiabatic cosmological perturbations](../../../../../../adiabatic-initial-conditions.md), expansion of the local scale and [scalar field](../../../../../../scalar-field.md) gives $\zeta_i=\partial_i[\Psi+\bar H\delta\phi/\bar\Pi]$. For nonzero spatial modes, linearizing the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) and the [momentum constraint](../../../../../../momentum-constraint.md) gives

$$
\delta\rho=\frac{3\bar H}{4\pi G}\delta H=-3\bar H\bar\Pi\delta\phi,\qquad \bar\rho+\bar P=\bar\Pi^2.
$$

Thus

$$
\boxed{\zeta_i\simeq\partial_i\left[\Psi-\frac{\delta\rho}{3(\bar\rho+\bar P)}\right]=\partial_i\zeta.}
$$

This uses the paper's overall sign for the [uniform-density curvature perturbation](../../../../../../uniform-density-curvature-perturbation.md); the opposite overall sign is also common. For an adiabatic single-field attractor, [superhorizon conservation of single-field comoving curvature](../../../../../../superhorizon-conservation-of-single-field-comoving-curvature.md) allows the primordial amplitude to be transported through later epochs without following every short-scale process. This proof specifically discarded the shear contribution to the [momentum constraint](../../../../../../momentum-constraint.md) and assumed a usable field clock. It is not a claim that every single-field background conserves every curvature mode: [growing curvature perturbation in ultra-slow-roll inflation](../../../../../../growing-curvature-perturbation-in-ultra-slow-roll-inflation.md) is a non-attractor counterexample, and $\Pi=0$ makes this particular covector undefined.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
