# Deviatoric eddy-viscosity closure

↑ **Parent:** [Eddy viscosity](eddy-viscosity.md)

For an incompressible mean flow, an [eddy viscosity](eddy-viscosity.md) can model the non-isotropic part of the [Reynolds stress](reynolds-stress.md) through the [strain-rate tensor](strain-rate-tensor.md) $S_{ij}=(U_{i,j}+U_{j,i})/2$. The isotropic part is fixed separately by the [turbulent kinetic energy](turbulent-kinetic-energy.md) $e_t=\overline{u_k'u_k'}/2$ in $d$ fluctuating dimensions. Taking the [trace](matrix-trace.md) proves that the isotropic term is necessary: $S_{ii}=0$, whereas $-\rho\overline{u_i'u_i'}=-2\rho e_t$. In the mean momentum equation the isotropic term can be absorbed into $P_{\mathrm{eff}}=P+2\rho e_t/d$.

## ↑ Ancestors (7)

1. [Eddy viscosity](eddy-viscosity.md)
2. [Reynolds stress](reynolds-stress.md)
3. [Turbulence](turbulence-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-topics-in-fluid-mechanics-course-of-the-university-of-oxford/2023/3/a/iii/solution.md)
