<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The claimed equality does not hold for the printed joint distribution.** The original PDF specifies a centered [Maxwell-Boltzmann distribution](../../../../maxwell-boltzmann-distribution.md) of $\mathbf v=\dot{\mathbf R}$ independent of $\mathbf R$, with

$$
\langle v_i\rangle=0,\qquad\langle v_iv_j\rangle=\frac{2k_BT}{m}\delta_{ij}.
$$

Since the double average includes number density $n$, evaluating the [Gaussian integrals](../../../../gaussian-integral.md) gives

$$
\boxed{\left\langle\!\left\langle\frac\zeta2|\mathbf v-K\mathbf R|^2\right\rangle\!\right\rangle
=\frac{3n\zeta k_BT}{m}+\frac{n\zeta}{2}\operatorname{tr}(KCK^T).}
$$

The cross term vanishes because the conditional mean of $\mathbf v$ is zero. In particular, set $K=0$ and take the equilibrium configuration [probability density](../../../../probability-density.md) $\psi_{\rm eq}\propto e^{-HR^2/(2k_BT)}$. The left side is $3n\zeta k_BT/m>0$, while $nHC:K=0$. This is a counterexample even at thermal equilibrium, so no rearrangement of the earlier [conformation tensor](../../../../conformation-tensor.md) equation can prove the printed statement.

The discrepancy is [thermal bead drag and heat-bath power](../../../../thermal-bead-drag-and-heat-bath-power.md): gross viscous loss of microscopic thermal motion is replenished by the thermal bath. It is not identical to mechanical polymer stress power. Moreover, $\dot{\mathbf R}$ in the earlier configuration continuity equation is a [probability current velocity](../../../../probability-current-velocity.md), including a distribution-dependent osmotic drift; it cannot simultaneously be identified with an independently sampled centered Maxwellian velocity.

A consistent overdamped result is the [free-energy balance of a Hookean dumbbell](../../../../free-energy-balance-of-a-hookean-dumbbell.md). Define $\mathbf q=H\mathbf R+k_BT\nabla_{\mathbf R}\log\psi$ and

$$
\mathcal F=nk_BT\int\psi\log\frac\psi{\psi_{\rm eq}}\,d\mathbf R,\qquad
\mathbf V=K\mathbf R-\frac2\zeta\mathbf q.
$$

Differentiate the [relative entropy](../../../../kullback-leibler-divergence.md) and use the configuration [Fokker-Planck probability current](../../../../fokker-planck-probability-current.md) $\psi\mathbf V$. After [integration by parts](../../../../integration-by-parts.md),

$$
\dot{\mathcal F}=n\int\psi\,\mathbf q\cdot\mathbf V\,d\mathbf R
=nHC:K-\frac{2n}{\zeta}\int\psi|\mathbf q|^2\,d\mathbf R.
$$

The affine osmotic term is $nk_BT\int\nabla\psi\cdot K\mathbf R\,d\mathbf R=-nk_BT\operatorname{tr}K=0$. Hence

$$
\boxed{nHC:K=\dot{\mathcal F}+\mathcal D,\qquad\mathcal D=\frac{2n}{\zeta}\int\psi|\mathbf q|^2\,d\mathbf R\ge0.}
$$

The polymer [stress tensor](../../../../cauchy-stress-tensor.md) $\sigma_p=n(HC-k_BTI)$ has $\sigma_p:K=nHC:K$ in an [incompressible flow](../../../../incompressible-flow.md). It stores or releases [free energy](../../../../thermodynamic-free-energy.md) as well as dissipating it, so the total stress-work term in part [a](../a.md) need not itself be a purely dissipative quantity for this [viscoelastic](../../../../viscoelasticity.md) material. Stress power equals $\mathcal D$ only for stationary [free energy](../../../../thermodynamic-free-energy.md), and $\mathcal D$ uses the probability-current slip. Neither condition turns the printed independent-Maxwellian average into that expression.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
