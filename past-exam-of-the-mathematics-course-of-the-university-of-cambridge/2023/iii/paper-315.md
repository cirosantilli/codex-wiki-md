# Paper 315

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_315.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_315.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Treat the morning and evening halves of the [day-night terminator](../../../exoplanet.md#day-night-terminator) as independent, isothermal, hydrostatic atmospheres with the same reference radius $R_0$, reference pressure $P_0$, composition, gravity $g$, and extinction coefficient $\kappa_\lambda$. Their [atmospheric scale heights](../../../exoplanet.md#atmospheric-scale-height) are

$$
H_m=\frac{k_BT_m}{\mu m_Hg},
\qquad
H_e=\frac{k_BT_e}{\mu m_Hg}.
$$

For $H_i\ll R_0$, the slant [optical depth](../../../astrophysics.md#optical-depth) of half $i$ at tangent altitude $z$ is approximately

$$
\tau_{\lambda,i}(z)
=\frac{\kappa_\lambda P_0}{g}
\sqrt{\frac{2\pi R_0}{H_i}}e^{-z/H_i}.
$$

The standard isothermal effective altitude is therefore

$$
z_{\lambda,i}=H_i\left[
\gamma_E+log\left(
\frac{\kappa_\lambda P_0}{g}
\sqrt{\frac{2\pi R_0}{H_i}}
\right)
\right],
$$

up to a wavelength-independent choice of reference radius. The two semicircular limbs add in projected area, so the [exoplanet transmission spectrum](../../../exoplanet.md#exoplanet-transmission-spectrum) is

$$
\boxed{
D_\lambda
=\frac{(R_0+z_{\lambda,m})^2+(R_0+z_{\lambda,e})^2}
{2R_*^2}}.
$$

Equivalently, $R_{\rm tr}^2=[(R_0+z_m)^2+(R_0+z_e)^2]/2$. Differentiating with respect to $\log\kappa_\lambda$ gives

$$
\frac{dR_{\rm tr}}{d\log\kappa_\lambda}
=\frac{(R_0+z_m)H_m+(R_0+z_e)H_e}{2R_{\rm tr}}
\simeq\frac{H_m+H_e}{2}.
$$

Thus a homogeneous retrieval measures, to leading order,

$$
\boxed{H_{\rm av}=\frac{k_B(T_m+T_e)}{2\mu m_Hg}},
$$

provided the opacity and composition do not themselves differ between the two limbs.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Along a ray, the [radiative transfer equation](../../../astrophysics.md#radiative-transfer-equation) has the [formal solution of the radiative transfer equation](../../../astrophysics.md#formal-solution-of-the-radiative-transfer-equation)

$$
I_{\nu,i}=I_{\nu,b}e^{-\tau_{\nu,i}/\mu}
+B_\nu(T_i)(1-e^{-\tau_{\nu,i}/\mu})
$$

for each isothermal region in [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium), neglecting scattering. For a self-luminous atmosphere with no incident intensity from below at the relevant photosphere, and in the optically thick limit, $I_{\nu,i}=B_\nu(T_i)$.

The observed [radiative flux](../../../astrophysics.md#radiative-flux) is the projected-disc integral

$$
F_{\nu,p}=\frac{2\pi R_p^2}{d^2}
\int_0^{\pi/2}I_\nu(\theta)\cos\theta\sin\theta\,d\theta.
$$

The inner region occupies projected fraction $f=\sin^2\theta_T$, hence

$$
\boxed{
F_{\nu,p}=\frac{\pi R_p^2}{d^2}
\left[
B_\nu(T_1)\sin^2\theta_T
+B_\nu(T_2)\cos^2\theta_T
\right]}.
$$

For finite optical depths, each [Planck law](../../../statistical-physics.md#planck-s-law) function in this formula is replaced by its corresponding emergent intensity above.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

A homogeneous interpretation assigns the planet a [brightness temperature](../../../exoplanet.md#brightness-temperature) $T_b$ satisfying

$$
\boxed{
B_\nu(T_b)=fB_\nu(T_1)+(1-f)B_\nu(T_2),
\qquad f=\sin^2\theta_T}.
$$

At a fixed wavelength let $x=hc/(\lambda k_B)$ and

$$
S=\frac{f}{e^{x/T_1}-1}
+\frac{1-f}{e^{x/T_2}-1}.
$$

Inverting the [Planck law](../../../statistical-physics.md#planck-s-law) gives

$$
\boxed{T_b=\frac{x}{\log(1+S^{-1})}}.
$$

At $\lambda=20\,\mu{\rm m}$, $x=719.4\,{\rm K}$. With $\theta_T=\pi/4$, $T_1=1500\,{\rm K}$, and $T_2=1000\,{\rm K}$, one obtains

$$
\boxed{T_b\simeq1251\,{\rm K}}.
$$

The [Rayleigh-Jeans law](../../../astrophysics.md#rayleigh-jeans-law) would give the nearly identical area-weighted estimate $1250\,{\rm K}$.

## 2

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Assume an [ideal-gas atmosphere](../../../statistical-physics.md#ideal-gas-atmosphere-in-uniform-gravity) of constant mean molecular mass and approximately constant gravity. If temperature decreases linearly with altitude, write $dT/dz=-\Gamma$. Combining the ideal-gas law with [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives

$$
\frac{d\log P}{dz}=-\frac{\mu m_Hg}{k_BT},
\qquad
\frac{d\log P}{d\log T}=\frac{\mu m_Hg}{k_B\Gamma}.
$$

The endpoint conditions determine the power law directly:

$$
\boxed{
T(P)=T_t\left(\frac{P}{P_t}\right)^a
=T_b\left(\frac{P}{P_b}\right)^a,
\qquad
a=\frac{\log(T_b/T_t)}{\log(P_b/P_t)}}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Differentiate the result of part i and use hydrostatic equilibrium:

$$
\frac{dT}{dz}
=aT\frac{d\log P}{dz}
=-\frac{a\mu m_Hg}{k_B}.
$$

Thus the constant [atmospheric lapse rate](../../../exoplanet.md#lapse-rate-atmosphere) is

$$
\boxed{
\Gamma=-\frac{dT}{dz}
=\frac{\mu m_Hg}{k_B}
\frac{\log(T_b/T_t)}{\log(P_b/P_t)}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Apply the [formal solution of the radiative transfer equation](../../../astrophysics.md#formal-solution-of-the-radiative-transfer-equation) successively to the two isothermal layers at normal incidence. In [local thermodynamic equilibrium](../../../astrophysics.md#local-thermodynamic-equilibrium),

$$
\boxed{
I_{\nu,2}=I_{\nu,0}e^{-(\tau_1+\tau_2)}
+B_\nu(T_1)(1-e^{-\tau_1})e^{-\tau_2}
+B_\nu(T_2)(1-e^{-\tau_2})}.
$$

For [optically thin](../../../astrophysics.md#optically-thin-medium) layers this becomes

$$
\boxed{
I_{\nu,2}=I_{\nu,0}
+\tau_1[B_\nu(T_1)-I_{\nu,0}]
+\tau_2[B_\nu(T_2)-I_{\nu,0}]
+O(\tau^2)}.
$$

This assumes no scattering and negligible reflection between layers.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

With $I_{\nu,0}=B_\nu(T_0)$, the sign of each first-order term is set by whether that layer is hotter or colder than the incident blackbody.

- If $T_2<T_1<T_0$, temperature decreases with altitude. Both layers remove intensity, so frequencies of larger optical depth appear in absorption; the colder upper layer gives the strongest absorption when it controls the opacity.
- If $T_2>T_1$ while $T_1<T_0$, the atmosphere has a [temperature inversion](../../../exoplanet.md#inversion-meteorology). The lower layer absorbs, whereas the upper layer partly fills the absorption. If $T_2>T_0$, upper-atmosphere bands appear in emission; if $T_2<T_0$, they remain in absorption but are shallower.
- If $T_2>T_1>T_0$, both layers add intensity and spectral bands appear in emission, with the hotter upper layer producing the largest contrast.

The corresponding temperature profiles, from bottom to top, are respectively monotone decreasing, decreasing then increasing, and increasing throughout.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Optical depth increases inward, so an [atmospheric thermal inversion](../../../exoplanet.md#inversion-meteorology) occurs where temperature decreases with $\tau$. Differentiation gives

$$
4T^3\frac{dT}{d\tau}=B-\beta Ce^{-\beta\tau}.
$$

Therefore the inversion condition in the observable atmosphere is

$$
\boxed{\beta Ce^{-\beta\tau}>B}.
$$

In particular, an inversion reaches the top when $\beta C>B$. A hot Jupiter can satisfy this when visible absorbers such as atomic metals, metal oxides, or negative hydrogen absorb incident starlight above the infrared photosphere. This makes the shortwave opacity large relative to the thermal opacity and deposits heat at low pressure.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Convection begins when the [radiative temperature gradient](../../../exoplanet.md#radiative-temperature-gradient) equals the [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient) $\nabla_{\rm ad}$. To convert optical depth into pressure, assume a pressure-law opacity $\kappa=\kappa_0P^n$ and constant gravity. Hydrostatic balance gives

$$
\tau(P)=\frac{\kappa_0P^{n+1}}{(n+1)g},
\qquad
\frac{d\log\tau}{d\log P}=n+1.
$$

Hence

$$
\nabla_{\rm rad}
=\frac{d\log T}{d\log P}
=\frac{(n+1)\tau[B-\beta Ce^{-\beta\tau}]}
{4[A+B\tau+Ce^{-\beta\tau}]}.
$$

The exact [radiative-convective boundary](../../../exoplanet.md#radiative-convective-boundary) is the positive solution of

$$
\boxed{
\frac{(n+1)\tau_{\rm rc}[B-\beta Ce^{-\beta\tau_{\rm rc}}]}
{4[A+B\tau_{\rm rc}+Ce^{-\beta\tau_{\rm rc}}]}
=\nabla_{\rm ad},
\qquad
P_{\rm rc}=\left[
\frac{(n+1)g\tau_{\rm rc}}{\kappa_0}
\right]^{1/(n+1)}}.
$$

Deep enough that the exponential term is negligible,

$$
\tau_{\rm rc}\simeq
\frac{4\nabla_{\rm ad}A}
{B(n+1-4\nabla_{\rm ad})},
$$

which requires $n+1>4\nabla_{\rm ad}$. This exposes why constant opacity is inadequate for a molecular atmosphere: its limiting radiative gradient is $1/4$, below $\nabla_{\rm ad}\simeq2/7$.

In a grey scaling, $A\sim T_{\rm eq}^4$ measures irradiation and $B\sim T_{\rm int}^4$ measures intrinsic flux. Thus

$$
P_{\rm rc}\propto(A/B)^{1/(n+1)}.
$$

For a hot Jupiter with $T_{\rm eq}\sim1500\,{\rm K}$ and $T_{\rm int}\sim100\,{\rm K}$, irradiation pushes the boundary to hundreds of bars for typical increasing opacity. Jupiter has $T_{\rm eq}$ and $T_{\rm int}$ both of order $10^2\,{\rm K}$ and becomes convective near the bar scale. The estimate is order-of-magnitude because real opacities depend on both pressure and temperature.

## 3

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Let

$$
A=\rho_c+\rho_m,
\qquad
b=\frac{\rho_m}{R_c},
\qquad
d=\frac{\rho_mR_c^3}{12}.
$$

The [enclosed mass](../../../stellar-structure.md#enclosed-mass) is

$$
m(r)=
\begin{cases}
\dfrac{4\pi}{3}\rho_cr^3,&0\leq r\leq R_c,\\
4\pi\left(\dfrac{Ar^3}{3}-\dfrac{br^4}{4}-d\right),&R_c\leq r\leq R_p.
\end{cases}
$$

This is continuous at the core boundary. [Hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives $dP/dr=-Gm(r)\rho(r)/r^2$, with $P(R_p)=0$. Define

$$
F(r)=4\pi G\left(
\frac{A^2r^2}{6}
-\frac{7Abr^3}{36}
+\frac{b^2r^4}{16}
+bd\log(r/R_c)
+\frac{Ad}{r}
\right).
$$

Since $F'(r)=Gm(r)(A-br)/r^2$, the mantle pressure is

$$
\boxed{P(r)=F(R_p)-F(r),
\qquad R_c\leq r\leq R_p}.
$$

Inside the uniform core, the [shell theorem](../../../physics.md#spherical-shell-theorem) gives $m(r)=4\pi\rho_cr^3/3$, so

$$
\boxed{
P(r)=F(R_p)-F(R_c)
+\frac{2\pi G\rho_c^2}{3}(R_c^2-r^2),
\qquad 0\leq r\leq R_c}.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The mantle density decreases outward when $\rho_m\geq0$. Requiring a nonnegative surface density gives the immediate physical bound

$$
\boxed{0\leq\rho_m\leq\frac{\rho_cR_c}{R_p-R_c}}.
$$

The measured planetary mass also fixes

$$
M_p=4\pi\left[
\frac{(\rho_c+\rho_m)R_p^3}{3}
-\frac{\rho_mR_p^4}{4R_c}
-\frac{\rho_mR_c^3}{12}
\right].
$$

Equivalently,

$$
\rho_m=
\frac{\rho_cR_p^3/3-M_p/(4\pi)}
{R_p^4/(4R_c)-R_p^3/3+R_c^3/12},
$$

and a viable model requires this value to obey the boxed bound.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Assume a thin [isothermal atmosphere](../../../statistical-physics.md#isothermal-atmosphere), so $g\simeq GM_p/R_p^2$ and the surface area are constant through it. Integrating [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) from base pressure $P_0$ to negligible top pressure gives atmospheric column mass $P_0/g$. Therefore

$$
\boxed{
M_{\rm atm}\simeq4\pi R_p^2\frac{P_0}{g}
=\frac{4\pi P_0R_p^4}{GM_p}}.
$$

Equivalently, $M_{\rm atm}\sim4\pi R_p^2\rho_0H$, with $\rho_0=P_0\mu m_H/(k_BT_0)$ and $H=k_BT_0/(\mu m_Hg)$; the explicit temperature dependence cancels.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The location between pure-silicate and pure-water [planetary mass-radius curves](../../../exoplanet.md#planetary-mass-radius-relation) does not determine a unique composition. Possibilities include a rocky iron-silicate interior with a deep water layer, a rock-water mixture, or a mostly rocky planet whose small hydrogen-helium envelope inflates its radius. The atmosphere could accordingly be hydrogen-helium, steam-rich, carbon-dioxide-rich, or secondary gas released from the interior. Residence in the [circumstellar habitable zone](../../../exoplanet.md#circumstellar-habitable-zone) constrains stellar flux but does not by itself distinguish these models or guarantee surface liquid water.

For an atmosphere spanning fixed base and photospheric pressures,

$$
\Delta R\simeq H\log(P_0/P_{\rm ph}),
\qquad
H=\frac{k_BT}{\mu m_Hg}.
$$

Thus two compositions have

$$
\boxed{
\frac{\Delta R_1}{\Delta R_2}
\simeq\frac{T_1/\mu_1}{T_2/\mu_2}}.
$$

At equal temperature, a hydrogen-helium atmosphere with $\mu\simeq2.3$ is about

$$
\boxed{\frac{18}{2.3}\simeq7.8}
$$

times thicker than a steam atmosphere with $\mu\simeq18$. This large difference is one reason atmospheric composition contributes strongly to the [exoplanet interior-composition degeneracy](../../../exoplanet.md#exoplanet-interior-composition-degeneracy).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The stellar flux at the orbit is

$$
F_*=\sigma T_s^4\left(\frac{R_s}{a}\right)^2.
$$

Let $\epsilon$ be the fraction of the planet's total absorbed power transported to the night side, and let $A_B$ be its [Bond albedo](../../../exoplanet.md#bond-albedo). Equating transported power to nightside blackbody emission gives

$$
2\pi R_p^2\sigma T_n^4
=\epsilon\pi R_p^2(1-A_B)F_*.
$$

Hence the [nightside equilibrium temperature](../../../exoplanet.md#nightside-equilibrium-temperature) is

$$
\boxed{
T_n=T_s\sqrt{\frac{R_s}{a}}
\left[\frac{\epsilon(1-A_B)}2\right]^{1/4}}.
$$

Perfect global [day-night heat redistribution](../../../exoplanet.md#day-night-heat-redistribution) has $\epsilon=1/2$ and gives $T_n=T_s\sqrt{R_s/a}[(1-A_B)/4]^{1/4}$; without redistribution, stellar heating alone gives $T_n=0$ in this idealization. Efficient atmospheric or oceanic transport prevents volatile cold trapping and broadens the habitable region of a tidally locked planet, whereas a thin atmosphere can leave a frozen night side even when the day side is temperate.

## 4

↑ **Parent:** [Paper 315](paper-315.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Specific intensity is defined by $dE=I_\nu\cos\theta\,dA\,d\Omega\,d\nu\,dt$. A ray bundle in free space expands in area while its solid angle contracts by the same factor, so

$$
\boxed{\frac{dI_\nu}{ds}=0}.
$$

Thus [specific intensity](../../../astrophysics.md#specific-intensity) does not obey an inverse-square law; the flux of an unresolved source does because its apparent solid angle scales as distance${}^{-2}$.

For a cold medium with coherent, isotropic, conservative scattering, the source function is the [mean intensity](../../../astrophysics.md#mean-intensity) $J_\nu$. With scattering optical depth increasing along the ray,

$$
\frac{dI_\nu}{d\tau_\nu}=-I_\nu+J_\nu,
$$

and

$$
\boxed{
I_\nu(\tau)=I_\nu(0)e^{-\tau}
+\int_0^\tau J_\nu(t)e^{-(\tau-t)}dt}.
$$

The unscattered pencil beam is attenuated by $e^{-\tau}$ and reappears as a diffuse halo in other directions. Coherent scattering preserves frequency, and conservative scattering preserves total luminosity when all outgoing directions are collected.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $A+B\rightleftharpoons C+D$, the forward and reverse rates are

$$
r_f=k_fn_An_B,
\qquad
r_r=k_rn_Cn_D.
$$

At [thermochemical equilibrium](../../../thermodynamics.md#thermochemical-equilibrium), $r_f=r_r$ by [detailed balance](../../../markov-process.md#detailed-balance), while

$$
K_c=\frac{n_Cn_D}{n_An_B}
=\exp\left(-\frac{\Delta_rG^\circ}{RT}\right)
$$

after the appropriate standard-concentration factors are included. The standard reaction [Gibbs free energy](../../../thermodynamics.md#gibbs-free-energy) is

$$
\Delta_rG^\circ=G_C^\circ+G_D^\circ-G_A^\circ-G_B^\circ.
$$

Consequently

$$
\boxed{k_r=\frac{k_f}{K_c}
=k_f\exp\left(\frac{\Delta_rG^\circ}{RT}\right)}.
$$

For other stoichiometries, the same argument uses the corresponding activity product and its standard-state factors.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Assume uniform global temperatures, all visible light not scattered back to space is absorbed by the surface, and use [Kirchhoff's law of thermal radiation](../../../astrophysics.md#kirchhoff-s-law-of-thermal-radiation) so that the atmospheric infrared emissivity is $\alpha$. If $F_*=\sigma T_*^4(R_*/a)^2$, the globally averaged absorbed stellar flux is

$$
S=\frac{1-\beta}{4}F_*.
$$

The atmosphere absorbs $\alpha\sigma T_{\rm surf}^4$ from the surface and emits from both faces, so

$$
\alpha\sigma T_{\rm surf}^4=2\alpha\sigma T_a^4,
\qquad T_a^4=\frac12T_{\rm surf}^4.
$$

Surface balance is

$$
S+\alpha\sigma T_a^4=\sigma T_{\rm surf}^4.
$$

Therefore the [single-layer greenhouse model](../../../exoplanet.md#single-layer-greenhouse-model) gives

$$
\boxed{
T_{\rm surf}=T_*\sqrt{\frac{R_*}{2a}}
\left(\frac{1-\beta}{1-\alpha/2}\right)^{1/4}}.
$$

Visible scattering cools the surface, whereas infrared absorption and downward re-emission warm it.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

On a [planetary mass-radius relation](../../../exoplanet.md#planetary-mass-radius-relation), compressed rocky planets grow sublinearly, approximately $R\propto M^{0.25-0.3}$. Adding a hydrogen-helium envelope produces a rapid radius increase toward sub-Neptunes and gas giants. Around a few Jupiter masses the radius is nearly constant and then decreases as [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) becomes important, approximately approaching the nonrelativistic degenerate scaling $R\propto M^{-1/3}$.

[Brown dwarfs](../../../stellar-astrophysics.md#brown-dwarf) occupy roughly $13$ to $75$--$80$ Jupiter masses, with deuterium burning near the lower conventional boundary and sustained hydrogen burning beginning at the [hydrogen-burning minimum mass](../../../stellar-astrophysics.md#hydrogen-burning-minimum-mass). Low-mass main-sequence stars then have radii that increase with mass. Thus an isolated-body sketch has a rising rocky branch, a broad giant-planet/brown-dwarf radius maximum and decline, followed by a rising stellar branch.

[Hot-Jupiter radius inflation](../../../exoplanet.md#hot-jupiter-radius-inflation) places strongly irradiated hot Jupiters above the isolated giant-planet sequence. Irradiation retards cooling and contraction; additional proposed contributions include tidal heating, Ohmic dissipation, atmospheric circulation depositing energy at depth, enhanced opacity, and residual youth.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Young giant planets retain high formation entropy and radiate gravitational and thermal energy as they contract. Their infrared self-luminosity, especially at wide angular separation from a young nearby star, made the first [directly imaged exoplanets](../../../exoplanet.md#exoplanet-direct-imaging) much easier to detect than mature reflected-light planets. The inferred brightness depends on whether formation followed a high-entropy hot start or a low-entropy cold start.

By $10^{10}$ years, deuterium burning and most rapid [Kelvin-Helmholtz contraction](../../../stellar-astrophysics.md#kelvin-helmholtz-mechanism) have ended. The intrinsic luminosity is governed mainly by the remaining interior entropy and ionic heat capacity, slow contraction supported by partially degenerate electrons, and the atmospheric opacity that controls escape of heat. Composition-dependent processes such as helium rain can add energy. For an irradiated planet, absorbed and reradiated starlight may dominate the observed luminosity, but it does not equal the planet's intrinsic cooling luminosity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
