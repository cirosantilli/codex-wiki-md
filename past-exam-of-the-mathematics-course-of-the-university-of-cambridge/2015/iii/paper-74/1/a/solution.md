<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the inviscid, nonrotating [Boussinesq approximation](../../../../../../boussinesq-approximation.md), with a stable background [mass density](../../../../../../density.md) $\bar\rho(z)$ and reference density $\rho_*$. Write $B=-g\rho'/\rho_*$ for the perturbation [buoyancy](../../../../../../buoyancy.md) and $\pi=p'/\rho_*$ for the kinematic pressure. The [buoyancy frequency](../../../../../../buoyancy-frequency.md) is $N_0^2=-(g/\rho_*)\bar\rho_z>0$. Dropping products of perturbations in the [Boussinesq equations](../../../../../../boussinesq-equations.md) gives the [Linearized Boussinesq equations](../../../../../../linearized-boussinesq-equations.md)

$$
\mathbf u_t=-\nabla\pi+B\mathbf e_z,\qquad B_t+N_0^2w=0,\qquad \nabla\cdot\mathbf u=0.
$$

The last equation expresses [incompressible flow](../../../../../../incompressible-flow.md); the second follows by advecting the background [mass density](../../../../../../density.md) gradient. Neglecting rotation and [viscosity](../../../../../../dynamic-viscosity.md) is part of this [internal gravity wave](../../../../../../internal-wave.md) model.

For a [plane internal gravity wave](../../../../../../plane-internal-gravity-wave.md) proportional to $\exp[i(\mathbf k_h\cdot\mathbf x_h+mz-\omega t)]$, put $\kappa=|\mathbf k_h|>0$ and $K^2=\kappa^2+m^2$. Eliminating the horizontal [velocity](../../../../../../velocity.md), pressure and [buoyancy](../../../../../../buoyancy.md) from the linear equations gives

$$
\boxed{\omega^2=N_0^2\frac{\kappa^2}{\kappa^2+m^2}.}
$$

For example, the horizontal [momentum](../../../../../../momentum.md) and continuity equations give $\pi=-\omega m w/\kappa^2$; substituting $B=-iN_0^2w/\omega$ into vertical [momentum](../../../../../../momentum.md) yields the displayed [dispersion relation](../../../../../../dispersion-relation.md). Thus an [IGW](../../../../../../internal-wave.md) has $0<|\omega|\le N_0$ in this model.

On the positive-frequency branch, the [phase velocity](../../../../../../phase-velocity.md) normal to a constant-phase plane and the [group velocity](../../../../../../group-velocity.md) are

$$
\boxed{\mathbf c_p=\frac{\omega}{K^2}(\mathbf k_h,m),}\qquad
\mathbf c_{g,h}=\frac{N_0m^2}{K^3}\frac{\mathbf k_h}{\kappa},\quad
c_{g,z}=-\frac{N_0\kappa m}{K^3}.
$$

Consequently $(\mathbf k_h,m)\cdot\mathbf c_g=0$, and **phase and [group velocity](../../../../../../group-velocity.md) are perpendicular**. Equivalently, the [dispersion relation](../../../../../../dispersion-relation.md) is homogeneous of degree zero in the [wave vector](../../../../../../wavevector.md), so differentiating with respect to its scale proves the same orthogonality. Energy travels with the [group velocity](../../../../../../group-velocity.md), along the phase planes. At the degenerate limit $m=0$, $\omega=N_0$ and the [group velocity](../../../../../../group-velocity.md) vanishes; the orthogonality statement then has this limiting interpretation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
