<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To obtain the [Boltzmann equation](../../../../boltzmann-equation-split.md), take a dilute [gas](../../../../gas.md) with a short-range [pair potential](../../../../pair-potential.md). Its interaction range is small compared with the [mean free path](../../../../mean-free-path.md) and the spatial scale on which the [phase-space distribution function](../../../../phase-space-distribution-function.md) changes. The [binary collision approximation](../../../../binary-collision-approximation.md) treats encounters as isolated [elastic collisions](../../../../elastic-collision.md); simultaneous encounters involving three or more particles can be neglected. The encounter duration is short compared with the [collision relaxation time](../../../../collision-relaxation-time.md) and macroscopic evolution time, and the external [force](../../../../force-split.md) changes negligibly during an encounter. This permits local, effectively instantaneous scattering at one position $\mathbf x$.

The essential statistical closure is [molecular chaos for the Boltzmann equation](../../../../molecular-chaos-for-the-boltzmann-equation.md): the distribution of _incoming_ pairs factorizes as $ff_\star$. Outgoing pairs need not be independent. Follow each incoming pair through its two-body scattering, and use conservation of [momentum](../../../../momentum-split.md) and [kinetic energy](../../../../kinetic-energy.md), together with time reversal and the invariant scattering measure, to express both gain and loss in the same variables. This gives

$$
C_B[f](\mathbf v)=\int d^3v_\star\int_{\mathrm{hemisphere}}d\Omega\,B(g,\theta)\left(f'f'_\star-ff_\star\right),\qquad g=|\mathbf v-\mathbf v_\star|.
$$

Here $d\Omega=\sin\theta\,d\theta\,d\varphi$; when the measure is written as $d\theta\,d\varphi$, its Jacobian is included in the [Boltzmann scattering kernel](../../../../boltzmann-scattering-kernel.md). In a scattering-angle convention, that kernel contains relative [speed](../../../../speed.md) times differential [scattering cross-section](../../../../scattering-cross-section.md). The hemisphere prevents double counting equivalent outcomes for indistinguishable particles; the precise factor is included in $B$. The primed [velocities](../../../../velocity.md) are connected to the unprimed ones by the reversible [elastic collision](../../../../elastic-collision.md) map. This closure is appropriate for a dilute short-range [gas](../../../../gas.md), rather than a generic long-range interacting system with an important collective [mean-field theory](../../../../mean-field-theory.md) contribution.

The further replacement by the [BGK model](../../../../bgk-model.md) is a phenomenological relaxation closure. Replace the full [nonlinear Boltzmann collision operator](../../../../nonlinear-boltzmann-collision-operator.md) by relaxation towards a [local Maxwellian](../../../../local-maxwellian.md), with a single, velocity-independent [collision relaxation time](../../../../collision-relaxation-time.md) $\tau>0$:

$$
C_{\mathrm{BGK}}[f]=-\frac{f-f^{(0)}}{\tau},\qquad f^{(0)}=\frac{\rho}{(2\pi\Theta)^{3/2}}\exp\left(-\frac{|\mathbf v-\mathbf u|^2}{2\Theta}\right).
$$

It models relaxation towards a [local Maxwellian](../../../../local-maxwellian.md) without resolving the detailed scattering. Treating $\tau$ as constant is an additional simplification; it is of the order of a mean time between effective collisions. Near a [local Maxwellian](../../../../local-maxwellian.md), departures in the nonconserved [velocity moments](../../../../velocity-moment.md) decay on this timescale.

Choose $f^{(0)}$ to match the [collision invariants](../../../../collision-invariant.md) $1$, $\mathbf v$ and $|\mathbf v|^2$ of $f$. For unit particle [mass](../../../../mass.md), this means

$$
\boxed{\rho=\int f\,d^3v,\qquad \mathbf u=\rho^{-1}\int\mathbf v f\,d^3v,\qquad \Theta=\frac{1}{3\rho}\int|\mathbf v-\mathbf u|^2f\,d^3v.}
$$

Here $\rho$ is the [mass density](../../../../density.md), $\mathbf u$ is the [mean velocity](../../../../mean-velocity-of-a-kinetic-distribution.md), and $\Theta$ is the [temperature](../../../../temperature-split.md) in squared-[velocity](../../../../velocity.md) units, $\Theta=k_BT/m$ before setting $m=1$. In particular,

$$
\int (1,\mathbf v,|\mathbf v|^2)\,C_{\mathrm{BGK}}[f],d^3v=0.
$$

Thus relaxation preserves local [mass](../../../../mass.md), [momentum](../../../../momentum-split.md) and [kinetic energy](../../../../kinetic-energy.md) rather than relaxing them to externally prescribed values.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
