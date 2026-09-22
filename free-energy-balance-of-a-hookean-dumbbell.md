# Free-energy balance of a Hookean dumbbell

↑ **Parent:** [Hookean dumbbell model](hookean-dumbbell-model.md)

For constant number density $n$, constant [temperature](temperature-split.md), a homogeneous incompressible [linear velocity field](linear-velocity-field.md) and decaying configuration tails, define

$$
\mathcal F=nk_BT\int\psi\log\frac\psi{\psi_{\rm eq}}\,d\mathbf R,\qquad
\mathcal D=\frac{2n}{\zeta}\int\psi|H\mathbf R+k_BT\nabla\log\psi|^2\,d\mathbf R\ge0.
$$

This [free energy](thermodynamic-free-energy.md) is a [relative entropy](kullback-leibler-divergence.md) times $nk_BT$. Differentiate it using the configuration [Fokker-Planck probability current](fokker-planck-probability-current.md). One [integration by parts](integration-by-parts.md) gives $\dot{\mathcal F}=n\int\psi(H\mathbf R+k_BT\nabla\log\psi)\cdot\mathbf V\,d\mathbf R$. Substituting the [probability current velocity](probability-current-velocity.md) gives the displayed balance: the diffusive affine contribution is $-nk_BT\operatorname{tr}K=0$. The polymer [stress tensor](cauchy-stress-tensor.md) $\sigma_p=n(HC-k_BTI)$ has mechanical power $\sigma_p:K=nHC:K$. Its instantaneous power need not be nonnegative, because it includes changes of stored [free energy](thermodynamic-free-energy.md). The nonnegative quantity is $\mathcal D$, and equality of stress power and dissipation requires a stationary [free energy](thermodynamic-free-energy.md).

## ↑ Ancestors (4)

1. [Hookean dumbbell model](hookean-dumbbell-model.md)
2. [Polymer](polymer-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2024/2/d/solution.md)
- [Thermal bead drag and heat-bath power](thermal-bead-drag-and-heat-bath-power.md)
