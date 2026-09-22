<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [acoustic analogy](../../../../../../acoustic-analogy.md) is an exact rearrangement of the fluid equations into a chosen linear propagation operator acting on an acoustic variable, with everything left over placed on the right as effective forcing. The rearrangement becomes a sound-prediction method only after a reference medium, [boundary conditions](../../../../../../boundary-condition.md) and approximations to the forcing are specified. In particular, a right-hand-side term need not represent independently generated sound.

Use [Einstein summation convention](../../../../../../einstein-notation.md) and write $\partial_i=\partial/\partial x_i$. Differentiating the [continuity equation](../../../../../../continuity-equation.md) in time and taking the divergence of the momentum equation eliminates $\partial_t(\rho u_i)$:

$$
\rho_{tt}=\partial_i\partial_j(\rho u_i u_j-\sigma_{ij})+\nabla^2(p+\chi).
$$

Set $q=p-\widehat p_0$ and $W_{ij}=\rho u_i u_j-\sigma_{ij}$. Since $p+\chi=q+P$, the constant $P$ has zero [Laplacian](../../../../../../laplacian.md). The prescribed reference [mass density](../../../../../../density.md) and reference [speed of sound](../../../../../../speed-of-sound.md) are independent of time, so

$$
Q_{tt}=\frac{q_{tt}}{\widehat c_0^2}-\rho_{tt}.
$$

Combining the two identities gives

$$
\boxed{\left(\widehat c_0^{-2}\partial_t^2-\nabla^2\right)q
=\partial_i\partial_j W_{ij}+\partial_t^2 Q.}
$$

Only [conservation of mass](../../../../../../mass-conservation.md) and [conservation of momentum](../../../../../../momentum-conservation.md) have been used; no equation of state or energy equation was needed. Spatial variation of $\widehat c_0$ creates no omitted derivative in this identity, because it multiplies a time derivative. The double divergence of the [momentum flux](../../../../../../momentum-flux.md) tensor has the structure of an [acoustic quadrupole](../../../../../../acoustic-quadrupole.md).

For a localized flow, choose the reference fields to match the stationary surrounding medium: $\widehat\rho_0=\rho_0$ and $\widehat c_0^2=c_0^2$ outside the flow, with $P$ chosen so $\widehat p_0=p_0$ there. A uniform surrounding fluid permits ambient constant [mass density](../../../../../../density.md) and [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md), giving the familiar homogeneous [wave equation](../../../../../../wave-equation-split.md). A nonuniform surrounding fluid calls for its actual stationary reference profiles, extended sensibly through the flow region. This makes the acoustic variable vanish in the unperturbed exterior and minimizes artificial contrast terms. In a uniform isentropic exterior the leading acoustic relation $p'=c_0^2\rho'$ also makes $Q$ vanish to first order. In a stratified exterior, propagation and [entropy](../../../../../../entropy.md)-advection effects can remain in $Q$, as the next part demonstrates.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
