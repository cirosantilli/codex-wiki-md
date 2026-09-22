<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Clifford algebra](../../../../../clifford-algebra.md) $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$ and unit-weight antisymmetrization. The duality identity between $\gamma_5\gamma_\nu$ and three antisymmetrized [gamma matrices](../../../../../gamma-matrices.md) turns the equation into

$$
E^\mu:=\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho=0,
\qquad \gamma^{\mu\nu\rho}=\gamma^{[\mu}\gamma^\nu\gamma^{\rho]}.
$$

The overall nonzero factor in this identity depends on the orientation and $\gamma_5$ convention and does not change its solutions. This [Rarita-Schwinger field](../../../../../rarita-schwinger-field.md) equation has the [gauge symmetry](../../../../../gauge-invariance.md)

$$
\Psi_\mu\longmapsto\Psi_\mu+\partial_\mu\epsilon,
$$

since $\gamma^{\mu\nu\rho}\partial_\nu\partial_\rho\epsilon=0$. It is the free-field limit of local [supersymmetry](../../../../../supersymmetry-split.md), so it is suitable for the [gravitino](../../../../../gravitino.md).

To check which [spin](../../../../../spin.md) it propagates, put $A=\gamma^\mu\Psi_\mu$ and $B=\partial^\mu\Psi_\mu$. Expanding the three [gamma matrices](../../../../../gamma-matrices.md) using the [Clifford algebra](../../../../../clifford-algebra.md) gives

$$
E^\mu=\not\partial\Psi^\mu-\partial^\mu A
+\gamma^\mu(\not\partial A-B),
\qquad
\gamma_\mu E^\mu=2(\not\partial A-B)
$$

in four dimensions. Thus the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) requires $B=\not\partial A$. Under the [gauge transformation](../../../../../gauge-transformation.md), $A\mapsto A+\not\partial\epsilon$; locally one may choose gamma-trace [gauge fixing](../../../../../gauge-fixing.md), $A=0$, by solving $\not\partial\epsilon=-A$. The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) then yields

$$
\gamma^\mu\Psi_\mu=0,
\qquad \partial^\mu\Psi_\mu=0,
\qquad \not\partial\Psi_\mu=0.
$$

These are the [massless Dirac equation](../../../../../massless-dirac-equation.md), transversality and gamma-trace constraints that remove the lower-[spin](../../../../../spin.md) part of a vector-spinor.

For a more explicit [massless Rarita-Schwinger polarization count](../../../../../massless-rarita-schwinger-polarization-count.md), take a positive-frequency [plane wave](../../../../../plane-wave.md) with null momentum along the third axis, in signature $(-,+,+,+)$. Transversality relates its temporal and longitudinal components. Residual [gauge transformations](../../../../../gauge-transformation.md) with $\not p\epsilon=0$ remove both. Write the surviving components as $u_1,u_2$; their gamma-trace condition reads $\gamma^1u_1+\gamma^2u_2=0$, hence

$$
u_2=\gamma^1\gamma^2u_1,
\qquad \not p\,u_1=0.
$$

The [massless Dirac equation](../../../../../massless-dirac-equation.md) leaves two complex positive-frequency amplitudes in $u_1$. If $i\gamma^1\gamma^2u_1=s u_1$, $s=\pm1$, then $(u_1,u_2)$ is proportional to $(1,-is)$ in the transverse vector index. With spatial rotation generators $J_3^{\mathrm{vec}}{}_{12}=-i$ and $J_3^{\mathrm{spin}}=-i\gamma^1\gamma^2/2$, the vector has [helicity](../../../../../helicity.md) $-s$ and the [Majorana spinor](../../../../../majorana-spinor.md) has [helicity](../../../../../helicity.md) $-s/2$, giving total [helicity](../../../../../helicity.md) $-3s/2$. The [Majorana spinor](../../../../../majorana-spinor.md) condition fixes the negative-frequency coefficients from these amplitudes. Therefore **a massless gravitino has spin $3/2$, with the two physical helicities $\pm3/2$**. A complex vector-spinor would also have independent antiparticle modes.

The requested count is instead the [off-shell component count of minimal supergravity](../../../../../off-shell-component-count-of-minimal-supergravity.md), before imposing any [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md). A four-dimensional [Majorana spinor](../../../../../majorana-spinor.md) has four real components. Its vector index supplies four copies, and local [supersymmetry](../../../../../supersymmetry-split.md) supplies four real gauge functions:

$$
\boxed{n_{\mathrm{gravitino,off}}=4\times4-4=12.}
$$

One must not additionally subtract transversality and the [massless Dirac equation](../../../../../massless-dirac-equation.md) in this count: those are [on shell](../../../../../on-shell.md) conditions. The gamma-trace [gauge fixing](../../../../../gauge-fixing.md) already uses the same four gauge functions subtracted above. For the [graviton](../../../../../graviton.md), a symmetric [metric tensor](../../../../../metric-tensor.md) has ten real components, with four [diffeomorphism](../../../../../diffeomorphism.md) gauge functions. Equivalently, a [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) has sixteen real components, minus six [local Lorentz transformation](../../../../../local-lorentz-transformation.md) and four [diffeomorphism](../../../../../diffeomorphism.md) functions:

$$
\boxed{n_{\mathrm{graviton,off}}=10-4=16-6-4=6.}
$$

The [gravitino](../../../../../gravitino.md) and [graviton](../../../../../graviton.md) each have two propagating states [on shell](../../../../../on-shell.md), but their off-shell counts disagree by six.

An [auxiliary field](../../../../../auxiliary-field.md) has an algebraic [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) and no propagating kinetic term. In [old-minimal supergravity](../../../../../old-minimal-supergravity.md), a complex scalar $M$ contributes two real bosonic components and a real vector $b_\mu$ contributes four, so the bosonic count becomes $6+2+4=12$, matching the [gravitino](../../../../../gravitino.md). Their [supersymmetry](../../../../../supersymmetry-split.md) transformations also absorb the terms that would otherwise require the propagating [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) to close the local algebra. Thus **auxiliary fields allow off-shell supersymmetry closure and matching component counts without adding physical particles**. Eliminating them recovers an [on shell](../../../../../on-shell.md) formulation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
