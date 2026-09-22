<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p_T=nk_BT$, $C=\langle\mathbf R\mathbf R^T\rangle$, and $M=I+\alpha\sigma$, so the single-bead [mobility](../../../../hydrodynamic-mobility-matrix.md) is $M/\zeta$. Assume an [incompressible solvent](../../../../incompressible-flow.md), constant $n,H,T,\zeta$, negligible [bead inertia](../../../../inertia.md), and a symmetric [positive-definite](../../../../positive-definite-matrix.md) $M$. The last requirement makes the [resistance](../../../../hydrodynamic-resistance-matrix.md) invertible and [Brownian diffusion](../../../../diffusion.md) physically admissible. At a given position and time, $M$ depends on the moment $C$ but not on the individual configuration $\mathbf R$.

Use the source's [gradient](../../../../gradient.md) convention $K_{ij}=\partial_i u_j$, and write $G=K^T$ for the [component-first gradient](../../../../velocity-gradient.md). Then $\mathbf u(\mathbf r_2)-\mathbf u(\mathbf r_1)\simeq G\mathbf R$. The [spring forces](../../../../hooke-s-law.md) on the two beads are $\mathbf F_1=H\mathbf R$ and $\mathbf F_2=-H\mathbf R$. Their overdamped [probability currents](../../../../fokker-planck-probability-current.md) are

$$
\mathbf j_i=\mathbf u_i\psi+\frac M\zeta
\left(\mathbf F_i\psi-k_BT\nabla_{\mathbf r_i}\psi\right).
$$

Here the [Brownian term](../../../../brownian-motion-split.md) written as $-k_BT\nabla\psi$ is a [force](../../../../force-split.md) weighted by [probability density](../../../../probability-density.md). Its corresponding conditional [osmotic force](../../../../osmotic-pressure.md) is $-k_BT\nabla\log\psi$; treating the given term as an unweighted deterministic [force](../../../../force-split.md) per bead would not produce the stated [Fokker–Planck equation](../../../../fokker-planck-equation.md).

With midpoint $\mathbf x=(\mathbf r_1+\mathbf r_2)/2$, the derivatives are $\nabla_{r_1}=\tfrac12\nabla_x-\nabla_R$ and $\nabla_{r_2}=\tfrac12\nabla_x+\nabla_R$. Subtracting the bead currents gives the [configuration current](../../../../fokker-planck-probability-current.md)

$$
\boxed{\mathbf j_R=G\mathbf R\psi-
\frac{2H}{\zeta}M\mathbf R\psi-
\frac{2k_BT}{\zeta}M\nabla_R\psi.}
$$

The [midpoint current](../../../../fokker-planck-probability-current.md) is $\mathbf u\psi$ after neglecting the specified spatial [Brownian diffusion](../../../../diffusion.md). [Configuration probability conservation](../../../../continuity-equation.md) therefore gives

$$
\boxed{\partial_t\psi+\mathbf u\cdot\nabla_x\psi+
\nabla_R\cdot\left(G\mathbf R\psi-\frac{2H}{\zeta}M\mathbf R\psi\right)
=\frac{2k_BT}{\zeta}\nabla_R\cdot(M\nabla_R\psi).}
$$

Since $G\mathbf R$ has components $R_j\partial_j u_i$, this agrees with the source's $\mathbf R\cdot\nabla\mathbf u$. The factor two in both spring relaxation and configuration [diffusivity](../../../../diffusion-coefficient.md) comes from relative motion of both beads.

The [second moment](../../../../second-moment.md) $C$ is the unnormalized [conformation tensor](../../../../conformation-tensor.md). Now multiply by $R_iR_j$ and integrate over [configuration space](../../../../mechanical-configuration-space.md). Assume sufficiently decaying tails so every boundary term at infinite separation vanishes. The affine current gives $GC+CG^T$; spring drift gives $-(2H/\zeta)(MC+CM)$; two [integrations by parts](../../../../integration-by-parts.md) of [diffusion](../../../../diffusion.md) give $(4k_BT/\zeta)M$. Hence

$$
D_tC-GC-CG^T=-\frac{2H}{\zeta}(MC+CM)+\frac{4k_BT}{\zeta}M,
\qquad D_t=\partial_t+\mathbf u\cdot\nabla_x.
$$

