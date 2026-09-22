<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Introduce water [dynamic viscosity](../../../../../dynamic-viscosity.md) $\mu$ and the net driving liquid-pressure difference $\Delta P=p_0-p_f>0$. If $p_c>0$ denotes capillary suction relative to an ambient gas pressure $p_a$, then $p_f=p_a-p_c$ and $\Delta P=p_0-p_a+p_c$. If $p_c$ is instead the prescribed liquid front pressure, use $\Delta P=p_0-p_c$. This makes the capillary sign convention explicit.

**Hemispherical front and injection flux.** A hemispherical surface at radius $r$ has area $2\pi r^2$. Quasi-steady [mass conservation](../../../../../mass-conservation.md) makes the total [volume flux](../../../../../volumetric-flow-rate.md) independent of $r$ in the saturated region, so [Darcy's law](../../../../../darcy-law.md) gives

$$
u_r(r)=\frac{Q(t)}{2\pi r^2}=-\frac{k}{\mu}p_r,
\qquad
\Delta P=\frac{\mu Q}{2\pi k}\left(\frac1{R_s}-\frac1R\right).
$$

The changing pore volume is $2\pi\phi(R^3-R_s^3)/3$, giving $Q=2\pi\phi R^2\dot R$. Hence

$$
\boxed{Q(R)=\frac{2\pi k\Delta P R_s}{\mu}\frac{R}{R-R_s},\qquad
\dot R=\frac{k\Delta P R_s}{\mu\phi R(R-R_s)}.}
$$

For the initially dry idealization $R(0)=R_s$, integration gives the implicit front law

$$
\boxed{t=\frac{\mu\phi}{k\Delta P R_s}
\left(\frac{R^3}{3}-\frac{R_sR^2}{2}+\frac{R_s^3}{6}\right),\qquad R\geq R_s.}
$$

Its right-hand side increases for $R>R_s$, defining one advancing radius and thus the flux implicitly in time. Equivalently, with $r=R/R_s$ and $t_*=\mu\phi R_s^2/(k\Delta P)$, $t/t_*=r^3/3-r^2/2+1/6$. The infinite initial flux is an idealization of zero wetted resistance; inertia, finite inlet geometry and pore-scale effects regularize its earliest stage.

For a thin wetted shell $\ell=R-R_s\ll R_s$, the law reduces to

$$
\ell\sim\left(\frac{2k\Delta P t}{\mu\phi}\right)^{1/2},\qquad
Q\sim2\pi R_s^2\left(\frac{k\Delta P\phi}{2\mu t}\right)^{1/2}.
$$

For $R\gg R_s$, the [hemispherical capillary imbibition](../../../../../hemispherical-capillary-imbibition.md) model instead predicts

$$
\boxed{R\sim\left(\frac{3k\Delta P R_st}{\mu\phi}\right)^{1/3},\qquad
Q\longrightarrow Q_\infty=\frac{2\pi k\Delta P R_s}{\mu},}
$$

with $Q/Q_\infty=1+R_s/R+O((R_s/R)^2)$. Radial spreading makes the hydraulic resistance approach a finite value, while the increasing front area reduces its advance speed.

**Comparison with one-dimensional imbibition.** Under the same constant-driving-pressure, negligible-gravity assumptions, a planar front at depth $z$ has Darcy flux $q=k\Delta P/(\mu z)$ and storage law $\phi\dot z=q$. Therefore

$$
\boxed{z\sim\left(\frac{2k\Delta P t}{\mu\phi}\right)^{1/2},\qquad
q\sim\left(\frac{k\Delta P\phi}{2\mu t}\right)^{1/2}.}
$$

A fixed-area one-dimensional flux decays as $t^{-1/2}$, whereas the hemispherical total flux tends to a constant and its radius grows as $t^{1/3}$. If purely vertical imbibition includes gravity, upward penetration eventually approaches a capillary-rise height and downward penetration has a different gravity-driven limit. The hemispherical assumption itself neglects that directional gravity effect, so the power-law comparison is within its capillary-dominated regime.

**Evaporation-limited steady radius.** Take $F_e$ as volumetric water loss per unit front area per unit time. At equilibrium the incoming flux equals $2\pi R^2F_e$, giving

$$
R(R-R_s)=\frac{k\Delta P R_s}{\mu F_e},\qquad
\boxed{R_* =\frac{R_s+\sqrt{R_s^2+4k\Delta P R_s/(\mu F_e)}}2.}
$$

If the stated loss is a [mass flux](../../../../../mass-flux.md), replace $F_e$ by $F_e/\rho_w$. Porosity cancels from this equilibrium but affects the time to approach it. The incoming flux decreases with $R$ while the evaporating area increases, so the equilibrium is stable in this model. As $F_e\to0$, $R_*\sim[k\Delta P R_s/(\mu F_e)]^{1/2}$; sufficiently large radii can invalidate the negligible-gravity or semi-infinite homogeneous-medium assumptions.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
