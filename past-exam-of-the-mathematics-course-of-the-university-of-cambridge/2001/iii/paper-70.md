# Paper 70

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper70.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper70.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write the [reduced Planck mass](../../../physics.md#reduced-planck-mass) as $M=(8\pi G)^{-1/2}=m_{\rm pl}/\sqrt{8\pi}$, and use natural units. Near the flat maximum, the [quartic hilltop inflation](../../../cosmic-inflation.md#quartic-hilltop-inflation) trajectory has $V\simeq\alpha\sigma^4$ and $V'\simeq-12\alpha\phi^3$. The [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) gives $H^2\simeq V/(3M^2)$ and $3H\dot\phi\simeq-V'$. Therefore the [number of e-folds](../../../cosmic-inflation.md#number-of-e-folds) is

$$
N(\phi)\simeq\frac1{M^2}\int_\phi^{\phi_{\rm upper}}\frac{V}{-V'}d\phi
\simeq\frac{\sigma^4}{24M^2}\left(\frac1{\phi^2}-\frac1{\phi_{\rm upper}^2}\right).
$$

The lower field value dominates this integral. Thus

$$
\boxed{\phi_{50}^2\simeq\frac{\sigma^4}{1200M^2}
=\frac{\pi\sigma^4}{150m_{\rm pl}^2},\qquad
\phi_{50}\simeq0.145\frac{\sigma^2}{m_{\rm pl}}.}
$$

This is far below $\sigma$ for the assumed small symmetry-breaking scale. Strict slow roll actually fails before the minimum: $|M^2V''/V|\sim1$ at $\phi^2\sim\sigma^4/(36M^2)$. The last approach to the minimum is not described by slow roll. Using that earlier upper limit changes the dominant fifty-e-fold estimate by an order-one [number of e-folds](../../../cosmic-inflation.md#number-of-e-folds), not its leading scale dependence. No extrapolation of slow roll all the way to the minimum is needed.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A comoving [wavenumber](../../../wave-equation.md#wavenumber) crosses the inflationary Hubble scale at $k=aH$. Consequently $d\ln k=d\ln a+d\ln H\simeq Hdt$ when $H$ changes slowly. Combining with the [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) gives

$$
\boxed{d\ln k\simeq-\frac{V}{M^2V'}\,d\phi
\simeq\frac{\sigma^4}{12M^2\phi^3}\,d\phi.}
$$

Both $k$ and $\phi$ increase along the rolling branch. If $N$ denotes the remaining [number of e-folds](../../../cosmic-inflation.md#number-of-e-folds) rather than elapsed expansion, then $d\ln k\simeq-dN$. More precisely $d\ln k=(1-\epsilon_H)d\ln a$; the correction is beyond the constant-Hubble approximation used here.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

At leading order the scalar curvature power and total tensor power are

$$
\mathcal P_S=\frac{V}{24\pi^2M^4\epsilon_V},\qquad
\mathcal P_T=\frac{2V}{3\pi^2M^4},\qquad
\epsilon_V=\frac{M^2}{2}\left(\frac{V'}V\right)^2,\quad\eta_V=\frac{M^2V''}{V}.
$$

Applying the preceding $d/d\ln k$ relation gives the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) $n-1=-6\epsilon_V+2\eta_V$ and the [tensor spectral index](../../../cosmic-inflation.md#tensor-spectral-index) $n_T=-2\epsilon_V$. For this hilltop,

$$
\eta_V\simeq-\frac{36M^2\phi^2}{\sigma^4}=-\frac3{2N},\qquad
\epsilon_V\simeq\frac{72M^2\phi^6}{\sigma^8}
=\frac{\sigma^4}{192M^4N^3}.
$$

Thus, fifty e-folds before the end,

$$
\boxed{n\simeq1-\frac3{50}=0.94,\qquad
n_T\simeq-\frac{\sigma^4}{96M^4(50)^3}
=-5.26\times10^{-5}\left(\frac{\sigma}{m_{\rm pl}}\right)^4.}
$$

The tiny $-6\epsilon_V$ contribution and finite-endpoint corrections have been omitted in the quoted leading scalar tilt. The tensor tilt is nearly zero but slightly negative; treating $H$ as exactly constant in its spectrum would incorrectly discard its leading nonzero value.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The given large-angle temperature transfer relation gives the [low-multipole tensor fraction in quartic hilltop inflation](../../../cosmic-inflation.md#low-multipole-tensor-fraction-in-quartic-hilltop-inflation)

$$
\boxed{\frac TS\simeq-7n_T
\simeq3.68\times10^{-4}\left(\frac{\sigma}{m_{\rm pl}}\right)^4\ll10^{-4}.}
$$

This is not the primordial [tensor-to-scalar ratio](../../../cosmic-inflation.md#tensor-to-scalar-ratio) $r=16\epsilon_V$, because the scalar and tensor contributions to low CMB multipoles have different transfer functions. With $\sigma\ll m_{\rm pl}$, the tensor contribution is far below the scalar temperature signal and its [cosmic variance](../../../cosmic-microwave-background-anisotropy.md#cosmic-variance), and the corresponding primordial gravitational-wave or polarization signal is extremely small.

For [COBE normalization of quartic hilltop inflation](../../../cosmic-inflation.md#cobe-normalization-of-quartic-hilltop-inflation), the historical scalar horizon amplitude is of order $\delta_H\simeq2\times10^{-5}$, or $\mathcal P_S\simeq25\delta_H^2/4\sim2.5\times10^{-9}$ in the usual matter-era convention. The slow-roll spectrum simplifies to

$$
\mathcal P_S\simeq\frac{V^3}{12\pi^2M^6V'^2}
\simeq\frac{\alpha\sigma^{12}}{1728\pi^2M^6\phi_{50}^6}
=\frac{8\alpha(50)^3}{\pi^2}.
$$

Hence

$$
\boxed{\alpha\simeq\frac{\pi^2\mathcal P_S}{8(50)^3}\sim2\text{--}3\times10^{-14}.}
$$

Late-time transfer and tilt corrections to the COBE normalization change the order-one coefficient, not the conclusion that the dimensionless coupling must be extraordinarily small. The leading normalization is independent of $\sigma$: reducing the height of the potential also changes the slope and field value at fixed $N$, causing the scale factors to cancel.

## 2

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Normalize $a_0=1$ and use the open dust model, with no [cosmological constant](../../../cosmology.md#cosmological-constant) and negligible present radiation. The [Friedmann equation](../../../cosmology.md#friedmann-equations) at the present epoch reads $H_0^2=H_0^2\Omega_m-kc^2$. Since $k=-r_{\rm curv}^{-2}$, the [curvature radius of an open FLRW universe](../../../cosmology.md#curvature-radius-of-an-open-flrw-universe) is

$$
\boxed{r_{\rm curv}=\frac{c}{H_0\sqrt{1-\Omega_m}}.}
$$

In the metric's $c=1$ convention the numerator is one. With $a_0=1$ this is also the present physical curvature radius; at [scale factor](../../../cosmology.md#scale-factor-cosmology) $a$ the physical radius is $a r_{\rm curv}$. Inferring curvature from $\Omega_m$ alone would require this matter-only assumption; an additional dark-energy density would also enter the present [Friedmann equation](../../../cosmology.md#friedmann-equations).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

At fixed [conformal time](../../../cosmology.md#conformal-time) and fixed radial coordinate, the metric gives transverse physical separation $D=a(\tau_1)r_1\theta$ to first order in the angle. Thus the [angular diameter distance](../../../cosmology.md#angular-diameter-distance) is

$$
\boxed{\theta\simeq\frac{D}{a(\tau_1)r_1},\qquad d_A=a(\tau_1)r_1.}
$$

The coordinate $r_1$ is the transverse comoving radius appearing in the angular metric coefficient. It is not the radial geodesic distance $r_{\rm curv}\operatorname{arsinh}(r_1/r_{\rm curv})$; replacing one by the other would omit the curvature dependence of angular projection.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Adiabatic [photon](../../../quantum-mechanics.md#photon) cooling gives $a_*\simeq1/1200$. During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $H(a)\simeq H_0\sqrt{\Omega_m}a^{-3/2}$, so the comoving sound distance traveled before last scattering is

$$
s_*\simeq\frac{c}{\sqrt3}\int_0^{a_*}\frac{da}{a^2H(a)}
=\frac{2c\sqrt{a_*}}{\sqrt3H_0\sqrt{\Omega_m}}.
$$

Multiplication by $a_*$ gives the physical [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon) radius:

$$
\boxed{R_{s,*}\simeq\frac{2c}{\sqrt3H_0\sqrt{\Omega_m}}(1200)^{-3/2}
\simeq\frac{0.119\,\mathrm{Mpc}}{\sqrt{\Omega_m}}
\left(\frac{70\,\mathrm{km\,s^{-1}\,Mpc^{-1}}}{H_0}\right).}
$$

This is a radius, or one-way sound-propagation length, rather than its diameter. The integral treats the early radiation interval as negligible under the specified late-equality approximation; it also neglects curvature at last scattering, requiring $\Omega_ma_*^{-3}\gg(1-\Omega_m)a_*^{-2}$. A very small matter fraction would violate those approximations.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

A radial null ray obeys $c\,d\tau=dr/\sqrt{1+r^2/r_{\rm curv}^2}$. Hence

$$
c(\tau_0-\tau_*)=r_{\rm curv}\operatorname{arsinh}\frac{r_*}{r_{\rm curv}},\qquad
r_*=r_{\rm curv}\sinh\frac{c(\tau_0-\tau_*)}{r_{\rm curv}}.
$$

For the open matter solution, let $\beta=\sqrt{1-\Omega_m}$. The [Friedmann equation](../../../cosmology.md#friedmann-equations) gives $a'=H_0\sqrt{\Omega_m a+\beta^2a^2}$, and the age in [conformal time](../../../cosmology.md#conformal-time) is

$$
\tau_0=\frac1{H_0}\int_0^1\frac{da}{\sqrt{a(\Omega_m+\beta^2a)}}
=\frac2{H_0\beta}\operatorname{arsinh}\frac{\beta}{\sqrt{\Omega_m}}
=\frac2{H_0\beta}\operatorname{artanh}\beta.
$$

Thus

$$
\boxed{\tau_0=\frac1{H_0\beta}\ln\frac{1+\beta}{1-\beta},\qquad
r_*\simeq\frac{c}{H_0\beta}\sinh(2\operatorname{artanh}\beta)
=\frac{2c}{H_0\Omega_m}.}
$$

Here the stated approximation $\tau_*\ll\tau_0$ was used only in the last distance estimate. The flat limit is smooth: $\tau_0\to2/H_0$ and $r_*\to2c/H_0$. Retaining $\tau_*$ in the preceding null-ray formula gives the finite-emission-time correction.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Divide the physical sound radius by the [angular diameter distance](../../../cosmology.md#angular-diameter-distance) $a_*r_*$. The [sound-horizon angle in an open matter universe](../../../cosmic-microwave-background-anisotropy.md#sound-horizon-angle-in-an-open-matter-universe) is

$$
\boxed{\theta_s\simeq\sqrt{\frac{\Omega_ma_*}{3}}
=\frac{\sqrt{\Omega_m}}{60}\ \mathrm{rad}
\simeq0.955^\circ\sqrt{\Omega_m}.}
$$

The characteristic acoustic multipole is approximately half a wavelength across this angle:

$$
\boxed{\ell_s\sim\frac\pi{\theta_s}\simeq\frac{190}{\sqrt{\Omega_m}}.}
$$

Thus negative curvature moves the acoustic feature to smaller angular scales and larger multipoles. The first temperature peak is of order $200/\sqrt{\Omega_m}$ in this approximation; precise peak positions include the sound-speed history, radiation effects and acoustic phase shifts, so the acoustic-scale multipole is not an exact peak-location formula.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

For instantaneous complete [hydrogen](../../../chemistry.md#hydrogen) [reionization](../../../cosmology.md#reionization), take $n_{e0}=\Omega_b\rho_{{\rm crit},0}/(m_pc^2)=3\Omega_bH_0^2/(8\pi Gm_p)$ and $n_e(z)=n_{e0}(1+z)^3$. Helium or incomplete [ionization](../../../physics.md#ionization) would multiply this by the appropriate free-electron count per baryon. In the matter-plus-curvature model,

$$
H(z)=H_0(1+z)\sqrt{1+\Omega_mz},\qquad
|dt|=\frac{dz}{(1+z)H(z)}.
$$

The [reionization optical depth in an open matter universe](../../../cosmology.md#reionization-optical-depth-in-an-open-matter-universe) is therefore

$$
\kappa=\frac{3\Omega_b\sigma_TcH_0}{8\pi Gm_p}
\int_0^{z_{\rm re}}\frac{1+z}{\sqrt{1+\Omega_mz}}dz.
$$

Set $u=\sqrt{1+\Omega_mz}$ and $\beta^2=1-\Omega_m$. The integral is $2\Omega_m^{-2}[u^3/3-\beta^2u]_1^{u_{\rm re}}$, giving

$$
\boxed{\kappa=\frac{\Omega_b C_H}{\Omega_m^2}
\left[u_{\rm re}^3-1-3(1-\Omega_m)(u_{\rm re}-1)\right],\quad
u_{\rm re}=\sqrt{1+\Omega_mz_{\rm re}},\quad C_H=\frac{\sigma_TcH_0}{4\pi Gm_p}.}
$$

At high redshift where matter dominates over curvature, this approaches $\kappa\simeq\Omega_bC_H(1+z_{\rm re})^{3/2}/\sqrt{\Omega_m}$. The exact expression should be retained when $\Omega_mz_{\rm re}$ is not large.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

For $\Omega_m=1$ the preceding result reduces to $\kappa=\Omega_b C_H[(1+z_{\rm re})^{3/2}-1]$. Using $C_H=0.032$ and $\Omega_b=0.05$ gives

$$
\boxed{z_{\rm re}=(1+625)^{2/3}-1\simeq72.2\qquad(\kappa=1).}
$$

At fixed $H_0$ and $\Omega_b$, a lower matter density lowers $H(z)$ relative to the flat dust value at positive redshift. The same [Electron](../../../physics.md#electron) density then persists for a longer scattering time, increasing the [optical depth](../../../astrophysics.md#optical-depth). Hence the [reionization](../../../cosmology.md#reionization) redshift giving unit depth is lower in an open universe.

In the high-redshift matter regime the scaling is $1+z_{\rm re}\propto\Omega_m^{1/3}$ at fixed [optical depth](../../../astrophysics.md#optical-depth); for $\Omega_m=0.3$ this suggests a redshift near fifty rather than seventy. This comparison holds the baryon density fixed, not the baryon fraction $\Omega_b/\Omega_m$, and is not an estimate of the actual observed [reionization](../../../cosmology.md#reionization) epoch.

## 3

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Choose a vacuum [order parameter](../../../critical-phenomenon.md#order-parameter) $\Phi_0$ and let $H$ be its [stabilizer](../../../group-theory.md#stabilizer-subgroup) in $G$. Acting with $G$ produces all symmetry-related minima; two elements produce the same minimum precisely when they differ by an element of $H$. The [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) is therefore

$$
\boxed{M\simeq G/H.}
$$

This assumes a single transitive orbit of minima; additional independent vacuum sectors would require more than one orbit. For a local [gauge symmetry](../../../relativistic-quantum-field.md#gauge-invariance), $G/H$ describes the vacuum directions used in finite-energy boundary conditions and defect classification, rather than distinct observable vacua after quotienting by every gauge redundancy.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Finite-energy configurations approach the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) outside defect cores. The surrounding boundary in the transverse directions is a sphere, and noncontractible boundary data prevent a smooth deformation to the uniform vacuum.

Nontrivial $\pi_0(M)$ means disconnected vacuum components. Choosing different components on the two sides of an interface produces [domain walls](../../../critical-phenomenon.md#domain-wall). Here $\pi_0$ labels components and need not itself carry a group structure. Nontrivial $\pi_1(M)$ means noncontractible loops: a circle surrounding a line can wind around the [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold), producing [cosmic strings](../../../cosmology.md#cosmic-string). Nontrivial $\pi_2(M)$ means noncontractible maps from an enclosing two-sphere, producing pointlike [magnetic monopoles](../../../physics.md#magnetic-monopole) in three spatial dimensions.

$$
\boxed{\pi_0:\ \text{walls},\qquad\pi_1:\ \text{strings},\qquad\pi_2:\ \text{monopoles}.}
$$

During the transition, initially uncorrelated vacuum choices in causally separated regions can generate these boundary classes through the [Kibble mechanism](../../../critical-phenomenon.md#kibble-mechanism). Nontrivial topology allows stable defects; it does not specify their exact formation efficiency or abundance.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Abelian Higgs model](../../../classical-field-theory-soliton.md#abelian-higgs-model) has local $G=U(1)$, and a nonzero minimally charged scalar expectation value has trivial [stabilizer](../../../group-theory.md#stabilizer-subgroup) $H=\{1\}$. Thus $M\simeq U(1)\simeq S^1$ and $\pi_1(M)=\mathbb Z$, while $\pi_0$ and $\pi_2$ are trivial. The defects are local strings, or [Nielsen-Olesen vortices](../../../classical-field-theory-soliton.md#nielsen-olesen-vortex), whose winding fixes flux $2\pi n/e$.

Put $R=\eta+\phi/\sqrt2$ and $\vartheta=\psi/(\eta\sqrt2)$. The specified gauge-field shift is $A=A'+\partial\vartheta/e$, so

$$
D_\mu\Phi=e^{i\vartheta}(\partial_\mu R-ieA'_\mu R),\qquad
|D\Phi|^2=\frac12(\partial\phi)^2+e^2R^2A'_\mu A'^{\mu},\qquad F(A)=F(A').
$$

Expanding the potential gives $V=\lambda\eta^2\phi^2/2+O(\phi^3)$. Hence the [broken-phase spectrum of the Abelian Higgs model](../../../classical-field-theory-soliton.md#broken-phase-spectrum-of-the-abelian-higgs-model) follows from

$$
\mathcal L_2=\frac12(\partial\phi)^2-\frac12\lambda\eta^2\phi^2
-\frac14F'_{\mu\nu}F'^{\mu\nu}+\frac12(2e^2\eta^2)A'_\mu A'^{\mu}:
$$



$$
\boxed{m_\phi=\sqrt\lambda\eta\quad\text{one real scalar},\qquad
m_A=\sqrt2e\eta\quad\text{one massive vector}.}
$$

The phase is not an additional physical massless scalar: the [Higgs mechanism](../../../standard-model.md#higgs-mechanism) supplies the vector's longitudinal polarization. In the symmetric phase the [complex scalar](../../../scalar-field-theory.md#complex-scalar-field) has two real [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) and the massless vector has two polarizations, a total of four. In the broken phase there are one scalar and three massive-vector polarizations, again four. The symmetric phase is the thermally restored phase; the origin of the given zero-temperature potential is unstable, not a separate stable particle vacuum. The local polar change of variables cannot remove global vortex winding everywhere, so the massive spectrum is consistent with string defects.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

The [SU(5) grand unified theory](../../../perturbative-quantum-field-theory.md#su-5-grand-unified-theory) has [simply connected space](../../../algebraic-topology.md#simply-connected-space) $G=SU(5)$ and a connected [Standard Model](../../../standard-model.md) subgroup. More precisely that subgroup is $(SU(3)\times SU(2)\times U(1))/\mathbb Z_6$; the product notation suppresses a finite central quotient. The [long exact sequence of homotopy groups of a fibration](../../../algebraic-topology.md#long-exact-sequence-of-homotopy-groups-of-a-fibration) $H\to G\to G/H$ gives

$$
\pi_2(G/H)\simeq\pi_1(H)\simeq\mathbb Z,\qquad
\pi_1(G/H)\simeq\pi_0(H)=0.
$$

Thus stable [magnetic monopoles](../../../physics.md#magnetic-monopole) form, whereas this transition does not require walls or strings. The [monopole core and mass scales in an SU(5) transition](../../../perturbative-quantum-field-theory.md#monopole-core-and-mass-scales-in-an-su-5-transition) are set by the massive gauge and [scalar fields](../../../quantum-field-theory.md#scalar-field):

$$
\boxed{r_V\sim(g\eta)^{-1},\qquad r_\phi\sim(\sqrt\lambda\eta)^{-1},\qquad
M_M\sim\frac{4\pi\eta}{g}\times\text{an order-one profile factor}.}
$$

For order-one couplings, the core size is of order $\eta^{-1}$ and the mass is of order $\eta$ up to the often substantial factor $4\pi/g$. These heavy objects are nonrelativistic soon after formation and can survive as stable relics.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Take the transition temperature $T_i\sim\eta$ and [radiation-dominated universe](../../../cosmology.md#radiation-dominated-universe). With $g_*\simeq100$ relativistic [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom), $\rho_{r,i}=(\pi^2/30)g_*T_i^4$ and the [Friedmann equation](../../../cosmology.md#friedmann-equations) gives

$$
H_i\simeq1.66\sqrt{g_*}\frac{\eta^2}{m_{\rm pl}},\qquad
\boxed{t_i\simeq\frac{0.301m_{\rm pl}}{\sqrt{g_*}\eta^2}
\simeq2.4\times10^{-39}\,\mathrm{s}\left(\frac{10^{16}\,\mathrm{GeV}}\eta\right)^2.}
$$

A saturated causal correlation length is of order the radiation-era horizon $H_i^{-1}=2t_i$. Write $C_n\sim1$ for the geometric/formation efficiency and $C_M=M_M/\eta$. One monopole per horizon volume gives the [horizon-density monopole abundance bound](../../../cosmology.md#horizon-density-monopole-abundance-bound) estimate

$$
\boxed{n_i\sim C_nH_i^3=C_n(1.66)^3g_*^{3/2}\frac{\eta^6}{m_{\rm pl}^3},\qquad
\rho_i\sim M_Mn_i=C_nC_M(1.66)^3g_*^{3/2}\frac{\eta^7}{m_{\rm pl}^3}.}
$$

The first quantity is number density and the second is defect energy density. Relative to the initial radiation [critical density](../../../cosmology.md#critical-density),

$$
\frac{\rho_i}{\rho_{r,i}}\sim13.9\,C_nC_M\sqrt{g_*}\left(\frac\eta{m_{\rm pl}}\right)^3.
$$

This can initially be small even when the surviving monopole abundance is unacceptable today. Causality supplies an order-of-magnitude lower abundance estimate under the stipulated saturation; it is not a precise statistical count of defects.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

Without substantial annihilation or decay, monopole number in a comoving volume is conserved. Hence $n_M\propto a^{-3}$ and, for constant nonrelativistic mass, $\rho_M\propto a^{-3}$. Radiation redshifts as $a^{-4}$, so the monopole-to-radiation ratio grows with $a$.

Use [comoving entropy conservation](../../../cosmology.md#comoving-entropy-conservation) rather than assuming the same relativistic content at every epoch:

$$
\left(\frac{a_i}{a_0}\right)^3=\frac{g_{*s,0}}{g_{*s,i}}\left(\frac{T_0}\eta\right)^3.
$$

With $g_{*s,i}\simeq100$, $g_{*s,0}\simeq3.91$ and $T_0\simeq2.35\times10^{-13}\,\mathrm{GeV}$, the surviving energy density is

$$
\rho_{M0}\sim C_nC_M(1.66)^3g_*^{3/2}\frac{g_{*s,0}}{g_{*s,i}}
\frac{\eta^4T_0^3}{m_{\rm pl}^3}.
$$

Taking $m_{\rm pl}\simeq1.22\times10^{19}\,\mathrm{GeV}$ and $H_0\simeq70\,\mathrm{km\,s^{-1}\,Mpc^{-1}}$ gives $\rho_{{\rm crit},0}\simeq4.0\times10^{-47}\,\mathrm{GeV}^4$. Requiring $\rho_{M0}<0.01\rho_{{\rm crit},0}$ yields

$$
\boxed{\eta\lesssim1.3\times10^{11}\,\mathrm{GeV}\,(C_nC_M)^{-1/4}
\left(\frac{H_0}{70\,\mathrm{km\,s^{-1}\,Mpc^{-1}}}\right)^{1/2}.}
$$

Unknown geometric and mass prefactors change this estimate only through a fourth root. Conventional grand-unification scales near $10^{15}$–$10^{16}\,\mathrm{GeV}$ are far above the bound: this is the [cosmological monopole problem](../../../cosmology.md#cosmological-monopole-problem), not a universal prohibition on unification. Inflation after monopole formation can dilute the relics; [reheating](../../../cosmic-inflation.md#reheating) must then stay below their regeneration temperature. Later [entropy](../../../thermodynamics.md#entropy) production, efficient annihilation, or a symmetry-breaking history avoiding stable monopoles can also weaken the bound. These mechanisms change the assumed conserved initial relic abundance.

## 4

↑ **Parent:** [Paper 70](paper-70.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Each separately conserved component obeys the [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) $\rho\propto a^{-3(1+w)}$. For the flat [Friedmann-Lemaître-Robertson-Walker metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric), the [Friedmann equations](../../../cosmology.md#friedmann-equations) therefore give

$$
\frac{H(z)^2}{H_0^2}=\Omega_m(1+z)^3+\Omega_r(1+z)^4+\Omega_X(1+z)^{3(1+w)}.
$$

Write $H(z)/H_0=1+h_1z+O(z^2)$, where $h_1=[3\Omega_m+4\Omega_r+3(1+w)\Omega_X]/2$. Expanding the reciprocal inside the [luminosity distance](../../../cosmology.md#luminosity-distance) integral gives

$$
H_0d_L=(1+z)\left[z-\frac{h_1}2z^2+O(z^3)\right]
=z+\left(1-\frac{h_1}2\right)z^2+O(z^3).
$$

Matching its quadratic coefficient gives the [deceleration parameter](../../../cosmology.md#deceleration-parameter) $q_0=h_1-1$. Using flatness in this part,

$$
\boxed{q_0=\frac{\Omega_m}2+\Omega_r+\frac{1+3w}{2}\Omega_X
=\frac12\left(1+\Omega_r+3w\Omega_X\right).}
$$

A negative [deceleration parameter](../../../cosmology.md#deceleration-parameter) signifies accelerated expansion; negative pressure must overcome the positive matter and radiation terms. Restoring units replaces $H_0d_L$ by $H_0d_L/c$ in the expansion, leaving $q_0$ unchanged.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In the observational setting of this paper, the [cosmic microwave background](../../../cosmology.md#cosmic-microwave-background) favours nearly flat geometry, while cluster dynamics and large-scale structure favour a matter density near $\Omega_m\sim0.3$. The missing contribution to the [critical density](../../../cosmology.md#critical-density) is then roughly $\Omega_X\sim0.7$. The supernova [luminosity distance](../../../cosmology.md#luminosity-distance) measurements require recent accelerated expansion. With present radiation negligible, $q_0<0$ requires

$$
\boxed{w< -\frac1{3\Omega_X}\simeq-0.48\quad(\Omega_X\simeq0.7).}
$$

For an X-dominated universe the threshold would instead be $w<-1/3$. Thus X cannot be ordinary pressureless matter or radiation. It must be comparatively smooth on cluster scales, so that it contributes to the background expansion without being counted as clustered dynamical matter. Its negative pressure makes its density dilute more slowly than matter, allowing late dominance. A [cosmological constant](../../../cosmology.md#cosmological-constant), with $w=-1$, or sufficiently potential-dominated [quintessence](../../../cosmology.md#quintessence-physics) can have these properties.

The comparison with a [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) needs a distinction between background stress and perturbations. A homogeneous canonical scalar has [canonical scalar stress as a perfect fluid](../../../general-relativity.md#canonical-scalar-stress-as-a-perfect-fluid):

$$
\rho=K+V,\qquad p=K-V,\qquad K=\dot\phi^2/2.
$$

It has isotropic pressure and no background shear stress, just as a [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) does. Negative pressure therefore does not, by itself, prevent a perfect-fluid description. However, an adiabatic [barotropic fluid](../../../fluid-mechanics.md#barotropic-fluid) with the constant closure $p=w\rho$ would have $c_s^2=dp/d\rho=w$. For negative $w$, a short-wavelength density mode then has $\omega^2\simeq wk_{\rm phys}^2<0$, the [negative-w barotropic-fluid gradient instability](../../../cosmology.md#negative-w-barotropic-fluid-gradient-instability). Such a closure cannot give a stable, smooth propagating X component.

A canonical scalar instead has rest-frame [sound speed](../../../compressible-flow.md#speed-of-sound) squared equal to one: its spatial and temporal kinetic terms have the same coefficient. Its pressure perturbation need not obey the background relation $\delta p=w\delta\rho$. This nonadiabatic response suppresses small-scale clustering without the negative-sound-speed instability. A [cosmological constant](../../../cosmology.md#cosmological-constant) is a separate limiting case with no independent propagating fluid density mode. Thus the issue is the microphysics and perturbation closure, not whether the background [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor) has perfect-fluid form.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Varying the canonical scalar action gives $\Box\phi+V_{,\phi}=0$. In a homogeneous flat [Friedmann-Lemaître-Robertson-Walker metric](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) written in [conformal time](../../../cosmology.md#conformal-time), $\sqrt{-g}=a^4$ and $g^{00}=a^{-2}$, so

$$
\Box\phi=\frac1{a^4}\partial_\tau(a^2\phi')
=\frac1{a^2}\left(\phi''+2\frac{a'}a\phi'\right).
$$

The quadratic potential therefore gives

$$
\boxed{\phi''+2\frac{a'}a\phi'+a^2m^2\phi=0.}
$$

Equivalently $\ddot\phi+3H\dot\phi+m^2\phi=0$ in cosmic time. The intrinsic roll/oscillation time is $m^{-1}$ and the damping time is $H^{-1}$. If $m\gg H_0$, the scalar has long since begun rapid oscillations: averaging over a quadratic oscillation gives equal kinetic and potential energies, $\langle p\rangle\simeq0$, so it behaves as matter rather than accelerating [dark energy](../../../cosmology.md#dark-energy). To remain nearly frozen or only begin rolling today requires the [mass scale of quadratic quintessence](../../../cosmology.md#mass-scale-of-quadratic-quintessence)

$$
\boxed{m\lesssim H_0\sim2.3\times10^{-18}\,\mathrm{s}^{-1}
\sim1.5\times10^{-33}\,\mathrm{eV}.}
$$

If its energy is predominantly potential, equating $m^2\phi_0^2/2$ to $\rho_{X0}=3M^2H_0^2\Omega_X$, with $M$ the [reduced Planck mass](../../../physics.md#reduced-planck-mass), gives

$$
\boxed{|\phi_0|\simeq\sqrt{6\Omega_X}\,M\frac{H_0}{m}.}
$$

Taking the natural onset estimate $m\sim H_0$ and $\Omega_X\sim0.7$ gives $|\phi_0|\sim2M\sim5\times10^{18}\,\mathrm{GeV}$, of order the [Planck mass](../../../physics.md#planck-mass). More strongly frozen, negative-pressure evolution requires a smaller mass and correspondingly larger field. The density fixes the product $m|\phi_0|$ at this accuracy, rather than a unique mass and field separately.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

There are two normalization problems in the printed energy identity. In [conformal time](../../../cosmology.md#conformal-time), the physical density of a homogeneous scalar is $T_{00}/a^2$, and its kinetic contribution contains $\phi'^2$, not one power of $\phi'$. The [conformal density of a canonical scalar field](../../../general-relativity.md#conformal-density-of-a-canonical-scalar-field) follows directly from the [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor):

$$
\rho_\phi=\frac{\phi'^2}{2a^2}+V,\qquad
p_\phi=\frac{\phi'^2}{2a^2}-V,\qquad T_{00}=a^2\rho_\phi.
$$

Writing $K=\phi'^2/(2a^2)$, the condition $K-V=-(K+V)/3$ gives $V=2K$, hence

$$
\boxed{K=\rho_\phi/3,\qquad V=2\rho_\phi/3,\qquad
\phi'^2=\frac{2a^2\rho_\phi}{3}=\frac{2T_{00}}3.}
$$

The reconstruction is consistent with this corrected identity; the unsquared printed identity cannot hold as an energy relation.

The [constant-equation-of-state density scaling](../../../cosmology.md#constant-equation-of-state-density-scaling) for this [coasting fluid](../../../cosmology.md#coasting-fluid) gives $\rho_\phi=\rho_{X0}a^{-2}$, where $\rho_{X0}=3M^2H_0^2\Omega_X$. Choose the branch on which $\phi$ increases. Then

$$
\phi'=\sqrt2MH_0\sqrt{\Omega_X},\qquad
V=\frac{2M^2H_0^2\Omega_X}{a^2}.
$$

Keeping all three density parameters explicitly, the [Friedmann equations](../../../cosmology.md#friedmann-equations) in [conformal time](../../../cosmology.md#conformal-time) give

$$
a'^2=H_0^2\left(\Omega_r+\Omega_ma+\Omega_Xa^2\right),\qquad
\frac{da}{d\phi}=\frac1{\sqrt2M}
\sqrt{a^2+\frac{\Omega_m}{\Omega_X}a+\frac{\Omega_r}{\Omega_X}}.
$$

For $\Omega_X>0$, define

$$
b=\frac{\Omega_m}{2\Omega_X},\qquad
A=\frac{\sqrt{\Omega_m^2/4-\Omega_r\Omega_X}}{\Omega_X}.
$$

The square root is $\sqrt{(a+b)^2-A^2}$. Integrating on the expanding branch gives

$$
\operatorname{arcosh}\frac{a+b}{A}
=\frac{\phi-\phi_0}{\sqrt2M}+C,
$$

where $a(\phi_0)=1$. Thus the [scalar-field reconstruction of a coasting component](../../../cosmology.md#scalar-field-reconstruction-of-a-coasting-component) is

$$
\boxed{a=A\cosh[B(\phi-\phi_0)+C]+D,\quad
B=\frac1{\sqrt2M}=\frac{\sqrt{4\pi}}{m_{\rm pl}},\quad
C=\operatorname{arcosh}\frac{1+b}{A},\quad D=-b.}
$$

Substitution into the potential gives the requested present-field parametrization:

$$
\boxed{V(\phi)=\frac{2M^2H_0^2\Omega_X}
{\left[A\cosh\left(\frac{\phi-\phi_0}{\sqrt2M}+C\right)-b\right]^2}.}
$$

The domain is the branch where $a>0$ and the hyperbolic argument is positive; reversing the direction of the field changes the sign of $B$. The actual discriminant condition is $\Omega_m^2/4>\Omega_r\Omega_X$. The supplied stronger bound suffices for physical density fractions $0<\Omega_X\le1$. No density parameter has been eliminated using the flatness sum.

As a check, $\phi'$ is constant and $V_{,\phi}=-2V(a'/a)/\phi'$. Since $a^2V=\phi'^2$ along this solution, $\phi''+2(a'/a)\phi'+a^2V_{,\phi}=0$ identically. The reconstructed field therefore satisfies its equation of motion as well as the [Friedmann equations](../../../cosmology.md#friedmann-equations) and required [equation of state](../../../thermodynamics.md#equation-of-state).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
