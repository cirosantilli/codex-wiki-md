<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [real scalar triplet](../../../../real-scalar-triplet.md), with metric signature $(+---)$, differentiating the [Lagrangian density](../../../../lagrangian-density.md) gives $\partial\mathcal L/\partial\phi_a=-\lambda\phi_a$ and $\partial\mathcal L/\partial(\partial_\mu\phi_a)=\partial^\mu\phi_a$. Hence

$$
\boxed{(\Box+\lambda)\phi_a=0,\qquad
\partial_t^2\phi_a-\nabla^2\phi_a+\lambda\phi_a=0.}
$$

For a constant internal [rotation](../../../../rotation-mathematics.md) parameter, the variation is

$$
\delta\mathcal L=\theta\epsilon_{abc}n_b
\left[(\partial_\mu\phi_a)(\partial^\mu\phi_c)-\lambda\phi_a\phi_c\right]=0.
$$

Each bracketed [tensor](../../../../tensor.md) is symmetric in $a,c$, so its contraction with the antisymmetric symbol vanishes. This rotates the three field components, not the space coordinates; both the kinetic term and common [mass](../../../../mass.md) term are invariant.

For a first-principles [Noether current](../../../../noether-current.md) derivation, temporarily let $\theta$ depend on spacetime. The terms proportional to $\theta$ still cancel, leaving

$$
\delta\mathcal L=j^\mu(\mathbf n)\partial_\mu\theta,\qquad
j^\mu(\mathbf n)=\partial^\mu\phi_a\epsilon_{abc}n_b\phi_c.
$$

On a solution of the field equations, the [action](../../../../action.md) variation for a compactly supported $\theta$ vanishes after [integration by parts](../../../../integration-by-parts.md). Thus $\partial_\mu j^\mu=0$. To match the charges printed in the question, use the equivalent overall sign convention for the [SO(3) Noether current of a real scalar triplet](../../../../so-3-noether-current-of-a-real-scalar-triplet.md)

$$
\boxed{J_a^\mu=\epsilon_{abc}(\partial^\mu\phi_b)\phi_c,\qquad
j^\mu(\mathbf n)=-n_aJ_a^\mu.}
$$

Arbitrariness of $\mathbf n$ gives three [continuity equations](../../../../continuity-equation.md). Their charges are exactly

$$
\boxed{Q_a=\int d^3x\,J_a^0=\int d^3x\,\epsilon_{abc}\dot\phi_b\phi_c.}
$$

An overall reversal of all currents is immaterial; the minus sign above keeps the generator convention distinct from the supplied charge convention.

Direct verification is also short:

$$
\dot Q_a=\int d^3x\,\epsilon_{abc}
[(\nabla^2\phi_b-\lambda\phi_b)\phi_c+\dot\phi_b\dot\phi_c]
=\int_{\partial V}dS\,\epsilon_{abc}(\partial_n\phi_b)\phi_c.
$$

The [mass](../../../../mass.md) term and the products of equal-type derivatives cancel by antisymmetry; [integration by parts](../../../../integration-by-parts.md) produces the boundary term. **The charges are conserved when these integrals exist and the net boundary flux vanishes**: sufficiently decaying fields on all space, [periodic boundary conditions](../../../../periodic-boundary-conditions.md), or suitable symmetry-preserving no-flux boundaries suffice. Arbitrary open boundaries do not. A common constant $\lambda$ is necessary for this internal symmetry; its positivity is a stability issue, not needed for the algebraic conservation proof.

## ↑ Ancestors (14)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