Because $\sigma=nHC-p_TI$, $M$ is a [polynomial](../../../../polynomial-split.md) in $C$ and [commutes](../../../../commuting-operators.md) with it. Thus

$$
C^{\nabla}\equiv D_tC-GC-CG^T
=-\frac{4H}{\zeta}M\left(C-\frac{k_BT}{H}I\right).
$$

This is the [Hookean dumbbell conformation equation with anisotropic mobility](../../../../hookean-dumbbell-conformation-equation-with-anisotropic-mobility.md), an exact [second-moment closure](../../../../moment-closure.md) within the stated model; no [Gaussian approximation](../../../../normal-distribution.md) to $\psi$ was needed.

The [upper-convected derivative](../../../../upper-convected-derivative.md) of the [identity](../../../../identity-matrix.md) is $I^{\nabla}=-(G+G^T)$. Applying it to the [polymer stress](../../../../stress.md) therefore gives

$$
\sigma^{\nabla}=-\frac{4H}{\zeta}M\sigma+p_T(G+G^T).
$$

Consequently the coefficients and the closed [stress equation](../../../../constitutive-equation.md) are

$$
\boxed{\lambda=\frac{\zeta}{4H},\qquad
\mu=\lambda p_T=\frac{n k_BT\zeta}{4H},\qquad
\lambda\sigma^{\nabla}+\sigma+\alpha\sigma^2
=\mu(K+K^T),}
$$

where $\sigma^{\nabla}=D_t\sigma-\sigma K-K^T\sigma$ in the printed convention. Here $\lambda$ is a [polymer relaxation time](../../../../polymer-relaxation-time.md), unrelated to the inverse-length parameter of question [c](../../1/c.md); $\mu$ is the [polymer viscosity](../../../../dynamic-viscosity-split.md) scale. The coefficient $\alpha$ has inverse-stress units. In the [dimensional mobility parameter in the Giesekus model](../../../../dimensional-mobility-parameter-in-the-giesekus-model.md), the dimensionless factor is $b=\alpha p_T$, not the dimensional $\alpha$ printed in this problem.

The [upper-convected rate](../../../../upper-convected-derivative.md) removes the affine [stretching](../../../../conformation-tensor.md) and [rotation of material connectors](../../../../rotation-mathematics.md). If $\dot F=GF$, then a [tensor](../../../../tensor.md) transported purely as $C=FC_0F^T$ has $C^{\nabla}=0$. Under a time-dependent [rigid rotation](../../../../rotation-mathematics.md) $Q$, the [rate transforms](../../../../objective-time-derivative.md) as $Q C^{\nabla}Q^T$: this is [material frame indifference](../../../../material-frame-indifference.md), not an ordinary componentwise time derivative. The resulting equation is the [Giesekus model](../../../../giesekus-model.md) in these dimensional conventions.

The [isotropic subtraction](../../../../isotropic-tensor.md) is fixed by **zero [polymer extra stress](../../../../stress.md) at [thermal equilibrium](../../../../thermal-equilibrium-split.md)**. With no flow and [positive mobility](../../../../hydrodynamic-mobility-matrix.md), the [stationary distribution](../../../../stationary-distribution.md) is

$$
\psi_{\rm eq}=\left(\frac{H}{2\pi k_BT}\right)^{3/2}
\exp\left(-\frac{H R^2}{2k_BT}\right),\qquad
C_{\rm eq}=\frac{k_BT}{H}I,
$$

so $\boxed{\sigma_{\rm eq}=0}$. The [constitutive equation](../../../../constitutive-equation.md) correspondingly has a zero-stress quiescent state and a [Newtonian low-rate limit](../../../../newtonian-fluid.md) $\sigma\simeq\mu(K+K^T)$. Without subtracting exactly $p_TI$, the spring contribution would retain an equilibrium [isotropic stress](../../../../isotropic-tensor.md) and the equation would acquire corresponding reference terms. Because [mobility](../../../../hydrodynamic-mobility-matrix.md) itself depends on $\sigma$, that reference cannot simply be shifted while retaining the same model. The separate [fluid pressure](../../../../pressure-split.md) enforcing [incompressibility](../../../../incompressible-flow.md) is not included in this [polymer extra stress](../../../../stress.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
