<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a constant [porosity](../../../../../porosity.md) $\phi$ and let $v$ denote pore [velocity](../../../../../velocity.md). [Darcy law](../../../../../darcy-law.md) gives the [Darcy velocity](../../../../../darcy-velocity.md) $q=\phi v$. If the [velocity](../../../../../velocity.md) convention has already absorbed [porosity](../../../../../porosity.md), set $\phi=1$ in the following formulas. Assume positive [permeability of a porous medium](../../../../../permeability-of-a-porous-medium.md) throughout the layer, so $k_0>0$ and $k_0+k_1>0$.

$$
v(y)=\frac{\Delta P}{\mu\phi L}\left(k_0+\frac{k_1y}{H}\right),\qquad U=\frac1H\int_0^H v(y)\,dy=\frac{\Delta P}{\mu\phi L}\left(k_0+\frac{k_1}{2}\right).
$$

Here $\mu$ is [dynamic viscosity](../../../../../dynamic-viscosity.md). The [flux-weighted residence time in a porous layer](../../../../../flux-weighted-residence-time-in-a-porous-layer.md) is the pore volume divided by throughput. Equivalently, weighting each streamline's transit time $L/v(y)$ by its inlet flux $v(y)\,dy$ gives

$$
\boxed{\overline\tau_Q=\frac{\mu\phi L^2}{\Delta P(k_0+k_1/2)}=\frac LU}.
$$

This is also the advective travel scale after cross-layer mixing has homogenized the [concentration](../../../../../concentration.md). For [resident-weighted transit time in a layered flow](../../../../../resident-weighted-transit-time-in-a-layered-flow.md), sampling the initial fluid uniformly by resident volume, while suppressing cross-stream exchange, is a different experiment: its mean is

$$
\overline\tau_{\rm resident}=\frac{\mu\phi L^2}{\Delta P k_1}\log\left(\frac{k_0+k_1}{k_0}\right),
$$

with the continuous $k_1=0$ limit $\mu\phi L^2/(\Delta P k_0)$. Specifying the sampling convention avoids confusing the reciprocal of the mean speed with the mean reciprocal speed.

For [Taylor dispersion in a linear porous-layer velocity profile](../../../../../taylor-dispersion-in-a-linear-porous-layer-velocity-profile.md), take isotropic pore-scale [mass diffusivity](../../../../../mass-diffusivity.md) $D_p>0$ and reflecting boundaries at $y=0,H$. Write $v-U=\gamma(y-H/2)$, where $\gamma=\Delta P k_1/(\mu\phi LH)$. Let $C(x,t)$ be cross-sectionally averaged [concentration](../../../../../concentration.md) and write the leading transverse correction as $c=C-\chi(y)C_x$. Substitution into [scalar transport](../../../../../scalar-transport.md) $c_t+v c_x=D_p(c_{xx}+c_{yy})$ yields the cell problem

$$
-D_p\chi''=v-U,\quad\chi'(0)=\chi'(H)=0,\quad\langle\chi\rangle=0.
$$

Thus $\chi'=\gamma y(H-y)/(2D_p)$, and averaging the axial solute flux gives $UC-(D_p+D_m)C_x$, with

$$
\boxed{D_m=\langle(v-U)\chi\rangle=D_p\langle(\chi')^2\rangle
=\frac{\gamma^2H^4}{120D_p}
=\frac{(\Delta P k_1)^2H^2}{120\mu^2\phi^2L^2D_p}}.
$$

The [integration by parts](../../../../../integration-by-parts.md) has no boundary term. It also proves nonnegativity, even when $k_1<0$. The total effective [mass diffusivity](../../../../../mass-diffusivity.md) is $\mathcal D=D_p+D_m$. For anisotropic pore dispersion, the denominator uses the transverse coefficient and the added molecular term uses the axial coefficient.

There are two separate tests for significance. The shear [Péclet number](../../../../../peclet-number.md) $\mathrm{Pe}_s=|\gamma|H^2/D_p$ gives $D_m/D_p=\mathrm{Pe}_s^2/120$. A large value implies substantial enhancement of axial spreading. But the [Taylor dispersion](../../../../../taylor-dispersion.md) limit additionally needs

$$
\boxed{\frac LU\gg\frac{H^2}{D_p}}.
$$

Otherwise particles can cross the rock before transverse mixing occurs, and a constant long-time $D_m$ is not an adequate breakthrough model. The relative front width is of order $\sqrt{\mathcal D/(UL)}$ once the long-time model applies.

For a constant tracer input flux, normalize $j_0$ as solute flux per pore cross-sectional area, and use the initially tracer-free half-line model

$$
C_t+UC_x=\mathcal D C_{xx},\quad C(x,0)=0,\quad
UC(0,t)-\mathcal D C_x(0,t)=j_0,\quad C(\infty,t)=0\ \text{for finite }t.
$$

This is a [constant-flux tracer inlet solution](../../../../../constant-flux-tracer-inlet-solution.md); prescribing a flux is distinct from prescribing the inlet [concentration](../../../../../concentration.md). A [Laplace transform](../../../../../laplace-transform.md) in time has decaying spatial root $r=(U-\sqrt{U^2+4\mathcal D p})/(2\mathcal D)$ and gives

$$
\widetilde C(x,p)=\frac{2j_0}{p\left(U+\sqrt{U^2+4\mathcal D p}\right)}e^{rx}.
$$

Define $\xi=UL/\mathcal D$, $\vartheta=U^2t/\mathcal D$, and $z_\pm=(\xi\pm\vartheta)/(2\sqrt\vartheta)$. Inverting, or differentiating the following expression to check the equation and flux boundary condition, gives the requested arrival history:

$$
\boxed{\frac{C(L,t)}{j_0/U}=\frac12\operatorname{erfc}(z_-)
+\sqrt{\frac{\vartheta}{\pi}}e^{-z_-^2}
-\frac12(1+\xi+\vartheta)e^\xi\operatorname{erfc}(z_+)}.
$$

It tends from zero to $j_0/U$. For $UL/\mathcal D\gg1$ near breakthrough, its leading front is

$$
\boxed{C(L,t)\simeq\frac{j_0}{2U}\operatorname{erfc}\left(\frac{L-Ut}{2\sqrt{\mathcal D t}}\right)}.
$$

If a well-stirred inlet instead holds $C(0,t)=C_0=j_0/U$, the exact [constant-concentration inlet solution](../../../../../constant-concentration-inlet-solution.md) is $C(L,t)=\tfrac{C_0}{2}\{\operatorname{erfc}(z_-)+e^\xi\operatorname{erfc}(z_+)\}$. The two inlet models have the same leading advective front, but are not identical at finite axial [Péclet number](../../../../../peclet-number.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
