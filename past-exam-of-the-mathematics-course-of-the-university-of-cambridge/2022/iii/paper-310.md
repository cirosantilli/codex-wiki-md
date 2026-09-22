# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_310.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
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

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation) is

$$
\dot\rho+3H(\rho+p)=0.
$$

For constant [equation-of-state parameter](../../../cosmology.md#equation-of-state-parameter) $w=p/\rho$, integration gives

$$
\rho_i(a)=\rho_{i,0}a^{-3(1+w_i)}
=\rho_{i,0}(1+z)^{3(1+w_i)},
$$

where $a_0=1$. Define the present [cosmological density parameter](../../../cosmology.md#cosmological-density-parameter)

$$
\Omega_{i,0}=\frac{\rho_{i,0}}{\rho_{c,0}},
\qquad
\rho_{c,0}=\frac{3H_0^2}{8\pi G}.
$$

The [Friedmann equation](../../../cosmology.md#friedmann-equations) then gives

$$
\boxed{H(z)=H_0E(z),\qquad
E(z)=\left[\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}\right]^{1/2}}.
$$

Spatial curvature may be included as an effective $w=-1/3$ component. Once the parameters are specified, the scale factor follows from the first-order equation $\dot a=aH(a)$, or equivalently

$$
\boxed{t(a)-t(a_i)=\int_{a_i}^a\frac{da'}{a'H(a')}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a variable equation of state, continuity gives

$$
\rho_{\rm DE}(z)=\rho_{{\rm DE},0}
\exp\!\left[3\int_0^z\frac{1+w(z')}{1+z'},dz'\right].
$$

For the [Chevallier-Polarski-Linder parametrization](../../../cosmology.md#chevallier-polarski-linder-parametrization)

$$
w(z)=w_0+w_a\frac{z}{1+z},
$$

the integral is

$$
(1+w_0+w_a)\log(1+z)-w_a\frac{z}{1+z}.
$$

Consequently

$$
\boxed{X(\Omega_{{\rm DE},0},z,w_0,w_a)
=\Omega_{{\rm DE},0}(1+z)^{3(1+w_0+w_a)}
e^{-3w_az/(1+z)}}
$$

and

$$
\boxed{H(z)=H_0\left[\Omega_{m,0}(1+z)^3+X\right]^{1/2}}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For successive wavecrests from the same comoving source, $1+z=a(t_0)/a(t_s)$. Therefore

$$
\Delta z=\frac{a(t_0+\Delta t_0)}{a(t_s+\Delta t_s)}
-\frac{a(t_0)}{a(t_s)}.
$$

The same radial null path implies equality of the elapsed [conformal time](../../../cosmology.md#conformal-time),

$$
\frac{\Delta t_s}{a(t_s)}=\frac{\Delta t_0}{a(t_0)},
\qquad
\Delta t_s=\frac{\Delta t_0}{1+z_1}.
$$

Expanding both scale factors to first order gives the [redshift drift](../../../cosmology.md#redshift-drift)

$$
\boxed{\Delta z
=\left[(1+z_1)H_0-H(z_1)\right]\Delta t_0
=H_0\Delta t_0\left[1+z_1-E(z_1)\right]}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Measurements at many source redshifts directly sample the function $H_0[1+z-E(z)]$. In principle, sufficiently many precise and well-spaced measurements can fit $H_0,\Omega_{m,0},\Omega_{{\rm DE},0},w_0,w_a$ simultaneously; a single redshift supplies only one combination and cannot. In a spatially flat two-component model, $\Omega_{m,0}+\Omega_{{\rm DE},0}=1$, reducing the number of independent parameters by one. In practice the signal accumulated over ten years is extremely small and parameter degeneracies require broad redshift coverage and complementary data.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) for $e^-+p\leftrightarrow H+\gamma$ requires $\mu_e+\mu_p=\mu_H$, since the photon chemical potential vanishes. Inserting the nonrelativistic [Maxwell-Boltzmann distribution](../../../statistical-physics.md#maxwell-boltzmann-distribution) and using charge neutrality $n_p=n_e$ gives

$$
\frac{n_H}{n_e^2}
=\left(\frac{2\pi}{m_eT}\right)^{3/2}
\exp\!\left(\frac{m_e+m_p-m_H}{T}\right),
$$

where the proton-to-hydrogen mass ratio and the stated degeneracy factors have been approximated by one. Thus

$$
\boxed{\left(\frac{n_H}{n_e^2}\right)_{\rm eq}
=\left(\frac{2\pi}{m_eT}\right)^{3/2}e^{B_H/T}}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

With $X_e=n_e/n_b$, charge neutrality and $n_b=n_p+n_H$ give

$$
n_e=X_en_b,
\qquad n_H=(1-X_e)n_b.
$$

Multiplying part a by $n_b=\eta n_\gamma$ and using $n_\gamma=2\zeta(3)T^3/\pi^2$ yields the [Saha ionization equation](../../../cosmology.md#saha-ionization-equation)

$$
\boxed{\left(\frac{1-X_e}{X_e^2}\right)_{\rm eq}
=\frac{2\zeta(3)}{\pi^2}\eta
\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{B_H/T}}.
$$

Although $T\ll B_H$ suppresses ionization of an individual atom, the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) is only about $10^{-9}$. The enormous number of photons per baryon leaves enough photons in the high-energy thermal tail to ionize hydrogen until $T\simeq0.3\,\mathrm{eV}$, far below $B_H$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

[Photon decoupling](../../../cosmology.md#photon-decoupling) occurs when the Thomson interaction rate falls below the expansion rate,

$$
\Gamma_\gamma=n_e\sigma_T\simeq H.
$$

At decoupling the universe is approximately matter dominated, so

$$
H(T)=H_0\sqrt{\Omega_{m,0}}
\left(\frac{T}{T_0}\right)^{3/2}.
$$

Using $n_e=X_e\eta(2\zeta(3)/\pi^2)T^3$ in $\Gamma_\gamma=H$ gives

$$
\boxed{X_e(T_{\rm dec})T_{\rm dec}^{3/2}
\simeq\frac{\pi^2H_0\sqrt{\Omega_{m,0}}}
{2\zeta(3)\eta\sigma_TT_0^{3/2}}}.
$$

For $X_e\ll1$, the Saha equation makes $X_e(T)$ exponentially steep through $e^{-B_H/(2T)}$. Power-law changes of $H_0$ or $\Omega_{m,0}$ therefore cause only a small shift in $T_{\rm dec}$, explaining why $T_{\rm dec}\simeq T_{\rm rec}$ is a good approximation.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

At fixed $\eta$, the [recombination temperature](../../../cosmology.md#recombination-temperature) is determined by atomic physics and the Saha equation, not by today's CMB temperature. Under the stated approximation,

$$
\boxed{\frac{T_{{\rm dec},1\rm K}}{T_{{\rm dec},2.73\rm K}}=1}.
$$

Since $1+z_{\rm dec}=T_{\rm dec}/T_0$,

$$
\boxed{\frac{1+z_{{\rm dec},1\rm K}}
{1+z_{{\rm dec},2.73\rm K}}=2.73},
$$

and the same ratio holds for the large redshifts themselves to excellent accuracy. The comoving distance $\chi_{\rm dec}=\int_0^{z_{\rm dec}}dz/H(z)$ can nevertheless be held fixed by adjusting the late-time expansion history, for example $H_0$, $\Omega_{m,0}$, spatial curvature, or dark-energy density and equation-of-state parameters.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $4\pi G\bar\rho_m=3H^2/2$ and $a\propto t^{2/3}$. Substitution of $\delta_m\propto t^p$ gives $p=2/3,-1$, hence

$$
\boxed{\delta_m=C_1a+C_2a^{-3/2}}.
$$

During [radiation domination](../../../linear-cosmological-density-perturbation.md#radiation-domination), neglecting the rapidly oscillating radiation perturbation and the subdominant matter source leaves

$$
\ddot\delta_m+2H\dot\delta_m=0,
\qquad a\propto t^{1/2}.
$$

Therefore

$$
\boxed{\delta_m=C_3+C_4\log a}.
$$

This logarithmic behavior is the [Mészáros effect](../../../linear-cosmological-density-perturbation.md#meszaros-effect) for subhorizon cold dark matter.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For an approximately scale-invariant primordial spectrum, the late [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) behaves schematically as

$$
P(k)\propto k^{n_s}T^2(k).
$$

Modes with $k\ll k_{\rm eq}$ enter the horizon after matter-radiation equality and retain $T(k)\simeq1$, so $P(k)\sim k^{n_s}$. Modes with $k\gg k_{\rm eq}$ enter during radiation domination and grow only logarithmically until equality. Their transfer function behaves as $T(k)\sim\log(k/k_{\rm eq})/(k/k_{\rm eq})^2$, giving a strongly falling small-scale spectrum. The result is a turnover near the [matter-radiation equality scale](../../../cosmology.md#matter-radiation-equality-scale) $k_{\rm eq}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The Fourier-space [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives

$$
\phi(\mathbf k,\tau)
=-\frac{4\pi Ga^2\bar\rho_m}{k^2}\delta_m
=-\frac{3\Omega_{m,0}H_0^2}{2ak^2}\delta_m.
$$

Insert this into the line-of-sight expression for the [CMB lensing potential](../../../cosmic-microwave-background-anisotropy.md#cmb-lensing-potential), Fourier transform $\delta_m$, and use the [Rayleigh plane-wave expansion](../../../analysis.md#rayleigh-plane-wave-expansion). Projection onto $Y_{lm}$ and spherical-harmonic orthogonality give

$$
\boxed{
a_{lm}^\psi=12\pi\Omega_{m,0}H_0^2i^{-l}
\int_0^{\chi_e}d\chi
\int\frac{d^3k}{(2\pi)^3}
\frac1{k^2}\frac{\chi_e-\chi}{\chi\chi_e}
\frac{\delta_m(\mathbf k,\tau)}{a(\tau)}
j_l(k\chi)Y_{lm}^*(\widehat{\mathbf k})}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Define the radial transfer integral

$$
F_l(k)=\int_0^{\chi_e}d\chi\,
\frac{\chi_e-\chi}{\chi\chi_e}
\frac{D_i(\tau_0-\chi)}{a(\tau_0-\chi)}j_l(k\chi),
$$

where $\delta_m(\mathbf k,\tau)=D_i(\tau)\delta_m(\mathbf k,\tau_i)$ and $D_i(\tau_i)=1$. With

$$
\langle\delta_m(\mathbf k,\tau_i)\delta_m^*(\mathbf k',\tau_i)\rangle
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k')P_i(k),
$$

the angular and radial integrations give

$$
\boxed{C_l^\psi
=\frac{18}{\pi}\Omega_{m,0}^2H_0^4
\int_0^\infty\frac{dk}{k^2}P_i(k)F_l^2(k)}.
$$

This expression makes the lensing signal a weighted projection of the evolving matter power spectrum.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The creation and annihilation operators obey the [canonical commutation relations](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}^\dagger]
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k'),
\qquad
[\widehat a_{\mathbf k},\widehat a_{\mathbf k'}]
=[\widehat a_{\mathbf k}^\dagger,\widehat a_{\mathbf k'}^\dagger]=0.
$$

Since $\delta\widehat\phi=\widehat f/a$, the vacuum two-point function identifies

$$
\Delta_{\delta\phi}^2(k,\tau)
=\frac{k^3}{2\pi^2}\frac{|f_k(\tau)|^2}{a^2}
=\frac{H^2}{4\pi^2}(1+k^2\tau^2).
$$

On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), $|k\tau|=k/(aH)\ll1$, so

$$
\boxed{\Delta_{\delta\phi}^2=\left(\frac H{2\pi}\right)^2}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For each mode, the right side of

$$
\Delta_{\mathcal R}^2(k)=\frac1{2\epsilon M_{\rm Pl}^2}
\left(\frac H{2\pi}\right)^2
$$

is evaluated at [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $k=aH$. Since

$$
\frac{d\log H}{dN}=-\epsilon,
\qquad
\frac{d\log\epsilon}{dN}=\eta,
\qquad
\frac{d\log k}{dN}=1-\epsilon,
$$

first order in the [Hubble slow-roll parameters](../../../cosmic-inflation.md#hubble-slow-roll-parameter) gives

$$
\boxed{n_s-1=\frac{d\log\Delta_{\mathcal R}^2}{d\log k}
=-2\epsilon-\eta}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For the [monomial inflation potential](../../../cosmic-inflation.md#monomial-inflation-potential) $V=\lambda M_{\rm Pl}^4(\phi/M_{\rm Pl})^\alpha$,

$$
\epsilon\simeq\frac{M_{\rm Pl}^2}{2}\left(\frac{V_{,\phi}}V\right)^2
=\frac{\alpha^2M_{\rm Pl}^2}{2\phi^2},
$$

and

$$
\eta=4\epsilon-2M_{\rm Pl}^2\frac{V_{,\phi\phi}}V
=\frac{2\alpha M_{\rm Pl}^2}{\phi^2}.
$$

Slow-roll inflation is possible when both are much smaller than one:

$$
\frac{\phi^2}{M_{\rm Pl}^2}\gg
\max\!\left(\frac{\alpha^2}{2},2\alpha\right).
$$

Inflation ends once one of these conditions fails, commonly near $|\phi|\simeq\alpha M_{\rm Pl}/\sqrt2$ when $\epsilon\simeq1$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The expressions in part c imply

$$
\eta=\frac4\alpha\epsilon,
\qquad
n_s-1=-2\epsilon\left(1+\frac2\alpha\right).
$$

Since the [tensor-to-scalar ratio](../../../cosmic-inflation.md#tensor-to-scalar-ratio) is $r=16\epsilon$,

$$
\boxed{n_s-1=-\frac{\alpha+2}{8\alpha}r}.
$$

For positive $\alpha$, this class predicts a red scalar tilt and

$$
0<r<8(1-n_s).
$$

A blue tilt with positive $r$, or $r\geq8(1-n_s)$, is incompatible. An allowed pair fixes $\alpha=2r/[8(1-n_s)-r]$, subject to slow roll and observational bounds.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
