<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

Use signature $(+---)$ and local inertial coordinates $x^0=ct$. Write $u^\mu=\gamma(c,\mathbf v)$ and $w=\rho c^2+p$, where $\rho$ is rest [mass density](../../../../density.md). The [perfect fluid in general relativity](../../../../perfect-fluid-in-general-relativity.md) has components

$$
T^{00}=w\gamma^2-p,\qquad T^{0i}=T^{i0}=\frac{w\gamma^2v_i}{c},\qquad
T^{ij}=\frac{w\gamma^2v_iv_j}{c^2}+p\delta_{ij}.
$$

Here $T^{00}$ is [energy density](../../../../energy-density.md), $cT^{i0}$ is [energy flux](../../../../energy-flux.md), $T^{0i}/c$ is [momentum density](../../../../momentum-density.md), and $T^{ij}$ is the flux of the $j$th [momentum](../../../../momentum-split.md) component through a surface normal to $i$. In the local rest frame these reduce to [energy density](../../../../energy-density.md) $\rho c^2$, zero energy and momentum flow, and isotropic [pressure](../../../../pressure-split.md) $p$. The equation $\nabla_\mu T^{\mu\nu}=0$ expresses local [stress-energy conservation](../../../../stress-energy-conservation.md). Its temporal and spatial components give energy and momentum balance; in flat coordinates, for example, $\partial_tT^{00}+\partial_i(cT^{i0})=0$.

For [relativistic dust](../../../../relativistic-dust.md), $T^{\mu\nu}=\rho u^\mu u^\nu$. Contracting its divergence with $u_\nu$, and using [metric compatibility](../../../../metric-compatibility.md) together with $u_\nu u^\nu=c^2$, gives

$$
0=u_\nu\nabla_\mu(\rho u^\mu u^\nu)
=c^2\nabla_\mu(\rho u^\mu)+\frac\rho2u^\mu\nabla_\mu(u_\nu u^\nu)
=c^2\nabla_\mu(\rho u^\mu).
$$

Consequently $\nabla_\mu(\rho u^\mu)=0$. Substituting this continuity equation back into the divergence leaves $\rho u^\mu\nabla_\mu u^\nu=0$. Wherever matter is present,

$$
\boxed{u^\mu\nabla_\mu u^\nu=0,}
$$

so the individual particles follow [geodesics](../../../../geodesic.md).

The electromagnetic [four-force](../../../../four-force.md) law $f^\mu=qF^{\mu\nu}u_\nu$ must preserve the particle's [rest mass](../../../../invariant-mass.md). Thus $u_\mu f^\mu=0$, and requiring this for arbitrary timelike [four-velocities](../../../../four-velocity.md) makes the [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) antisymmetric. Its six independent components comprise the [electric field](../../../../electric-field-split.md) and [magnetic field](../../../../magnetic-field-split.md). With the stated signature and $x^0=ct$, one consistent convention is

$$
F^{i0}=E_i/c,\qquad F^{0i}=-E_i/c,\qquad F^{ij}=-\epsilon_{ijk}B_k.
$$

It gives the spatial force $d\mathbf p/dt=q(\mathbf E+\mathbf v\times\mathbf B)$ and energy transfer $dE/dt=q\mathbf E\cdot\mathbf v$. Under a [Lorentz transformation](../../../../lorentz-transformation.md), $F^{\mu\nu}$ transforms as a rank-two [contravariant tensor](../../../../contravariant-tensor.md); its electric and magnetic components consequently mix. A four-potential supplies $F_{\mu\nu}=\nabla_\mu A_\nu-\nabla_\nu A_\mu$, unchanged by $A_\mu\mapsto A_\mu+\nabla_\mu\chi$. The [Maxwell equations](../../../../maxwell-equations-split.md) are

$$
\nabla_\mu F^{\mu\nu}=\mu_0j^\nu,\qquad
\nabla_\alpha F_{\beta\gamma}+\nabla_\beta F_{\gamma\alpha}+\nabla_\gamma F_{\alpha\beta}=0.
$$

These combine the source equations and the homogeneous equations into covariant tensor statements; $j^\mu$ is the [four-current](../../../../four-current.md).

For [charged relativistic dust](../../../../charged-relativistic-dust.md), the matter tensor exchanges [four-momentum](../../../../four-momentum.md) with the electromagnetic field: $\nabla_\mu T_{\rm m}^{\mu\nu}=F^{\nu\alpha}j_\alpha$, while their total [stress-energy tensor](../../../../stress-energy-tensor-split.md) is conserved. Identical particles of [rest mass](../../../../invariant-mass.md) $m$ and [electric charge](../../../../electric-charge-split.md) $q$ have $j^\alpha=(q/m)\rho u^\alpha$. Contraction with $u_\nu$ again gives mass continuity because $u_\nu F^{\nu\alpha}u_\alpha=0$. Removing that term gives

$$
\boxed{u^\mu\nabla_\mu u^\nu=\frac qmF^{\nu\alpha}u_\alpha.}
$$

Using zero divergence for the matter tensor alone in this last step would omit the electromagnetic [Lorentz force](../../../../lorentz-force.md).

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
