<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [Faraday's law](../../../../../faraday-s-law-of-induction.md) $\partial_t\mathbf B=-\nabla\times\mathbf E$ and the [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md) $\nabla\cdot\mathbf B=0$. In the nonrelativistic, single-fluid approximation, neglect Hall and other nonideal electromotive terms and use the moving-conductor [moving-conductor Ohm law](../../../../../moving-conductor-ohm-law.md), $\mathbf E+\mathbf u\times\mathbf B=\mathbf J/\sigma$. Infinite [electrical conductivity](../../../../../electrical-conductivity.md) with finite current gives $\mathbf E=-\mathbf u\times\mathbf B$, hence

$$
\boxed{\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B).}
$$

This is the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md). For comparison, neglecting [displacement current](../../../../../displacement-current.md) in [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) gives $\mathbf J=\nabla\times\mathbf B/\mu_0$; with uniform finite [electrical conductivity](../../../../../electrical-conductivity.md) it produces [magnetic diffusion](../../../../../magnetic-diffusion.md) $\eta_m\nabla^2\mathbf B$, where the [magnetic diffusivity](../../../../../magnetic-diffusivity.md) is $\eta_m=1/(\mu_0\sigma)$. The ideal approximation requires a large [magnetic Reynolds number](../../../../../magnetic-reynolds-number.md) $UL/\eta_m$. Dropping displacement current is useful for this finite-conductivity comparison, but Faraday's law and the ideal Ohm relation already suffice for the ideal induction equation.

Expanding the curl and using the [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md) gives the [material derivative](../../../../../material-derivative.md) form

$$
\frac{D\mathbf B}{Dt}=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\nabla\cdot\mathbf u.
$$

Combine this with [mass conservation](../../../../../mass-conservation.md), $D\rho/Dt=-\rho\nabla\cdot\mathbf u$, to obtain

$$
\boxed{\frac D{Dt}\left(\frac{\mathbf B}{\rho}\right)=\left(\frac{\mathbf B}{\rho}\cdot\nabla\right)\mathbf u.}
$$

Now parametrize a [material curve](../../../../../material-curve.md) by a fixed label $a$: $\mathbf X(a,t)$ obeys $\partial_t\mathbf X=\mathbf u(\mathbf X,t)$. Differentiating with respect to $a$ shows that its tangent $\boldsymbol\ell=\partial_a\mathbf X$ evolves by $D\boldsymbol\ell/Dt=(\boldsymbol\ell\cdot\nabla)\mathbf u$. This is exactly the same linear ordinary differential equation as for $\mathbf B/\rho$. Initially parallel tangents remain parallel by uniqueness, with a label-dependent proportionality factor constant along each particle trajectory. Thus **[magnetic field lines](../../../../../magnetic-field-line.md) are transported as [material curves](../../../../../material-curve.md)**, wherever the field and fluid flow are smooth and the field is nonzero. This is the field-line form of [magnetic flux freezing](../../../../../magnetic-flux-freezing.md).

For the flux statement, take a [material surface](../../../../../material-surface.md) $\mathbf X(a,b,t)$ and let $\mathbf t_a=\partial_a\mathbf X$, $\mathbf t_b=\partial_b\mathbf X$. Both tangents obey $D t_i/Dt=(\partial_j u_i)t_j$. Its oriented [material surface element](../../../../../material-surface-element.md) is $\mathbf A=\mathbf t_a\times\mathbf t_b\,da\,db$. Differentiating the cross product, rather than assuming its transport rule, gives

$$
\frac{DA_i}{Dt}=\varepsilon_{ijk}\big[(\partial_\ell u_j)t_{a\ell}t_{bk}+t_{aj}(\partial_\ell u_k)t_{b\ell}\big]da\,db
=(\partial_j u_j)A_i-(\partial_i u_j)A_j.
$$

Equivalently, $D\mathbf A/Dt=(\nabla\cdot\mathbf u)\mathbf A-(\nabla\mathbf u)^T\mathbf A$, with $(\nabla\mathbf u)_{ij}=\partial_j u_i$. Contracting this derived rule with the induction equation gives a pointwise cancellation:

$$
\frac D{Dt}(\mathbf B\cdot\mathbf A)=\big[(\nabla\mathbf u)\mathbf B-\mathbf B\nabla\cdot\mathbf u\big]\cdot\mathbf A+\mathbf B\cdot\big[(\nabla\cdot\mathbf u)\mathbf A-(\nabla\mathbf u)^T\mathbf A\big]=0.
$$

Integrating over the fixed material labels therefore proves **conservation of flux through an open [material surface](../../../../../material-surface.md)**:

$$
\boxed{\frac d{dt}\int_{S(t)}\mathbf B\cdot d\mathbf S=0.}
$$

The surface need not be closed; its boundary is carried with the fluid. The result follows from material transport, rather than from the zero flux through a closed surface.

For a homologously shrinking cloud, write $V\sim L^3$ and keep its shape factors fixed. Conserved mass gives $\rho\sim M/L^3$; conserved [magnetic flux](../../../../../magnetic-flux.md) gives $B\sim\Phi/L^2$. Thus the gravitational and [magnetic energies](../../../../../magnetic-energy.md) scale as

$$
\boxed{W_g=-C_g\frac{GM^2}{L},\qquad E_B=C_B\frac{\Phi^2}{\mu_0L},}
$$

where $C_g,C_B>0$ are dimensionless geometry factors. Both grow in magnitude as $L^{-1}$, so collapse cannot reduce magnetic support relative to gravity while the [mass-to-flux ratio](../../../../../mass-to-flux-ratio.md) is frozen. With negligible gas [pressure](../../../../../pressure.md), contraction lowers the combined [potential energy](../../../../../potential-energy.md) only when its coefficient of $L^{-1}$ is negative. Consequently **a necessary [critical mass-to-flux ratio](../../../../../critical-mass-to-flux-ratio.md) condition** is

$$
\boxed{\frac M\Phi>\frac{\lambda}{\sqrt{\mu_0G}},\qquad \lambda=\sqrt{C_B/C_g}.}
$$

Here $\Phi$ denotes the magnitude of the conserved threading flux. The numerical coefficient depends on geometry and boundary conditions; the scaling argument does not determine it or make the condition sufficient in the presence of other support.

For [adiabatic pressure support during gravitational collapse](../../../../../adiabatic-pressure-support-during-gravitational-collapse.md), $p\propto\rho^\gamma\propto L^{-3\gamma}$. The pressure-support scale is $pV\propto L^{3-3\gamma}$, so relative to either gravity or [magnetic energy](../../../../../magnetic-energy.md),

$$
\boxed{\frac{pV}{|W_g|}\ \propto\ L^{4-3\gamma}.}
$$

[Pressure](../../../../../pressure.md) becomes more important as $L$ decreases if $\gamma>4/3$, equally important in scaling if $\gamma=4/3$, and less important if $\gamma<4/3$. In particular, a monatomic [perfect gas](../../../../../ideal-gas.md) with $\gamma=5/3$ becomes increasingly [pressure](../../../../../pressure.md) supported. For [isothermal pressure support during gravitational collapse](../../../../../isothermal-pressure-support-during-gravitational-collapse.md), the [isothermal equation of state](../../../../../globally-isothermal-equation-of-state.md) gives $p\propto\rho\propto L^{-3}$, so $pV$ is constant and $pV/|W_g|\propto L$: **isothermal [pressure](../../../../../pressure.md) becomes less important during collapse**. The same comparisons hold against magnetic support because its energy has the same $L^{-1}$ scaling as gravity.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
